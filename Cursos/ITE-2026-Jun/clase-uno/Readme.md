# Clase Uno - 24 de Junio del 2026

# Roadmap 

* Large language Models (LLM)
  * Funcionamiento de los LLM
  * Distintos modelos y para que destaca cada uno
  * Tipos de Modelos
    * Propietarios
    * Open Source
      * Util para privacidad de datos
  * Agentes
* Prompt Engineering
  * Tecnicas para hablarle a la IA para obtener respuestas mas efectivas
  * Como arma la respuesta la IA
  * Vibe Coding
* Herrmientas de IA
  * Herramientas de IA para la productividad
  * Voz a texto y texto a voz
      * Transcripcion de reuniones online
  * IA en la oficina
  * Presentacion con IA
  * Videos Institucionales
  * Automatizacion con IA (N8n, make)
* IA Generativa Multimedia/Creativa
  * Generacion de Imagenes
  * Generacion de Videos
  * Generacion de Canciones/Audio
* IA Tradicional y Etica
  * Mechine Learning
  * IA para toma de decisiones basado en datos
  * Uso responsable de la IA
  * Riegos de la IA
* Ai-900
  * Azure
  * Servicios para desarrollar tus propias soluciones de IA
    
---

# Informacion de Contacto

* Mct Esteban Calabria.
* Me puden contactar en:
  * https://www.instagram.com/mct.esteban.calabria/
  * https://www.linkedin.com/in/esteban-calabria-7a44401a/

--- 
# Large language Models (LLM)

## Distintos LLM

* Propietarios
  * ChatGPT
  * Copilot (Licencia)
    * Domestico : https://copilot.microsoft.com/
    * Corporativo : https://www.office.com/ (Requiere licencia)
  * Gemini

## Entrenamiento y fundamentos

* Dataset Enorme con toda la Informacion de Internet de texto
* Entrenamiento de una red neuronal de arquitectura trasnformer con ese data set
  * Requiere enorme capacidad de computo
* Ese modelo predice que proximo Token

* Paso 1
  * "Hola que" -> Modelo -> "Tal"
  * "Hola qu tal"
* Paso 3
  * "Hola qu tal" -> Modelo -> "Como"
  * "Hola que tal. Como"
* Paso 4
  * "Hola que tal. Como" -> Modelo -> "estas?"
  * "Hola que tal. Como estas?"


## ChatGPT

* URL
  * https://chatgpt.com/
* Empresa
  * OpenAI
* Caracteristicas
  * Emular conversaciones humanas

## Caractisticas : Memoria

* A ChatGPT
```
Con la informacion que tenes de mi, haceme un roast, una gastada.
```

* A Copilt  (Como tiene guardrails si le pido el roast no me lo hace porque es mas para uso corporativo)

```
Haceme un resumen de lo que sepas de mi tipo perfil del FBI
```

* Usuario---> Personalizaion ---> Memoria
 * Podes ver lo que ChatGPT recuerda de uno
 * Pedirle que olvide lo que no queres que recuerde
 * Y en un chat podes pedirle explicitamente que recuerde algo

> [!NOTE]
> Copilot tambien tiene el tema de la memoria (tambien gemini)

## Caractisticas : Instrucctiones Personalizadas

* En chatGPT
  * Personalizacion -> Instruccioens personalizadas

* Le vamos a poner esta instruccion personalizada

```
Quiero que me respondas en poema. Todo lo que tenes que responder tiene que estar en verso. Todo con rima. 
Que tu respuesta sea una poesia, llena de metaforas. Una obra de arte literaria.
```

* Le pido algo a ChatGPT y veo como me responde en poema

> [!NOTE]
> Copilot y Gemini tambien lo tieen.

* Algunas instrucciones personalizadas que me resultaron de utilidad
  * https://github.com/estebancalabria/Intro-Ia/tree/main/Large%20Language%20Models/ChatGPT/instrucciones-personalizadas

## Caractisticas : Uso de herramientas y busqueda web

* Al principio ChatGPT te respondia hasta una fecha determinada
* Hoy en dia los modelos de lenguaje tienen la capacidad de hacer busquedas web y generar respuespuestas ancladas (grounding) en lo que buscaros

> [!NOTE]
> TIP : Es importarte saber si la respuesta de la IA la baso solamente en su conocimiento o si utilizo la herrmienta de busqueda web para usar esa informacion como contexto para darme una respuesta basada no solamente en su conocimiento sino tambien en informacion actualizada


---

# Glosario

## Alucinacion

* Cuando la IA responde informacion incorrecta o inventada sin saber y actua como si eso fuera cierto.
* O cuando responde cualquier cosa no relacionado con el prompt

## Prompt 

* La instruccion que uno escribe a la IA para que complete una respuesta

## System Prompt

* Es una instruccion oculta que definio el fabricante del LLM para determinar la forma en la que tiene que responder, el tono que usa por defecto y su personalidad.
* Supuesto repositorio donde se guardan los "leaks" (filtraciones) de los system prompts
  * https://github.com/asgeirtj/system_prompts_leaks

## Token

* Es una palabra o parte de la misma como subdivision de un texto. Es la unidad minima que utiliza la IA.
* Ejemplo de tokenizador
  * https://platform.openai.com/tokenizer

## Grounding

* Anclar la respuesta de la IA en informacion verificable
* Anecota:
  * Un abogado que uso ChatGPT y genereo un alegado impecablente redactado pero la IA inveto toda la jurisprudencia
    * https://www.infobae.com/colombia/2026/06/09/consejo-de-estado-fijo-reglas-para-usar-la-inteligencia-artificial-en-la-justicia-tras-caso-de-abogado-que-habria-inventado-sentencias-con-chatgpt/
   

## Multimodal

* Capacidad de procesar texto, imagenes, pdfs.. 
