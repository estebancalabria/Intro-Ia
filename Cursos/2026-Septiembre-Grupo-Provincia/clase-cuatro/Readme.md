# Clase Cuatro - 13 de Octubre del 2026

# Repaso

* Ecosistena Copilot
  * Integracion con 365
    * Calendario
  * Enfique de IA responsable de Microsoft
    * Confidencialidad
    * Acuerdo empresarial
  * Office
    * Copilot en PowerPoint
  * Copilot para 365
    * Personalizacion
    * Biblioteca de Prompts
    * Cuadernos (simil NotebookLM)
    * Biblioteca Creativa
    * Memoria
 
---

# Microsoft

* 365
* Power Platform
  * PowerBI

---

# Analisis de Informacion

* El chatbot convencional no suele procesar todas las filas del Excel ni es confiable para calculos matematicos
* En ese caso vamos a usar el copilot para excel o el agente analista

## Copilot para Excel

* Vamos a crear un documento de Ejemplo
  * Nombre
  * Documento
  * Provincia
  * Tipo de Seguro
  * Monto

### Pivot Charts

```
Armame un grafico dinamico (pivot graph) en otro libro para poder discriminar y agrupar montos por provincia o Tipo de Seguro
```

* En excel puedo armar los siguientes graficos:
    * https://support.microsoft.com/en-us/excel/available-chart-types-in-office

```
Me podes armar en otro libro dos graficos de pie que muestren agrupado el monto un grafico por provicia y otro por tipo de seguro
```

### Tabla Dinaminca

```
Quiero una tabla nueva donde se muestre la cantidad de asegurados por tipo de seguro, el monto total de asgurados por tipo de seguros. Y otra tabla donde se vea la cantidad de asegurados por provincia y el monto total asegurado por provincia. La quiero en un libro nuevo.
```

* Me ahorro tener que conocer las formulas

## Agente Analista

* Traicionalmente
    * (prompt) -> (llm + herramienta) -> (respuesta)
      
* Agente analista
    * (prompt) + (fuente de datos, xls, csv) -> (llm + herramienta) -> (codigo en python) -> (interprete de codigo) -> (llm) -> (respueta)


* Prueba previa

```
Podes generar un codigo que cosulte las bases de datos del SSN (superintendencia de seguros de la nacion) y me realice algun informa sumarizador
```
> No lo pudo hacer

* Vamos a analizar los datos de un archivo excel
    * Regresion (predecir valores futuros)
    * Clasificacion
    * Analisis de Anomalias
    * Graficos y analisis

```
Dame las tres provincias con mas monto asegurado
```


## Agente Investigador

```
Quiero una investigacion sobre las disintas companias de seguro en argentina, los tipos de seguro que ofrecen, el porcentaje de mercado que manejan y el monto aproximado que operan. Buscar informacion con fuentes y  generar estimados.
```

* A diferencia de Gemini se centra mas en fuentes corporativas


* Puedo utilizar el agente analista en conjunto con un copilot sin agente
    * Al primero primero le pregunto "Dame una lista de 5 KPI que puedo determinar con estos datos"
        * Esto lo puede calcular viendo solo los titulos de las columnas, no necesito ejecutar mucho codigo

* Me armo este prompt para el agente analista

```
Actuá como analista de datos especializado en seguros.

Analizá el archivo de Excel adjunto utilizando el intérprete de código. Inspeccioná automáticamente la estructura de los datos, identificá las columnas disponibles y calculá los KPI más relevantes que puedan obtenerse a partir de la información existente.

Como mínimo, evaluá:

1. Cantidad total de asegurados.
2. Monto total asegurado.
3. Monto promedio asegurado por cliente.
4. Distribución de asegurados por tipo de seguro.
5. Distribución de montos por tipo de seguro.
6. Distribución de asegurados por provincia.
7. Distribución de montos por provincia.
8. Tipo de seguro con mayor y menor participación.
9. Provincia con mayor y menor monto asegurado.
10. Ranking Top 10 provincias por monto asegurado.

Además:

- Identificá patrones, concentraciones y posibles hallazgos de negocio.
- Indicá cuáles son los productos más relevantes para la cartera.
- Detectá posibles valores atípicos (montos inusualmente altos o bajos).
- Calculá cualquier KPI adicional que consideres útil según las columnas disponibles.
- Generá tablas resumen.
- Generá gráficos cuando aporten valor al análisis.
- Incluí una sección final llamada "Conclusiones ejecutivas" con los principales insights encontrados.

Mostrá los cálculos realizados y los resultados numéricos obtenidos.
```

## OTros agentes

* Prompt Coach
* ...
* Mirar la lista de agentes que vienen con 365


## Agentes Personalizados

* Copilot 365 te da la posibilidad de crear tu propio agente
  * Directamente desde la interfaz de 365
  * Dentro de Power Platform con Copilot Studio
      * https://copilotstudio.microsoft.com/
      * Estan pensados tambien para que los utilicen gente de afuera de la compania (ej chatbot de atencion al cliente)
* Que es un agente
    * (llm) + system prompt + (Fuentes de Informacion fijas) + herramientas
 
* 
