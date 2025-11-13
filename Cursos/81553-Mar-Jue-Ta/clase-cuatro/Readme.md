# Clase Cuatro - 13 de Noviembre de 2025

---

# Repaso

* Prompt Engineering
  * Rol
    * Patron Persona / Rol
  * Contexto
    * Patron de Interaccion
  * Salida
    * Personalizacion de Salida
      * Formatos Tecnicos
        * JSON
        * XML
        * HTML (Util para generar PDFS)
        * CSV
      * Markdown
      * Graficos
        * Mermaid
        * Python : MatPlotLib (Todos los graficos que se te ocurran)
  * Tips
    * Responder solo lo solicitado para copiar y pegar
    * Ofrecer Recompensas

* Instrucciones Personalizadas
  * Google Gems
  * Anything LLM (Tambien permtie instrucciones personalizadas)
  * Personalizacion de ChatGPT

# Herramientas de IA

## Text-to-Speech (Texto a voz)

- ### Natural Readers

> https://www.naturalreaders.com/
* Puntaje : 9 / 10
    * No te deja bajar el mp3 salvo que lo piratees
  
## Speech-To-Text (Voz o Video a Texto)

- ### Unlimited Summary Generator for YouTube™

> https://chromewebstore.google.com/detail/unlimited-summary-generat/eelolnalmpdjemddgmpnmobdhnglfpje
* Puntaje : 9 / 10

- ### NoteGPT
> https://notegpt.io/

- ### Herrmientas para transcribir reuniones o videos

> https://www.instagram.com/p/DBzb-kHxqae/?img_index=1

- ### Taqtic

> https://tactiq.io/es
* Puntaje : 8.5 / 10

## Generacion de Diagramas

- ### Napkin
  
> https://www.napkin.ai/
* Puntaje : 10 / 10

- ### XMind (Sugerencia de un alumno

> https://xmind.com/

## Clonar Voces

> https://elevenlabs.io/

## Compendio de herramientas de IA 

> https://theresanaiforthat.com/

# Uso de la API

Cada vez hay mas herramietnas de IA.
Los proveedores de los modelos de ia generalmente tienen dos web
* Una para el usuario final
    * https://chatgpt.com/
    * https://chat.groq.com/
* Una para el desarrollasor 
    * https://platform.openai.com/
    * https://console.groq.com/home
 

- ## Pasos para usar la APi con GROQ

1. Ir al portal de desarrollador de Groq https://console.groq.com/home
2. Generar una Api Key y guardarla en un lugar seguro
3. Ir colab.google.com y generar un script de python

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

4. Ejecutar
