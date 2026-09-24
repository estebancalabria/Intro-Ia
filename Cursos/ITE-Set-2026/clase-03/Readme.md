# Clase Tres - 24 de Septiembre 2026

# Repaso

* LLM
  * Guardrails / Jailbreak
  * Redes Neronals
  * Modelos chat / modelos de razonamiento
  * Propietarios
    * ChatGPT
      * Generalista
      * Generacion de texto humano
    * Gemini
      * Busqueda
      * Ecosistema de Google
      * Modo investigacion
    * Copilot
      * Pasarela a otros modelos
      * Empresarial
      * Control, etica, proteccion de datos
      * Ecosistema 364
    * Claude
      * Tecnico / Progrramacion
    * Grok
      * Irreverente / Grounding / Actualidad
    * Perplexity
      * Academico
  * OpenSource
    * Qwen
      * Generalista
    * Kimi
      * Tecnico / Progrramacion
    * Mistral
      * Europeo / GPRD
    * DeepSeek
      * Razonamiento
      * Noticia de trup y nvidia
     
----

# Ivestigacion de Gemini

* LA clase pasada nos quedo pendiente el informe de Gemini
    * https://share.gemini.google/WIV2Pd4ihVmU

 * Vamos a aprovechar el informe y mezclar algunas herramientas de IA (Modulo 4) para usar con el inofrmee

## Texto to Speech (Modulo 4)

* Herramienta
  * https://www.naturalreaders.com/

* A partir texto puedo hacer que la herramienta me lo lea en un segundo plano mientras voy en tren
* Para una version mas profesional el estandar del mercado
  * https://elevenlabs.io/

## Enriquecer un texto con Diagramas (Modulo 4)

* Herramienta
    * https://www.napkin.ai/es/
 
* Me permite enriquever un texto con diragramas como este....

<img width="438" height="369" alt="image" src="https://github.com/user-attachments/assets/886b7822-0205-4477-ab3a-f499e9900866" />

---
   
# Foto del estado de los LLM

* Como saber cuando sale un modelo nuevo
* Saber el listado de los modelos existentes
* Poder probar y compara un modelo con otro
* Poder dar nuestra opinion sobre que modelo me gusta y aporta mi granito de arena a la comunidad IA
* Elegir en un momento dado el modelo mas adecuado segun la taera

* URL
  * https://arena.ai/

* Primero vamos a hacer una experiencia ingresamos un prompt y lo responden dos modelo
* Con las votaciones de las personas va armando un raning
* Si quiero saber en algun momento determinado
    * Que modelos se estan usando
    * Cual es la percepcion de las personas sobre el raking
    * Que modelo elegir para una tarea determinada

---
# Break hasta y 10
---

# Como ejecutar un LLM localmente

## Donde se suben los modelos OS

* En HuggingFace (HF)
  * https://huggingface.co/
  * Una organizacion que nuclea todos los modelos OS (de todo tipo, no solo LLM) para democratizar el acceso a la IA
 
* En esta pagina vamos a encontrar
    * Modelos
      * Catalogo de modelos OS
    * Datasets
      * Datos usados para entrenar modelos
    * Spaces
      * Lugares para probar los modelos online antes de descargarlos
      * HF te da grauitamente cierta capacidad de computo diaria
      * Ejemplo : https://huggingface.co/spaces/black-forest-labs/FLUX.1-dev
     
> [!NOTE]
> Hay una veta bastante interesante en esto del OS donde muchas personas toman un modelo open source como el que esta en https://huggingface.co/spaces/jbilcke-hf/ai-comic-factory y genera una web independiente en la cual se descarga el modelo y cobra por su uso como es el caso de https://aicomicfactory.com/

 ---

 ## Como uso localmente un modelo Open Source

 * Para los LLM (Que son muy grandes) se suele utilizar
     * LMStudio
         * Es una aplicacion de escritorio facil de usar
         * Gratuita
         * DEscarga lo modelos desde HF
         * https://lmstudio.ai/
     * Ollama
         * Mas dificil, por linea de comando todo
         * https://ollama.com/
* Todo el resto de los modelos (Lenguaje, TTS, Imagenes, Video...)
    * Generalmente se ejecutan directamente programando en python

---
*  Entonces para manipular datos sensibles, usar LM Studio es recomendable?
    *  Si. (Por ejemplo si sos una aseguradora que usa la IA para generar contratos con los clientes con datos personales)


 ---
# Break hasta y 10
---

# Propmpt Engineering

* Como hablarle a la IA para obtener respuestas efectivas

* Arquitectura de un Prompt
    * Tarea
    * Contexto
        * Instrucciones Personalizada
        * System Prompt
        * Memoria
        * Herrammientas (Busqueda Web)
        * Convesacion
        * Conversaciones Pasadas
        * Personalizacion
        * Razonamiento
    * Persona / Rol
    * Ejemplo
    * Formato
    * Tono
  
* Tecnicas de prompting
  * Patrones probados para cada una de esas componente para mejorar la efectividad de la respuesta de la IA

---

## Tencica Persona / Rol

* Consiste en decirle a la Ia desde que lugar quiero que me responda, que rol quiero que asuma

* Experiencia. Abrimos 4 solapas de ChatGPT
  * Solapa 1 : Prompt sin un Rol, solo la tarea
    * "Elegime un coche electrico."
    * https://chatgpt.com/share/6ab5726c-18a0-83e9-9ccd-5bc53323aa21
  * Solapa 2 : Prompt preguntandole a un rol que me de la respuesta
    * "Actua como un experto en automoviles elecricos, econmia y sustentabilidad. Eligeme el mejor coche elecrico segun tu criterio"
    * https://chatgpt.com/share/6ab57279-ad2c-83e9-af42-3c0d5ba63b7d
  * Solapa 3 : Vamos a invitar a habalr del tema a una persona famosa (diverido)
    * "Eres Elon Musk. Recomiendame segun tu criterio el mejor coche electrico"
    * https://chatgpt.com/share/6ab57279-ad2c-83e9-af42-3c0d5ba63b7d
  * Solapa 4: Vamos a citar a un panel de expertos para tener distintas visiones de un tema (super util)
    * "Quiero elegir un auto elecrico. Quiero que me armes un panel de distintos expertos con distints percepciones donde cada uno me de en una oracion un resumen de que coche elegiria y porque"
    * https://chatgpt.com/share/6ab5728d-97bc-83e9-8cfc-bc323f97cc77

# PRoxima Clase

* Ver el repositorio del patron persona que hay
