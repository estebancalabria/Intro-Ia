# Clase Tres - 20 de Marzo del 2026

# Repaso

* LLM
  * Propietarios
    * ChatGPT
    * Gemini
    * Claude
    * Grok
    * Perplexity
  * Open Source
    * Chinos
        * DeepSeeK (DeepThinking / Pensamiento Profundo)
        * Qwen
    * Americanos
        * Familia Meta
    * Otros
        * Mistral (https://mistral.ai/ - https://chat.mistral.ai/chat)
            * "Francia Segundo"
* Herramientas
  * NaturalReaders

# Large language Models

* Open Source
    * Groq (No confundir con el de Elon Musk) : El es Motor de inferencia mas rapido gracias a su arquitectura (LPU) para ejecutar online modelos Open Source

## Curiosidades

* GPT "Zurdo" : https://chatpts.laizquierdadiario.com/

## Hugging Face

> https://huggingface.co/

* Plataforma/Repositorio donde se suben todos los Modelos Open Source
* El github de los modelos de IA Open Source
* Ideal para pasarse probando y curioseando modelos OS.
* Lo mas importante de esta pagina esta aca en los spaces
  * https://huggingface.co/spaces

## LMArena

> https://arena.ai/

* Para probarlo utilizamos este prompt : "Tengo el lavadero e auto a una cuadra. Quiero saber si me recomendas ir caminando o en auto?"
* LA gente vota y ahi arma un ranking para determinar que modelo es mejor

## LMStudio

> https://lmstudio.ai/

* Te permite descargar los modelos OS de Huggign Face para ejecturarlos localmentes (Siempre que tengamos una buena pc)
* Hay otras alternativas como Ollama

# Prompt Engineering

## Un buen prompt

* Buen prompt = Tarea + Contexto + Ejemplos + Persona/Rol + Fomato + Tono
* Para patron o tecnica de prompting se focaliza en alguno de esos puntos

## Patrones de Prompting : Rol/Persona

* Vamos a tomar un prompt y probarlo con distintos formas
    * Sin especificar un Rol
        * "Dame ideas de destinos en el mundo para visitar"
    * Especicando un rol especifico
        * "Actua como un experto en organizacion de viajes coorporativos para empresas donde las empresas me contratan para organizar sus viajes, experto en turismo, cultura organizacional, incentivo organizacional (para organizar sus viajes de incentivo).  Dame ideas de destinos en el mundo para visitar"
    * Como si fuera una persona conocida
        * Actua como "Luisito comunica". Dame ideas de destinos en el mundo para visitar.
    * Citar un panel de expertos (distintos roles)
        * Quiero que conformes un panel de expertos con distitnos roles para organizacion de viajes coorporativo. Cada rol me tiene que dar una lista de destinos distinta recomendada desde su perspectiva y una oracion corta de porque elije ese destino.

## Patrones de Prompting : Interaccion (Contexto)

* Consiste en pedirle a la IA que me haga preguntas para armar el contexto correcto y que me una respuesta optima para mi caso.

```
Soy el encargado de organizar un viaje cooportativo para una empresa y quiero que me recomiendes la mejor opcion y porque.
Antes de recomendarme una opcion quiero que hagas preguntas DE A UNA para tener toda la informacion necesaria para tomar una mejor decision.
Debes consultarme sobre todos los aspectos que se te ourran sobre la organizacion del viaje y recien cuando tengas toda la informacion dame una recomendacion.
No te apures a darme una recomendacion sin antes recopilar toda la informacion necesario.
Busca antes informacion geopolitica global y tene en cuenta la situacion mundial para hacer la recomencacion.
Que las preguntas sean para respuestas cortas o multiple choice.
```
* Aca lo importante es PEDIR las pregutnas DE A UNA.

* Ejemplo anterior:
> https://chatgpt.com/share/69bd43a2-7b98-8005-8cba-6c642bb55f15


# Glorsario

* Prompt : Las Intrucciones
* Contexto : Toda la informacion provista por el usuario que dispone el LLM para darnos una respuesta tanto en el prompt como en toda la conversacion
      * Ademas LLM con ChatGPT utilizan memoria y chats anteriores como contexto
* La IA no es deterministica : Un mismo prompt no siempre no da la misma respuesta
