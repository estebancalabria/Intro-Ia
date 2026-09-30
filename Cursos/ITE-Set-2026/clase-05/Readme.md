# Clase 05 - 30 de Septiembre del 2026

# Repaso

* Prompt Engineering
  * Tecnicas de prompting
      * Rol / Persona
      * Interaccion / Prompt Chaining
      * Formatos de Salida
        * Simples
          * Tabla
          * Bullets y sub bullets
        * Tecnicos
          * xml
          * json
          * csv (interactuar con y desde excel)
          * codigo de programacion
        * Presenteacion
          * pdf
          * 365 -> Powerpoint. word
          * HTML -> mayor personalizacion
        * Markdown
          * Generacion de plantillas de salida
          * Es el lenguaje con la que la IA responde por defecto
        * Diagramas
            * Mermaind
            * SVG
            * Matplotlib

---

# Prompt Engineering

* Tip: Usar la ia como experto experto en prompt engineerings

# Herrmientas de Productividad (Modulo 4)

## Modalidad de Uso

* Las herramientas de IA generalmente presentan un plan de uso freemium. Donde te permiten cierto uso gratuito limita con renovacion periodica de creditos y si se necesita la herramienta para un uso mas intensivo todas ofrecen planes de pago. Lo que realmente cobran las herramientas son la capacidad de computo de lado del servidor que ofrecen

## Presetnaciones

### Powerpoint en 365

* Con el agente de 365 podemos generar una presentacion facilmente

### Gamma

* Me parece que genera incluso mejores presentaciones que PowerPoint para algunos
* URL
  * https://gamma.app/signup?r=cjucljp9heegmkv
* Caracteristicas
  * Presentacion
  * Graficos
  * Paginas web
  * Publicas para redes Socials

* Con la IA genere este prompt para Gamma

