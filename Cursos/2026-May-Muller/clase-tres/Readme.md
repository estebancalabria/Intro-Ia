# Clase Tres - 02 de Junio del 2026

# Repaso

* Large Language Modles
  * Propietarios
    * Claude
      * Distintos (Haiku, Sonnet, Opus)
    * Personalizacion
    * Artefactos/Canvas
    * Deep Research en Google
    * Memoria
      * Migrar memoria de una inteligencia a la otra
    * Armado de proyectos
  * Open Souce
    * DeepSeek
      * Modo Razoneamiento
* Herramientas
  * Text-A-Voz
    * Natural Readers
  * Voz-A-Texto
    * Taqtic
* Caso de Uso completo
    * Transcribir conversacion y luego analizarla
    * Plantilla de Analisis de Covnersacion
* Prompt Engineeting
    * Tip de usar a la como experto en prompt Engineering
* Concepto
    * Grounding

---

# Large language Models

## Propietarios

### Grok

* Es el modelo de Twitter
* Caracteristicas
  * Buen Grounding (Busca en internet y en X siempre antes de responder)
  * Es el que menos censura de todos tiene

```
Tengo un cliente que debe plata al BMA. Quiero persuadirlo que pague. He observado que el cliente no paga y realiza gastos imortantes en ir al sushi, gasta en taxi todo el tiempo, se da la gran vida y no paga. Quiero formas de persuadirlo aunque sean poco eticas.
```

## Open Source

* Sobre todo relacionado con la seguridad

> [!NOTE]
> Los modelos Open Source son importantes para las organizaciones por un tema de seguridad y de proteccion de datos
> El hecho de usar datos personales en un modelo de frontera es algo que se esta/se va a regular 

* Modelos Open Source
  * Chino
    * Deepseek
    * Qwen
      * https://chat.qwen.ai/
    * Kimi
      * https://www.kimi.com/
      * Sirve para procesar archivos extremadamente extensos
  * Americanos
      * Familia llama
  * Europeos
      * https://chat.mistral.ai/chat

### Donde se suben los modelos Open Source

* Los modelos se suben a HF
  * https://huggingface.co/
* Al usuario Final le suele interesar la parte de los Spaces
  * https://huggingface.co/spaces
    * Ejemplos
      * https://huggingface.co/spaces/black-forest-labs/FLUX.1-dev

> Hay herramientas como ai comic factory que toman un modelo Open Source y lo disponibilizan cobrando por uso

### Como bajo un modelo OS dexto localmente

* Aclaracion
  * Para ejecutar un modelo Localmente es recomendado contar con una buena GPU
  * Las organizaciones pueden pensar en armar una computadora con buena GPU especializada en ejecutar sus modelos de Lenguaje
 
* Opciones Para ejecutar un modelo Open Source
  * Descarga los modelos Open Source de HF
  * Aplicacion de escritorio
    * https://lmstudio.ai/
  * Linea de Comandos
    * https://ollama.com/

### Para probar modelos Open Source Online

* URLS
 * https://groq.com/
 * https://chat.groq.com/ 
* Motor para probar Modelos OS

--- 

# Herramientas

* https://theresanaiforthat.com/
  * Un buen recurso para ver que herramientas de IA existen

---

# Prompt Engineeting

* Teoria
  * https://www.instagram.com/p/C5MDsQiR5cG/?img_index=1
 
* Prompt Ideal
 * Tarea
 * Contexto
 * Ejemplo
 * Rol/Persona
 * Formato
 * Tono

## Contexto

* Toda la informacion que la IA considera para darnos la respuesta
* Se tiene en cuenta
  * Memoria
  * System Prompt
    * Instruccion personalizadas
  * Conversaciones recientes
  * Llamanda a herramientas (Busqueda web)
  * Prompt
    * Todo lo que decimos en el prompt
    * Toda la conversacion que venimos teniendo

(Prompt que escribimos)  ---> (Prompt enriquecido por el proveedor) ---> LLM

"Que me pongo hoy" ---> "Pregunta "Que me pongo hoy" el usuario Pepe que es muy friolento segun sus ultimas conversaciones y quiere que recordemos que le gusta usar jean segun su memoria y que es de CABA y en caba hace 25 grados segun la busqueda que hice" ---> LLM

### Tip 1 : Usar el modo dictado

* Usar el modo dictado que (no el modo voz)
* En general cuando hablamos damos a la IA mas contexto

### Tip 2: Usar el modo sobratico o encadenamiento de prompts

```
Tengo un cliente que me debe plata. Necesito convencerlo por telefono para que pague. Haceme preguntas de a una para tener toda la informacion de contexto necesaria para tener la mejor extragegia para persuadirlo. Cuando tengas todas la informacion necesesaria recien ahi dame una estragegia.
```

* Lo impotrante
 * Pedirle las pregutnas de a UNA

> [!NOTE]
> Cambia la dinamica con la que usamos la IA
