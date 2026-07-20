# Anonimización de Datos

## Introducción

La anonimización de datos es un proceso fundamental para proteger la privacidad de las personas al utilizar información en análisis, inteligencia artificial, investigación o intercambio de datos. Su objetivo no es simplemente eliminar nombres, sino reducir al mínimo la posibilidad de que una persona pueda ser identificada.

En la práctica, las empresas aplican diferentes técnicas según el nivel de protección requerido y el uso que tendrán los datos.

---

# Anonimización vs. Seudonimización

Es importante distinguir estos dos conceptos.

| Concepto            | ¿Se puede identificar nuevamente a la persona? | Ejemplo                  |
| ------------------- | ---------------------------------------------- | ------------------------ |
| **Anonimización**   | No, de forma razonable.                        | `1992-04-13 → 1992`      |
| **Seudonimización** | Sí, si existe una tabla de correspondencia.    | `Juan Pérez → ID_847291` |

La **seudonimización** es muy utilizada en las empresas porque permite relacionar información del mismo usuario sin almacenar sus datos personales en cada registro.

---

# Técnicas de anonimización más utilizadas

## Eliminación de identificadores directos

Consiste en eliminar información que identifica de manera directa a una persona, como:

* Nombre y apellido
* DNI o pasaporte
* Correo electrónico
* Teléfono
* Dirección

### Antes

| Nombre     | Email                                   | Compra  |
| ---------- | --------------------------------------- | ------- |
| Juan Pérez | [juan@gmail.com](mailto:juan@gmail.com) | $25.000 |

### Después

| ID     | Compra  |
| ------ | ------- |
| 847291 | $25.000 |

---

## Hashing

Convierte un dato en un valor irreversible mediante una función hash (por ejemplo, SHA-256).

```text
juan@gmail.com
```

↓

```text
3f5c1e8a9d...
```

Permite detectar registros repetidos sin almacenar el dato original.

> **Importante:** para evitar ataques por fuerza bruta suele combinarse con una técnica denominada **salting**, que agrega un valor aleatorio antes de calcular el hash.

---

## Tokenización

Reemplaza un dato sensible por un identificador (token), manteniendo el valor real almacenado en un entorno altamente protegido.

```text
Tarjeta: 4509 1234 5678 9999
Token:   tok_7fA92KQ
```

Es una técnica ampliamente utilizada por plataformas de pago.

---

## Generalización

Reduce el nivel de detalle de la información para evitar identificar personas mediante combinaciones únicas de datos.

| Original        | Generalizado         |
| --------------- | -------------------- |
| 1992-04-13      | 1992                 |
| 34 años         | 30–39                |
| Córdoba Capital | Provincia de Córdoba |
| CP 5000         | CP 50xx              |

---

## K-Anonymity

Busca que cada registro sea indistinguible de al menos **k-1** personas.

Por ejemplo, en lugar de almacenar:

| Edad | Ciudad      |
| ---- | ----------- |
| 34   | Villa María |

se generaliza la información:

| Edad  | Región         |
| ----- | -------------- |
| 30–39 | Córdoba Centro |

Esta técnica es muy utilizada en el ámbito de la salud y la investigación.

---

## Differential Privacy

Consiste en introducir pequeñas alteraciones aleatorias en los datos para proteger la privacidad individual sin afectar significativamente las estadísticas globales.

Por ejemplo, en lugar de reportar exactamente **100 usuarios**, un sistema podría informar **97** o **102**.

Empresas como **Apple**, **Google** y **Microsoft** utilizan este enfoque para publicar estadísticas preservando la privacidad.

---

# Uso de datos en Inteligencia Artificial

Antes de utilizar información para entrenar modelos de IA, normalmente se sigue un proceso similar al siguiente:

```text
Datos originales
       │
       ▼
 ETL seguro
       │
       ▼
Anonimización
       │
       ▼
 Dataset para IA
```

Durante este proceso también es habitual aplicar:

* Accesos restringidos.
* Separación de la información personal (PII).
* Auditorías.
* Controles de seguridad.

---

# Ejemplo

## Datos originales

| Nombre           | Teléfono     | Dirección      | Pedido |
| ---------------- | ------------ | -------------- | ------ |
| Esteban Calabria | 351-555-1234 | Av. Colón 1234 | Pizza  |

## Datos para análisis

| User_ID | Zona           | Edad  | Pedido |
| ------- | -------------- | ----- | ------ |
| u_98fa  | Córdoba Centro | 40–49 | Pizza  |

De esta forma es posible responder preguntas como:

* ¿Cuántas pizzas se venden?
* ¿Qué zonas realizan más pedidos?
* ¿Qué rango etario consume más?

sin conocer la identidad del cliente.

---

# Riesgo de reidentificación

Anonimizar correctamente no siempre es sencillo.

Un caso muy conocido fue el **Netflix Prize**, donde investigadores lograron reidentificar usuarios combinando datos anónimos de calificaciones con información pública disponible en Internet.

Por este motivo, regulaciones como el **GDPR** (Europa) exigen evaluar el **riesgo de reidentificación**, además de aplicar técnicas de anonimización.

---

# Prácticas habituales en las empresas

Un escenario típico es el siguiente:

| Sistema                   | Información almacenada                        |
| ------------------------- | --------------------------------------------- |
| Base de datos operativa   | Datos completos                               |
| Data Warehouse            | Identificadores seudónimos                    |
| Dashboards                | Datos agregados                               |
| Compartición con terceros | Datos anonimizados o con Differential Privacy |
| Logs                      | Información enmascarada                       |

---

# Tecnologías utilizadas

Algunas herramientas comunes para proteger información sensible son:

* **Microsoft Purview**: descubrimiento y clasificación de datos sensibles.
* **SQL Dynamic Data Masking**: ocultamiento dinámico de columnas.
* **Always Encrypted**: cifrado de información sensible en SQL Server y Azure SQL.
* **Azure OpenAI Data Redaction**: eliminación automática de información personal antes de enviar prompts a modelos de IA.

---

# Conclusión

La anonimización moderna no consiste únicamente en eliminar nombres o correos electrónicos. Su verdadero objetivo es reducir la probabilidad de que una persona pueda ser identificada a partir de un conjunto de datos, permitiendo aprovechar la información para análisis e inteligencia artificial sin comprometer la privacidad de los usuarios.