```
# Presentación ejecutiva trimestral — Assurance Seguros

Crea una presentación corporativa ejecutiva para **Assurance Seguros**, una compañía multinacional ficticia de seguros que opera en América Latina, Europa y Norteamérica, ofreciendo seguros de automóviles, hogar, vida y empresas.

## Objetivo

Presentar los resultados del tercer trimestre de 2026 (Q3: julio, agosto y septiembre) ante el comité ejecutivo y los directores regionales. Mostrar resultados financieros y operativos, comparar el desempeño con el trimestre anterior y los objetivos, identificar oportunidades de mejora y establecer prioridades para el cuarto trimestre.

**Importante:** todos los datos, cifras, regiones y resultados son ficticios y se utilizan exclusivamente para una demostración.

## Estructura de la presentación

Crea 10 diapositivas con contenido ejecutivo, análisis cuantitativo y conclusiones respaldadas por los datos.

### 1. Portada

* Assurance Seguros.
* Resultados ejecutivos del tercer trimestre de 2026.
* Período: julio–septiembre de 2026.
* Presentación para el comité ejecutivo.

### 2. Resumen ejecutivo

Presenta los principales indicadores del trimestre:

* Primas emitidas: USD 1.280 millones.
* Crecimiento trimestral: +8,5 %.
* Ratio combinado: 94,8 %.
* Resultado operativo: USD 124 millones.
* Satisfacción del cliente: 84/100.
* Siniestros resueltos dentro del SLA: 91 %.

Incluye tres logros principales y dos desafíos identificados a partir de los datos.

### 3. Resultados financieros

Utiliza los siguientes datos:

| Indicador               |     Q2 2026 |     Q3 2026 | Objetivo Q3 |
| ----------------------- | ----------: | ----------: | ----------: |
| Primas emitidas         | USD 1.180 M | USD 1.280 M | USD 1.250 M |
| Ingresos reconocidos    | USD 1.105 M | USD 1.195 M | USD 1.180 M |
| Resultado operativo     |   USD 105 M |   USD 124 M |   USD 120 M |
| Ratio combinado         |      96,0 % |      94,8 % |      95,0 % |
| Ratio de siniestralidad |      65,0 % |      63,8 % |      64,0 % |
| Ratio de gastos         |      31,0 % |      31,0 % |      31,0 % |

Compara los resultados con Q2 y con los objetivos de Q3. Utiliza tarjetas KPI y gráficos de barras. Expresa las variaciones en porcentajes o puntos porcentuales según corresponda.

### 4. Rentabilidad y eficiencia

Explica la relación entre:

* Ratio de siniestralidad.
* Ratio de gastos.
* Ratio combinado.
* Resultado operativo.

Destaca que el ratio combinado resulta de sumar el ratio de siniestralidad y el ratio de gastos. Identifica las variaciones observadas sin atribuir causas que no estén demostradas por los datos.

### 5. Resultados por región

| Región         |   Primas Q3 | Variación vs. Q2 | Ratio combinado |
| -------------- | ----------: | ---------------: | --------------: |
| América Latina |   USD 420 M |          +11,0 % |          96,2 % |
| Europa         |   USD 510 M |           +6,0 % |          92,5 % |
| Norteamérica   |   USD 350 M |           +8,5 % |          95,4 % |
| Total          | USD 1.280 M |    +8,5 % aprox. |   94,8 % aprox. |

Compara crecimiento, volumen de negocio y rentabilidad técnica por región. Incluye un gráfico comparativo y un mapa estilizado. Señala diferencias regionales que merezcan análisis adicional.

### 6. Desempeño por línea de negocio

| Línea de negocio     |   Primas Q3 | Crecimiento trimestral |           Ratio combinado |
| -------------------- | ----------: | ---------------------: | ------------------------: |
| Automóviles          |   USD 480 M |                 +7,0 % |                    98,5 % |
| Hogar                |   USD 210 M |                 +5,0 % |                    91,0 % |
| Vida                 |   USD 310 M |                +10,0 % | No aplica en este ejemplo |
| Seguros corporativos |   USD 280 M |                +12,0 % |                    91,5 % |
| Total                | USD 1.280 M |                        |                           |

Compara el crecimiento y la contribución de cada línea. Explica que el ratio combinado consolidado debe calcularse sobre las líneas comparables, sin mezclar indicadores de seguros de vida que utilicen métricas de rentabilidad diferentes.

### 7. Operaciones y gestión de siniestros

| Indicador                  |  Q2 2026 |  Q3 2026 | Objetivo Q3 |
| -------------------------- | -------: | -------: | ----------: |
| Siniestros recibidos       |  185.000 |  198.000 |     195.000 |
| Siniestros resueltos       |  176.000 |  193.000 |     190.000 |
| Tiempo medio de resolución | 8,2 días | 6,9 días |    7,0 días |
| Resolución dentro del SLA  |     87 % |     91 % |        90 % |
| Procesamiento automatizado |     42 % |     55 % |        50 % |

Analiza el volumen de trabajo, la velocidad de resolución, el cumplimiento de los SLA y la automatización. Identifica oportunidades para mejorar la eficiencia operativa.

### 8. Experiencia del cliente y transformación digital

| Indicador                         | Q2 2026 | Q3 2026 | Objetivo Q3 |
| --------------------------------- | ------: | ------: | ----------: |
| Satisfacción del cliente          |  81/100 |  84/100 |      83/100 |
| NPS                               |     +32 |     +37 |         +35 |
| Retención de clientes             |  87,5 % |  89,0 % |      88,0 % |
| Operaciones por canales digitales |    61 % |    68 % |        65 % |

Muestra la evolución de los indicadores mediante gráficos sencillos. Distingue entre resultados observados y posibles explicaciones. No afirmes que la digitalización causó mejoras en satisfacción o retención si los datos no permiten establecer esa relación.

### 9. Riesgos, desafíos y oportunidades

Identifica y explica:

* Crecimiento del volumen de siniestros.
* Diferencias de rentabilidad entre regiones y líneas de negocio.
* Costos operativos y de siniestralidad.
* Retención y adquisición de clientes.
* Automatización de procesos.
* Oportunidades de mejora en la experiencia digital.

Separa los hechos medidos de las hipótesis que requieren validación adicional.

### 10. Prioridades para Q4 2026

Utiliza los siguientes objetivos ficticios:

* Primas emitidas: USD 1.350 millones.
* Ratio combinado: inferior al 95 % en las líneas comparables.
* Procesamiento automatizado de siniestros: 62 %.
* Satisfacción del cliente: 86/100.
* Retención de clientes: 90 %.

Presenta tres prioridades estratégicas, los indicadores para realizar su seguimiento y los próximos pasos propuestos.

## Diseño visual

* Formato panorámico 16:9.
* Estética de consultoría estratégica y presentación para comité ejecutivo.
* Paleta corporativa: azul marino, blanco, gris claro y verde azulado.
* Tipografía moderna, profesional y legible.
* Gráficos de barras, líneas de tendencia, tarjetas KPI y tablas compactas.
* Una idea principal por diapositiva.
* Títulos que comuniquen conclusiones, no solamente categorías.
* Uso moderado de iconos y elementos visuales.
* Evitar párrafos extensos, imágenes de stock genéricas y gráficos tridimensionales.
* Mantener consistencia entre cifras, porcentajes, unidades y períodos.
* Indicar siempre si una variación se expresa en porcentaje o en puntos porcentuales.

## Criterios de calidad

La presentación debe tener apariencia de informe interno de una multinacional aseguradora. Utiliza lenguaje ejecutivo, conclusiones concretas y visualizaciones que faciliten la toma de decisiones.

No inventes causas, acontecimientos ni resultados adicionales como si fueran hechos comprobados. Si detectas inconsistencias entre los datos, señálalas o aclara los supuestos antes de elaborar una conclusión. No presentes los datos simulados como resultados reales de una empresa.

Incluye una nota discreta en la portada o al pie de las diapositivas que indique: **“Datos ficticios elaborados exclusivamente para fines demostrativos”.**

```

