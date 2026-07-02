# Clase Cuatro - 2 de Julio del 2026

# Grupo Provincia

# Repaso

* Herramientas
  * Text-To-Speech
    * NaturalReaders
  * Napkin
* LLM
  * Open Source
    * Modelos
      * Gemmas (Google)
      * Qwen
      * DeepSeek
        * Modo pensamiento/razonamiento
    * Ejecutar un modelo OS Localmente
      * LMStudio
      * Ollama
  * Aistudio de google
  * Comparar modelos
      * Arena.AI
        

---

# Large Language Models

## Propietarios

### Instrucciones personalizadas en Gemini

* Se accede en
 * (Abajo a la izquiera en el  nombre de usuario) -> (ruedita) -> personal Intelligence -> Instrucciones para Gemini

```
Quiero que me respondas siempre en poesia. Tu respuesta siempre debe ser un poema y debe rimar. No se aceptan respuestas que no sean poemas con metaforas y obras maestras literarias
```

### Memoria

* Los llm recuendan detalles del usuario y lo guardan como memoria

---

# Herramientas

## There is an AI for That

* URL
  * https://theresanaiforthat.com/
* Caracteristicas
  * Catalogo online de herramientas de IA
  * El numero de herramientas de IA crece exponencialmente con el tiempo


## Speech-To-Text

* Existen un monton de herramientas
  * https://www.instagram.com/p/DBzb-kHxqae/?img_index=1

### Taqtic

* URL
  * https://tactiq.io/es
* Caracteristicas
  * La elegida por el profe

---

# Open Source

> [!NOTE]
> El OS es importante para las organizaciones por un tema de privacidad de datos.

## HuggingFace

* URL
  * https://huggingface.co/
* Caracteristica
  * Una organizacion sin fines de lucro que nuclea un repositorio centralizado de todos los modelos open source cuyo objetivo es democratizar el acceso a la IA
  * Tiene una seccion "spaces" donde puedo probar los modelos open source en forma limitada online
    * https://huggingface.co/spaces
    * Por ejemplo Speech to Text
      * https://huggingface.co/spaces/Oriserve/ASR_arena
    * Por Ejemplo Generacion de Imagees
      * https://huggingface.co/spaces/black-forest-labs/FLUX.1-dev

* Creado con Flux en Spaces "A Cute kitten"
<img width="1024" height="1024" alt="image" src="https://github.com/user-attachments/assets/2157177d-a796-463d-8736-fed96de094dd" />

> [!NOTE]
> Hay una tendencia/oportunismo en comercializar los modelos open source generando una web que te permite utilizar un modelo OS y cobrando por su uso

---

# Prompt Engineering

* Teoria
  * https://www.instagram.com/p/C5MDsQiR5cG/?img_index=1

## Prompts

* Componentes de un prompt
  * Tarea
  * Contexto
  * Ejemplos
  * Persona/Rol
  * Formato
  * Tono

### Contexto

* Es toda la informacion que la IA utiliza para genear una respuesta
* El contexto Incluye
  * El prompt que ingresa el usuario
  * Toda la conversacion
  * El historial de las ultimas conversaciones (reciente)
  * El System Prompt
     * Las Instrucciones Personalizadas me permiten influir en el system prompt
  * Memoria
  * Llamada a herramientas (Tool Calling)
    * Busqueda web
  

(prompt) --> (le agrega el system prompt) -> (instrucciones personalizadas) -> (le info sobre el historial de conversaciones) -> (le agrega datos de la memoria) -> (hace una busqeuda web) ---> ... ---> (llm)

* Uno escribe
  * "Decime como Va argentina en el mundial"
* Al llm le llega
  * "El usuario Esteban Calabria que es ingeniero en sistemas que le gustan las respuestas como poema pero a la vez tengo que se amable en la respuesta porque asi me pide Google que ademas la semana pasasa vio el partido del mundiioal y ademas en la web encontre que argentina juega el viernes con Cabo Verde..."   

### Tips para darle mejor contexto a la IA

> [!NOTE]
> Utilizar el modo voz o dicta muchas veces me permite darle a la ia en un prompt mucho mas detalle del que le daria normalmente solo escribiendo

> [!NOTE]
> Escribir prompts "largos" con mucha informacion relevante y accesoria a la tarea generalmente genera respuestas mucho mas efectivas y la ia suele utiliar doa la informacio que pasamos

---

# Glosario

* FOMO (Fear of missing out) : Ansiedad que genera no estar al dia en temas ia.
* System Prompt : Es una instruccion oculta que le da el propietario del modelo y regula su comportamiento, personalidad y forma de responder

--- 

# Proxima Clase : Seguimos con prompt engineering 
> No olvidar el tip de usar a la misma ia como experto en prompt engineering
