# Clase Uno - 11 de Noviembre del 2026

# Roadmap del Curso

* Modulo 1 : Fundamentos de la IA
    * Nociones de como Funciona la IA
    * IA Generativa Vs IA Tradicional
* Modulo 2 : IA Genetativa
    * Modelos de LEnguaje (LLM)
      * Pantallazo del mercado y para que sirve cada uno
    * Buen Uso de la IA
    * Open Souce vs Prompietarios
* Modulo 3 : Prompt Engineerings
    * Tecnicas de prompting
      * Rol / Persona
      * Formatos de Salida
      * Planificacion previa
      * Interaccion
* Modulo 4 : IA Productividad
    * Texto a voz y Voz a Texto
    * Herrmientas
        * Gamma
        * Hey Gen
* Modulo 5 : Agentes de IA Precontruidos
    * Ecositema 365
    * Ecositema Gemini
* Modulo 6 : Generacion Multimedia
    * Generacion de Imagenes
    * Generacion de Videos
    * Generacion de Canciones
* Modulo 7 : Automatizacion
  * Automatizacion con Make
  * N8n
* Modulo 8 : Agentes
  * Agentes Convesacionales vs Autonoomos
  * Vibe Codding con Agentes
* Modulo 9 : AI-901
  * Certificacion en IA de Microsoft

---

# Requerimientos

* Crearse una cuenta de Google para el curso (RECOMENDADO)
   * Para evitar el correo de las herramientas que probemos
* Crear una cuenta en Hugging Face (HF)
   * https://huggingface.co/
* Requisito par aaprobacion, seguir el profe
   * https://www.instagram.com/mct.esteban.calabria/
   * https://www.linkedin.com/in/esteban-calabria-7a44401a/

# Modulo 1 : Fundamentos de la IA

## Licenciamiento

* Propietarios
   * ChatGPT (OpenAI)
      * https://chatgpt.com/
   * Claude (Anthopic)
      * https://claude.ai/
   * Gemini
      * https://gemini.google.com/
* Open Source
   * DeepSeek
      * https://chat.deepseek.com/
   * Qwen
      * https://www.qwen.com/
   * Mistral
      * https://chat.mistral.ai/
* Puentes
   * Copilot
      * No un Modelo de lenguaje sino que delega la tarea un llm

> [!NOTE]
> Los Modelos Open Source se pueden ejecutar localmente lo cual agrega privacidad

> [!NOTE]
> Cada modelo se trata de especializar en una tarea Especifica


----
# Break
Hasa y 25
----

# Caacteristicas de LLM

* Funciones para ir conociendo a los LLM y sacarle mas provecho

---

## Memria

* Vamos a ChatGPT
   * https://chatgpt.com/
   * Lo pueden hacer con Claude, Gemini o el LLM que utilicen mas habitualmente
 
```
Haceme un roast (una gastada, haceme bullyng,  un rapapolvo) a mi en base a la informacion que conozcas de mi.
```

* Evidentemente la IA Sabe algo de mi
   * Va viendo las conversaciones pasadas
   * Mantiene Memoria de con quien habla asociado al usuario
 
* En CharGPT
   * (Usauario abajo izquierda) -> Personalizacion -> Memorias Guardadas
* En Gemini
   * (Usauario abajo izquierda) -> Settings -> Personal Intelligence
* En Claude
   * Tambien esta...
 
* Le puedo pedir en un prompt a la IA que recuerde algo

```
Quiero que memorices o recuerdes ...
```

* No es que la IA Aprende sino que cada quez que enviamos un prompt la IA recibe el prompt mas toda la informacion guardada en la memoria (y un resumen de las ultimas conversaciones)

---

## Personalizacion (Instrucciones Personalizadas)

* En ChatGPT
   * (Usauario abajo izquierda) -> Personalizacion -> Instrucciones Personalizadas