> [!NOTE]
> Puntaje : 9 / 10

* Vamos a probar tambien generar una landing
 * Prompt : "Haceme una pagina web que sea una landing para una aseguradora"
   * https://tranquilidad-segura-xvzcnol.gamma.site/

---
# Break 
# HAsta y 10
# Despues vemos otra herrmienta
---

# Videos Institucionales

## HEY GEN

* Herramienta para generar videos institucionales

* URL
  * https://www.heygen.com/
 
* Ejemplos de proyectos realizados
  * https://app.heygen.com/videos/llegada-a-la-luna-4fe57c7ee05c4340be90f26fa94d7f24
  * https://app.heygen.com/videos/cambio-climatico-1c6c4d3398ce4de0b06d707d99d87e30
 
* Vamos a crear un video nostoros

* Con ChatGPT genere el siguiente Script

```
Buenos días. Durante el tercer trimestre de 2026, Assurance Seguros registró un desempeño positivo, con primas emitidas por 1.280 millones de dólares, un crecimiento del 8,5 % respecto del trimestre anterior y por encima del objetivo establecido.

El resultado operativo alcanzó los 124 millones de dólares, mientras que el ratio combinado mejoró hasta el 94,8 %, frente al 96 % del trimestre anterior.

A nivel regional, América Latina registró el mayor crecimiento, con un 11 %, mientras que Europa presentó el ratio combinado más bajo, con un 92,5 %.

También observamos avances importantes en operaciones y experiencia del cliente. El 91 % de los siniestros se resolvió dentro del SLA y el procesamiento automatizado aumentó hasta el 55 %. La satisfacción del cliente alcanzó 84 puntos sobre 100 y el NPS llegó a 37.

Para el cuarto trimestre, las prioridades serán mantener el crecimiento, mejorar la eficiencia operativa, aumentar la automatización y continuar fortaleciendo la experiencia del cliente.

```

* Ia a Inicio -> Escena por Escena -> Nuevo Video
 * Abre el editor de video
 * Cargar el Script en la seccion izquierda de la intefaz
 * En la parte derecha podemos elegir el avatar y la voz

----
# Break
Hasta y punto 
----

# Agentes de Programacion (Modulo 7)

* Sirven para generar y alojar sitios web.
* No solamente sitios web estaticos que presentan iformacion, sino aplicaciones completas que pueden resolver un problema concreto

## Lovable
 
* URL
  * Lovable
 
* Vamos a generar una aplicacion para evaluar si un profesional tiene el concocimiento para ejercer su cargo
* Primero vamos a generar con IA un manual de procedimiento ficticio

