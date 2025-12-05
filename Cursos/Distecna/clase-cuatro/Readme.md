# Clase Cuatro - 5 de Diciembre 2024

## Repaso

* Prompt Engineering
    * Patrones de Prompting
        * Rol
            * Panel de Expertos
        * Interaccion
        * Personalizacion de Salida
            * JSON
            * XML
            * HTML => Para exportar a PDf
            * CSV => Para exportar desde y hasta Excel
            * Markdown  => Para escribir plantillas y tener mayor control sobre salida
            * Mermaind  => Para Generar diagramas
                * Andaba muy bien con los artefactos de Claude
    * Conceptos
        * Contexto

# Recomendacion

* Crearse una cuenta de GMAIL alternativa para probar las herramientas que vemos en el curso que despues te mandan correos para novedad

# Large Language Models

* Propietarios
* Open Source
   * LLama
      * La que se puede usar desde el Wsap
   * Qwen
   * Deepseeek

* https://chat.groq.com/  << Motor de Inferencia

# Patrones de Prompting

- ## Extension Rol : Patron de Expertos

```
Quiero un panel de expertos de distintos roles para analizar la situacion de la argentina como posible
destino de inversiones. Generame un reporte para cada experto del panel y conpartime sus visiones con
informacion actualizada."
```

* Otro Ejemplo
```
Quiero un panel de expertos de distintos roles para analizar la situacion del conflicto en medio oriente. Generame un reporte para cada experto del panel y compartime sus visiones con informacion actualizada.
```

* Otro Ejemplo mas
```
Quiero un panel de expertos de distintos roles para analizar la situación del fútbol femenino en la argentina como posibilidad de invertir en la actividad. generame un reporte para cada experto del panel con sus visiones e información actualizada.
```

> Funciona muy bien con el modo pensado. (ex patron Chain of thoughts)

- ## Personalizacion de Salida

> Un lenguaje de programacion

# Programando con la IA (Vibe Coding)

- ## Mi primer Hola Mundo :)
  
* Ir a la pagina de Google Colab
   * https://colab.google/
* Elegir "Nuevo notebook"
* Escribir el primer hola mundo en una celda de
   * print("Hola mundo")

- ## Usando Mat Plot Lib

* MatPlotLib es una libreria de python que tien todos los graficos imaginables
   * Pagina Oficial : https://matplotlib.org/
   * Pagina de Ejemplos de Graficos : https://matplotlib.org/stable/gallery/index.html

* Pedirle a la IA que genere alguno de los graficos que este en esa pagina

```
Crearme un **stacked bar chart** en **matplotlib** que muestre un estimativo del pbi por anio de la argentina en los utimos 5 anios discriminando en la misma barra por colores menores de 30 y mayores de 30. (Es estimativo no tiene que ser real)
```

* Ir a Google Colab y En una celda ejecutar el codigo que me devolvio la IA

> Gemini Pro y ChatGPT (pago o lo gratuito con limite) pueden ejectuar codigo mostrarndo directamente el grafico sin necesidad de ir a colab

- ## Agentes

* Los modelos de lenguaje generalemten tienen 2 formas de uso distintas.La primera es el portal web que utilizamos todos los dias. La segunta es el potal para desarrollador que permite utilizar el modelo de lenguaje internamente desde una aplicacion. 

- ## Uso de la Api Key

* Ir a https://console.groq.com/home y sacar una api key

```python

api_key = input("Ingrese su Api Key")
prompt =  input("Ingrese su prompt")

from openai import OpenAI
import os
client = OpenAI(
    api_key=api_key,
    base_url="https://api.groq.com/openai/v1",
)

response = client.responses.create(
    input=prompt,
    model="openai/gpt-oss-20b",
)
print(response.output_text)

```

# Herrarmientas

- ## There is an AI for that

* https://theresanaiforthat.com/
* Entren periodicamente al Ledearboard

- ## Napkin

*  https://www.napkin.ai/
   *  Puntaje : 10/10 ( 28 algunos :) )

- ## Text-to-Speech 

* Natural Readers
   * https://www.naturalreaders.com/
      * Puntaje : 10 / 10


  

