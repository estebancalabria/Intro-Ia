# Clase Cuatro - 1 de Julio de 2026

# Repaso 

* Large Language Models
  * Propietarios
    * Grok
  * Open Source
    * Modelos
      * Mistral
    * Ejecutar Modelos Offline
      * LMStudio
      * Ollama
    * Hugging Face
      * Repositorio de Modelos Open Source
      * Spaces
        * https://huggingface.co/spaces
        * Me permiten probar modelos OS gratuitamente
  * Comparativa de modelos con Arena
* Herramientas
  * Texto-A-Voz
    * Natural Readers
  * Generacion de Imagenes
    * Napkin
* Prompt Engenieering
  * Prompt = Tarea + Contexto + Ejemplo + Rol + Formato + Tono
  * Tecnicas de Prompting
  * Contexto
    * Patron Interaccion
    * Rol

---
---

# Noticias

* En la web esta esta pagina
  * https://aicomicfactory.com/
  * Te cobra 10 dolares por mes por utilizar un modelo de IA que genera comics
* Pero si nos fijamos en HF tenemos este space
  * https://huggingface.co/spaces/jbilcke-hf/ai-comic-factory
 
> [!NOTE]
> Lo que hicieron la pagina simplemente tomaron un modelo OS y construyeron una web alrededeor y te cobran por usarlo
> Hay muchas oportunidades comerciales alrededor de los modelos de IA OS

---
---

# Herramientas de IA

## Directorio de Herramientas e IA

* There is an AI for That
* URL
  * https://theresanaiforthat.com/
* Evolucion de Herramientas de IA
  * https://theresanaiforthat.com/period/2015/
    * 6 Herramientas
  * https://theresanaiforthat.com/period/2016/
    * 16 Herrmientas
  * https://theresanaiforthat.com/period/2017/
    * 30+ herramientas
  * ...
  * https://theresanaiforthat.com/period/2016/
    * 2000+ herramientas

## Desarrollo de Herramientas de IA

> [!NOTE]
> Muchas de las herramientas de IA son simplemente Interfaces sobre modelos de de IA tanto open source como propietarios por medio de API Key

* Fromas de Interactiar con la IA
  * Modelo Propietario
      * Portal web
        * Ej : https://chatgpt.com/
      * Api Key
        * Portal para el desarrollador con la documentacion, la parte facturacion y donde generamos una api key
            * Portal Principal : https://platform.openai.com/
            * Sacar Api Key : https://platform.openai.com/api-keys
            * Documentacion: https://developers.openai.com/api/docs
        * El uso de las API KEY es pago (aunque es infimo)
  * Modelo Open Source
      * Potales web de motores de Inferencia que me permiten usarlo
          * Ejemplo
            * https://groq.com/
            * https://chat.groq.com/
        * Api Key de Motor de Inferencio
            * https://console.groq.com/home
            * Se pueden usar las API key en forma gratuita con un limite bastante holgado
        * Descargar el modelo y usarlo localmente
            * Se descargan de HF
            * Suelen tener ciertos requerimientos minimos de hardware para utilizar el modelo

> [!NOTE]
> El creador de una herrmienta de IA (o el que va a desarrollar una automatizacion con IA) va obtener una API Key para utilizar un LLM desde su programa/codigo en lugar de hacerlo mediante el portal web tradicional que usa el usuario final

### Ejemplo de uso de API Key

* Sacar una api key de Groq (con q)
  * Ir a la web
    * https://console.groq.com/keys
  * Crear una api key
  * Guardarla en un lugar seguro
* Ver la documentacion de uso de la api key (En una solapa nueva)
    * https://console.groq.com/docs/overview
* Ir a google colab y oguearse
  * https://developers.google.com/colab
* Generar un notebook/cuaderno (entorno de programacion) nuevo
  * Open Colab...nuevo Cuaderno
* Copiar el codigo de uso de api key de la web de documentacion de Groq a la primer celda de codigo del colab

```python
from openai import OpenAI
import os
client = OpenAI(
    api_key=os.environ.get("GROQ_API_KEY"),
    base_url="https://api.groq.com/openai/v1",
)

response = client.responses.create(
    input="Explain the importance of fast language models",
    model="openai/gpt-oss-20b",
)
print(response.output_text)

```

* Modifcar el codigo

```python

from openai import OpenAI
import os

api_key = input("Ingrese su API Key:")
prompt =  input("Ingrese su prompt:")

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

* Ejecutar el codigo

---
---

# Large Laguage Models

## Propietarios

### Perplexity

* El modelo ideal para trabajos academicos por el grounding
* URL
  * https://www.perplexity.ai/
* Caracteristicas
  * Su modelo propietario se llama sonar pero puede usar GTP, Gemini o Claude
  * Lo relevante de perplexity es su enfoque academico hacia el grounding

* Lo probe con este prompt activando en el + solamente las fuentes academicas
```
Quiero que me investigues atualizaciones yestado del arte en materia de quimcos relacionados con pinturas. Ver ultimas investigaciones, novedades y referencias
```

* Cada parrafo tiene una cita academica con el grounding
---

## Open Source

### Groq

* Motor de inferencia que permite ejecutar modelos OS online
* Se caracteriza por su velocidad
  * URLs
    * https://groq.com/
    * https://chat.groq.com/

---

# Prompt Engenieering

# Formato + Tono

* Pedimos una lista de algo sin formato
 * Dame una lista de las 10 series mas populares de los utimos tiempos. Quiiero el nombre, cantidad de temporadas, fecha de lanzamiento, monto estimado recaudado, putnaje en imdb promedio, creador, actor principal (uno), argumento en una oracion

## Formatos tecnicos

* Casos de uso
  * Esto se usan mucho cuando usamos api key
  * Formatos usados por desarrollados
  * Para documentacion tecnica
* Ejemplos
  * JSON
     * Dame la lista en json
  * XML
     * Dame la lista en cml
 
## Fomato PseudoTecnico (HTML)

* Caso de uso
  * Generacion de pdf con formato
* Problema
 * Si le pido a ChatGPT que genere un pdf lo hace pero con un formato que deja mucho que desear
   * No es muy profesional como para mandarlo a un cliente, jefe, etc en cuanto a su presentacion
* Solucion
  * Pedirle a ChatGPT que me presente la informacion como una unica pagina html profesional que luego descargo, abro con el navegador e imprimo como pdf

```
Generame la lista de series en una unica pagina html que se vea profesional, elegante  con toda la informacion de cada serie que vimos y sea adecuada para presentar profesionalmente a un jefe, cliente, etc. Que sea un disenio moderno. 
```

## Formato tipo Tabla (CSV)

* Casos de USo
  * Para generar archivos que se puedan importar en una planilla de calculo como Excel o Google Sheets
* Formato
  * CSV (comma separated Values)
* Prompt
 * "Dame la lista como un CSV"

> [!NOTE]
> Ese archivo CSV se puede abrir direcgamente con Excel o se puede importar en Google Sheet

## Personalizacion de Salida con Markdown

* Caso de uso
  * Reducir el no determinismo de la IA especificando una plantilla exacta de como quiero la respuesta
* formato
  * Markdown