```
# Manual de Procedimiento

## Normas y procedimientos para operarios de planta embotelladora

**Empresa:** Bebidas del Plata S.A.
**Área:** Producción y Embotellado
**Puesto:** Operario de Planta
**Versión:** 1.0
**Documento ficticio para capacitación**

---

## 1. Objetivo

Establecer las normas y procedimientos que debe cumplir todo operario que trabaje en el área de producción y embotellado, con el objetivo de garantizar:

* La seguridad de los trabajadores.
* La calidad e inocuidad del producto.
* El correcto funcionamiento de los equipos.
* La limpieza y el orden de las instalaciones.
* La trazabilidad de la producción.
* El cumplimiento de los procedimientos internos.

---

## 2. Normas generales de ingreso a planta

Antes de ingresar al área de producción, el operario debe:

1. Registrar su ingreso según el sistema establecido.
2. Utilizar el uniforme correspondiente.
3. Colocarse los elementos de protección personal (EPP).
4. Lavarse y desinfectarse correctamente las manos.
5. Retirar relojes, pulseras, anillos y otros objetos que puedan contaminar el producto o provocar accidentes.
6. Mantener el cabello completamente cubierto.
7. Informar al supervisor cualquier condición que pueda afectar la seguridad o la calidad del producto.

Está prohibido ingresar al área de producción con alimentos, bebidas, cigarrillos u objetos personales no autorizados.

---

## 3. Elementos de protección personal

El operario debe utilizar, según el sector y la tarea:

* Calzado de seguridad.
* Protector auditivo.
* Gafas de seguridad.
* Guantes cuando el procedimiento lo requiera.
* Protección adicional indicada por el supervisor.

Los EPP deben mantenerse limpios y en buenas condiciones.

Si un elemento está deteriorado, debe informarse al supervisor antes de comenzar la tarea.

---

## 4. Higiene personal

Todo operario debe mantener una adecuada higiene personal durante la jornada.

### Es obligatorio:

* Lavarse las manos antes de comenzar a trabajar.
* Lavarse las manos después de utilizar los sanitarios.
* Lavarse las manos después de manipular residuos.
* Mantener las uñas cortas y limpias.
* Utilizar correctamente la indumentaria de trabajo.

### Está prohibido:

* Comer o beber en el área de producción.
* Fumar dentro de las instalaciones.
* Escupir.
* Manipular innecesariamente el producto o los envases.
* Utilizar teléfonos celulares en zonas donde esté prohibido.

---

## 5. Inicio del turno

Antes de iniciar la producción, el operario debe verificar:

1. Que el puesto de trabajo esté limpio.
2. Que no existan objetos extraños en la zona.
3. Que los equipos estén en condiciones visibles de operación.
4. Que las protecciones de seguridad estén colocadas.
5. Que existan los materiales necesarios para la producción.
6. Que el lote y producto correspondan a la orden de producción.
7. Que los registros del turno anterior hayan sido completados.

Cualquier anomalía debe comunicarse al supervisor antes de iniciar la operación.

---

## 6. Operación de la línea de embotellado

Durante la producción, el operario debe:

1. Controlar visualmente el funcionamiento de la línea.
2. Verificar que los envases ingresen correctamente.
3. Controlar que las botellas no presenten daños visibles.
4. Verificar el correcto llenado de los envases.
5. Controlar tapas, etiquetas y codificación.
6. Separar los productos que presenten defectos.
7. Registrar los controles establecidos en la hoja de producción.
8. Mantener limpia y ordenada el área de trabajo.

El operario **no debe modificar parámetros de la maquinaria** que no estén dentro de sus responsabilidades autorizadas.

Ante una falla que no pueda solucionar mediante el procedimiento establecido, debe detener la operación de manera segura y avisar al supervisor o al personal de mantenimiento.

---

## 7. Control de calidad

Durante el proceso deben realizarse los controles definidos para cada producto.

Entre otros aspectos, pueden verificarse:

* Nivel de llenado.
* Estado del envase.
* Colocación de la tapa.
* Integridad del sello.
* Posición de la etiqueta.
* Fecha y hora de producción.
* Código de lote.
* Apariencia general del producto.

Los productos que no cumplan los criterios establecidos deben colocarse en la zona identificada para producto no conforme.

**Nunca debe reincorporarse un producto rechazado a la línea sin autorización del área correspondiente.**

---

## 8. Seguridad durante la operación

Está prohibido:

* Introducir las manos en una máquina en funcionamiento.
* Retirar protecciones de seguridad.
* Anular sensores o dispositivos de seguridad.
* Realizar reparaciones sin autorización.
* Subirse a equipos o estructuras no diseñadas para ese fin.
* Correr dentro de la planta.

Si es necesario intervenir una máquina, debe seguirse el procedimiento de seguridad correspondiente y, cuando aplique, realizarse el aislamiento de las fuentes de energía antes de intervenir.

---

## 9. Atascos y fallas de la línea

Ante un atasco:

1. Mantener la calma.
2. Detener la línea utilizando el procedimiento establecido.
3. No introducir las manos mientras exista movimiento o energía peligrosa.
4. Informar al supervisor si la situación requiere intervención técnica.
5. Esperar la autorización correspondiente antes de reiniciar.

Nunca debe intentarse solucionar rápidamente un atasco ignorando las medidas de seguridad.

---

## 10. Limpieza y orden

El puesto debe mantenerse limpio durante toda la jornada.

El operario debe:

* Retirar residuos de manera periódica.
* Mantener despejadas las zonas de circulación.
* Limpiar los derrames inmediatamente siguiendo el procedimiento correspondiente.
* Depositar cada residuo en el recipiente indicado.
* Dejar el puesto limpio al finalizar el turno.

Los productos químicos de limpieza deben utilizarse únicamente de acuerdo con las instrucciones establecidas.

---

## 11. Gestión de residuos

Los residuos deben separarse según las categorías establecidas por la planta.

Ejemplos:

* Plástico.
* Cartón.
* Vidrio.
* Producto descartado.
* Residuos comunes.
* Residuos especiales.

Los residuos nunca deben acumularse en zonas de circulación o junto a los equipos de producción.

---

## 12. Trazabilidad y registros

El operario debe completar los registros correspondientes de manera:

* Clara.
* Legible.
* Completa.
* En el momento en que se realiza el control.

No está permitido completar registros basándose en suposiciones ni registrar controles que no hayan sido realizados.

Cualquier error en un registro debe corregirse siguiendo el procedimiento interno establecido.

---

## 13. Producto no conforme

Cuando se detecte un producto defectuoso:

1. Separarlo de la producción normal.
2. Identificarlo según el procedimiento establecido.
3. Informar al supervisor.
4. Registrar el incidente cuando corresponda.
5. No liberar ni reutilizar el producto sin autorización.

Los productos no conformes deben permanecer en la zona designada hasta que se determine su disposición.

---

## 14. Situaciones de emergencia

Ante una emergencia, el operario debe:

1. Detener la actividad de forma segura si es posible.
2. Informar inmediatamente al supervisor.
3. Seguir las instrucciones del personal responsable de la emergencia.
4. Utilizar las rutas de evacuación señalizadas.
5. Dirigirse al punto de encuentro establecido.

En caso de incendio, derrame químico, accidente laboral u otra emergencia, no debe intentarse resolver la situación por cuenta propia si no se cuenta con capacitación específica.

---

## 15. Comunicación de incidentes

Todo incidente, accidente o condición insegura debe ser comunicado inmediatamente.

Ejemplos:

* Derrames.
* Roturas de envases.
* Fallas de equipos.
* Protecciones de máquinas dañadas.
* Productos contaminados o sospechosos.
* Lesiones.
* Situaciones de riesgo.

Informar una condición insegura no constituye una falta: es una responsabilidad del trabajador.

---

## 16. Finalización del turno

Antes de retirarse, el operario debe:

1. Completar los registros correspondientes.
2. Informar cualquier problema pendiente al siguiente turno.
3. Dejar limpio y ordenado el puesto.
4. Retirar residuos según el procedimiento.
5. Dejar los materiales en las ubicaciones correspondientes.
6. Informar al supervisor cualquier anomalía detectada durante el turno.

---

## 17. Responsabilidades del operario

El operario es responsable de:

* Cumplir los procedimientos establecidos.
* Utilizar correctamente los EPP.
* Mantener la higiene personal.
* Cuidar los equipos y materiales.
* Registrar correctamente los controles.
* Informar anomalías e incidentes.
* Mantener el orden y la limpieza.
* No realizar tareas para las cuales no está autorizado o capacitado.

---

## 18. Regla fundamental

**Ante cualquier duda, detener la operación de manera segura y consultar al supervisor.**

La producción nunca debe realizarse ignorando una condición que pueda comprometer la seguridad de las personas, la calidad del producto o la integridad de los equipos.

---

### Confirmación del operario

Declaro haber recibido y comprendido las normas y procedimientos establecidos en este manual.

**Nombre y apellido:** ______________________________

**Fecha:** __________________

**Firma:** ______________________________

**Supervisor:** ______________________________

```

* Generamos Apps como estas
  * https://manual-minders.lovable.app/
  * https://bottler-pro-guide.lovable.app/cuestionario

<img width="617" height="365" alt="image" src="https://github.com/user-attachments/assets/d850fb67-8c64-46f2-b4ed-b208f6be9453" />

* Si quisier seguir trajando con mi aplicacion la puedo conectar con un excel, una base de datos, etc..
* Hay una amplia lista de conectores

<img width="409" height="197" alt="image" src="https://github.com/user-attachments/assets/7f1827cf-6b0b-46ec-a21a-331bad6dc3e0" />

> [!NOTE]
> Do o mas iteraciones probablemente nos exijan trabajar con la version paga

---

# Herramienta para transcripcion de Video y Reuniones

## Vos a Texto

* Para esto existen muchas aplicaciones
 * https://www.instagram.com/p/DBzb-kHxqae/?img_index=1

## Taqtic

* URL
  * https://tactiq.io/es