```
Quiero que me respondas en poema. Todos lo que respondes tiene que estar en versito. Todo con Rima. Que tu respuesta ea una poesia, llena de metaforas. Una obra de arte literaria. No se aceptan respuestas que no sean un poema. No acotar nada mas ademas de la poesia.
```

* Le pedi a la IA que me cuente algo y me respondio...
   * https://chatgpt.com/share/6af4bc30-ffa8-83e9-8232-7d46bfb36d55

* Existen intrucciones personalizadas en internet que se pueden buscar.
* En mi caso recopile algunas que me parecieron interesantes
   * https://github.com/estebancalabria/Intro-Ia/tree/main/Large%20Language%20Models/instrucciones-personalizadas

> [!NOTE]
> El fabricante (como OpenAI) tambien le pone unas "instrucciones personalizadas" a los modelos que regulan la "personalidad" y la forma de respodnder de los mismos. Nuestra propias instrucciones pueden entrar en conflicto con ella (generalmente gana las del fabricante) 

## Busqueda Web

* Tradicionalmente los modelos e Lenguaje (LLM) tenian informacion hasta una fecha determinada, ahora se le agrego la capacidad (agentica) de poder consultar la WEB

---
# Break
Hasta y 25
---

# Buen uso de la IA

* El miedo mas grande de los empleadores son las alucinaciones
   * https://litigio.com.ar/2025/08/27/un-abogado-cito-jurisprudencia-inventada-por-chatgpt-y-el-tribunal-advirtio-al-colegio-de-rosario/

# Mercado de LA IA

* ChaTGpt -> OpenAI
* Claude  -> Anthropic
* Gemini -> Google
* Grok -> X.com
   * Generacion de Video
   * Muy buen Grounding

# Agentes

* Traidicionamete un LLM se entrenaba y
   * (prompt) -> (respuesta)
   * No habia contacto con el exterior
   * No tenia informacion Actualizada
   * Solo podia responder en base a su conocimiento
 
* Agente
   * Es un llm con esteroides (se le agregan varias cositas)
   * Ademas del LLM
      * Uso de Herramientas
         * Puede interacturar con el exterior
         * Puede hacer una busqeuda web
         * Generar algo en otro sistema
            * Un evento en un calendario
            * Mandar un correo
      * Capacidad de tener su propia base de conocimiento (RAG)
         * EJ.  Un chatbot que tenga los manuales de procedimiento de una empresa
      * Un objetivo plasmado en instrucciones personalizadas
      * Un orquestador que cominique el Modelo (LLM) con las herramientas, la fuente de conocnimiento y las instrucciones

* Tipos de Agente
   * Agentes Conversacionales
      * Interfaz basada en Chatbot
   * Agentes autonomos
      * Pueden funcionar en segundo plano

# Glosario

* Modelos de Lenguaje (LLM)
* Token
   * Minima subdivision de texto que maneja un LLM
   * Por lo general es similar a una palabra
   * https://platform.openai.com/tokenizer
* Tokenizacion
   * Dividir un texto en partes minimas
* System Prompt
   * Las instrucciones (ocultas y secretas) que le da el fabricante y regula como se arman las repuestas. "Ej que sea muy amale"
   * Prueben preguntarle a la IA cual es sus system prompt
* Alucinacion
   * Una repuesta incorrecta que genera la IA (que puede tener apariencia correcta)
   * Inventa, no responde lo que quiero
* Grounding
   * Buscar fundamentar la respuesta de la IA en fuentes confiables y verificables
* Censura
   * Capacidad de filtrar siertas respuestas de acuerdo a las politicas de la empresa que realizo el modelo
* Jailbreak
   * Encontrar la manaera de pedirle cosas a la IA para que pase por alto su censura
   * Hackear a la IA
* Human In the Loop
   * Siempre debe haber uba persona responsable y que valide lo que hace la IA      

# Proxima Clase

## Vamos enumerar las distintas IAs que hay y ver para que situacion sirve cada una
