# Clase Cuatro - 9 de Octubre 2025

# Repaso

* LLM
  * Lienzo/Canvas
  * Investigacion
* Prompt Engineering
  * Persona / Rol
  * Interaccion
  * Personalizacion
    * xml, json, html
    * markdown
    * mermaid/ dot <<<< Hoy seguimos con esto
    * Codigo
* Herramientas
  * Lmarena (lymsys arena)
  * Natural Readers
  * Extension de youtube
  * Transcripcion de reuniones : Taqtic

# Google Colab

Es un entorno / notebook para programr en python interactivamente

> https://colab.google/


# Graficar con IA nivel PRO (Patron personalizacion de Salida)

Una libreria de python para hacer graficos y diagramas es:
> https://matplotlib.org/

Para usarla voy a ir primero a chatGPT y pedirle que me genere un grafico utilizando esta libreria
```
Buscame el pbi de los 5 paises con mayor pbi de europa y generame el codigo en python para ejecutar en colab que muestre un grafico de barras donde se vea el pbi de esos paises
```

Luego chatgpt me genera el codigo en python que puedo ejecutar en una celda de google colab

```python
# Importar librerías necesarias
import matplotlib.pyplot as plt

# Datos de los países y sus respectivos PBI en billones de USD
paises = ['Alemania', 'Reino Unido', 'Francia', 'Italia', 'España']
pbi = [5.57, 4.96, 3.75, 2.78, 1.62]

# Crear el gráfico de barras
plt.figure(figsize=(10, 6))
plt.bar(paises, pbi, color=['#1f77b4', '#ff7f0e', '#2ca02c', '#d62728', '#9467bd'])

# Añadir título y etiquetas
plt.title('PBI Nominal de los 5 Países con Mayor PBI de Europa (2023)', fontsize=14)
plt.xlabel('Países', fontsize=12)
plt.ylabel('PBI en Billones de USD', fontsize=12)

# Mostrar el gráfico
plt.tight_layout()
plt.show()
```

Otro ejemplo
```
Haceme un grafico en matplot lib con los valores del Bitcoin en este ultiimo mes sacado de internet y una linea donde se vea la tendencia
```

> Para generar el siguiente codigo tuve que corregirlo con charGPT porque a la primera me dio un error

El codigo que me genero
```python
import matplotlib.pyplot as plt
import numpy as np
import pandas as pd
from sklearn.linear_model import LinearRegression

# Fechas del último mes
fechas = pd.date_range(start='2025-09-09', end='2025-10-09', freq='D')

# Precios de Bitcoin (31 valores, uno por cada fecha)
precios = [
    109707.14, 109778.50, 113330.17, 113541.09, 112000.00, 116000.00, 118000.00, 120000.00,
    122000.00, 121000.00, 121500.00, 122500.00, 123000.00, 124000.00, 125000.00, 124500.00,
    124000.00, 123500.00, 123000.00, 122500.00, 122000.00, 121500.00, 121000.00, 120500.00,
    120000.00, 119500.00, 119000.00, 118500.00, 118000.00, 117500.00, 117000.00
]

# Convertir fechas a números para la regresión
fechas_num = np.arange(len(fechas)).reshape(-1, 1)
precios = np.array(precios).reshape(-1, 1)

# Crear el modelo de regresión lineal
modelo = LinearRegression()
modelo.fit(fechas_num, precios)

# Predecir la línea de tendencia
tendencia = modelo.predict(fechas_num)

# Crear el gráfico
plt.figure(figsize=(10, 6))
plt.plot(fechas, precios, label='Precio de Bitcoin', color='tab:blue')
plt.plot(fechas, tendencia, label='Tendencia', color='tab:red', linestyle='--')
plt.title('Evolución del Precio de Bitcoin (Septiembre - Octubre 2025)', fontsize=14)
plt.xlabel('Fecha', fontsize=12)
plt.ylabel('Precio en USD', fontsize=12)
plt.xticks(rotation=45)
plt.legend()
plt.grid(True)
plt.tight_layout()
plt.show()

```
# Uso de API

* Usar la api de ChatGPT tiene costo, por lo que para el ejemplo vamos a utilizar un modelo Open Source ya que existe una web que nos deja utilizarlo gratis
* Todos los modelos de lenguaje tienen dos portales, uno para el desarrollador y otro para el usuario final.
* Para utilizar cualquier modelo o serivicio de IA como desarollador desde la pagina de desarrolador voy a obtener una api key
* Asociada a esa api key te debitan la facturacion
* El pago para usar la api no siempre es el mismo que por ejemplo cuando contratas el pro

* ChatGPT
    * Usuario Final : https://chatgpt.com/
    * Desarrollador : https://platform.openai.com/docs/overview
* Grok
    * Portal para usuario Final : https://groq.com/

# Herramientas

## Napkin AI

Herramienta para enriquecen texto con diagramas

> https://www.napkin.ai/

Puntaje : 10 / 10

## There is a ai for that

## NotebookLM

# Open Source vs Propietario

PAra ejecutar y probar modelos de lenguaje (LLM) open source la mejor web es 

> https://groq.com/

Groq es una empresa que no entrena sus propios modelos de IA sino que descarga modelos open source y los brindan para que los usuarios finales los utilicen

