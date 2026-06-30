# Clase Tres - 29 de Junio de 2026

# Repaso

* LLM
  * Caracteristicas Generales
    * Lienzo, Canvas, Artefacto
      * Te permite editar parte de la respuesta del LLM sin tener que regenerar todo
  * Propietarios
    * Gemini
      * Integracion con ecosistema de Google
      * Modo investigacion
    * Claude
  * Open Source
    * DeepSeek
      * Inventor del modo pensamiento profundo
    * Qwen
 

# Repaso Canvas editable

```
Generame un canvas editable con una letra de una cancion para apoyar a la seleccion espaniola este mundial
```

# Repaso modo Investigacion

* Investigacion que realizamos
  * https://share.gemini.google/JPc6M7UWVDTP

---

# LLM

## Introduccion

> [!NOTE]
> Dependiendo la tarea voy a elegir el modelo mas adecuado para la misma

## Propietarios

### Gemini
\
* Ventana de contexto apliada

```
Cual es tamanio de tu ventana de contexto
```

* Gemini tiene una venta de contexto de 1 millón de tokens y genera salidas de 8,192 tokens.

### Grok

* Grounding de X
* Mucho menor censura que otros modelos

## Open Source

> [!NOTE]
> Estos modelos son necesarios en contexto donde la privacidad de los datos.
> VER El GDPR (Reglamento General de Protección de Datos)

### Mistral

* URL
  * https://mistral.ai/
* Caracteristicas
  * Modelo Frances
  * Siempre segundo

## Elegiendo el modelo...

* URL
  * https://arena.ai/
* Caracteristicas
  * Me permite poner a prueba un prompt con dos modelos y elegir el mejor
  * En base a lo que vota la gente se arma un rankin de modelos segun la tarea
 
## Ejecutar un modelo Open Source Localmente

* Las dos herramientas mas populares:
  * Ollama
   * https://ollama.com/
  * LMStudio
   * https://lmstudio.ai/
   * Dificultad
    * (BAJA)

## Repositorio Public de Modelos Open Source

* Url
  * https://huggingface.co/
* Caracteristicas
  * Es un repositorio publico donde se suben modelos de IA Open source (no solo de texto, sino de todo tipo)
  * Hay que crearse un usuario
  * Lo importante que tiene es lo de spaces
    * https://huggingface.co/spaces

---

# Herramientas

## Text-To-Speech

###  Natural Readers

* Url
  * https://www.naturalreaders.com/
* Catacteristicas
  * Conversion de texto a voz
* Puntaje
  * 7 / 10

---

## Generacion de Diagramas

### Napkin

* URL
  * https://www.napkin.ai/
* Caracteristica
  * Genera Diagramas a partir de Texto
* Puntaje
 * 8/10

---

# Prompt Engineering

* Teoria
  * https://www.instagram.com/p/C5MDsQiR5cG/?img_index=1
* Prompt
  * Tarea
  * Contexto
  * Ejemplo
  * Persona/Rol
  * Formato
  * Tono

## Contexto

* Todo lo que la IA considera para darnos una respuesta
  * Prompt
  * Toda la conversacion
  * Conversaciones pasadas
  * Memoria
  * System Prompt
    * Instrucciones Personalizadas
  * Herramientas
    * Busqueda Web
  * RAG (Base de datos de documento)
* Ventana de contexto
 * La cantidad de tokens que el modelo puede producir considerando la entrada y la salida

* (prompt) -->  (prompt + memoria + conversacion + system prompt + busquedas web)     -> (LLM)
* "quien descubrio america" -> "El usuario Esteban Calabria pregunta quien descubrio america tener que responder de forma amable.... -> LLM

### Tecnicas de prompting : Interaccion

* AKA
 * Encadenamiento de prompts
 * Prompt Chainning
 * Metodo socratico

* Sin tecnica

```
Armame un plan de comidas para el dia de hoy?
```

* Aplicando la tecnica de interaccion

```
Armame un plan de comidas para el dia de hoy. Quiero que me hagas todas las preguntas necesesarias de a una para determinar el plan de comida optio que mas me guste y se acerque a mis objetivos. Haceme todas las preguntas que necesites de a una hasta que tengas toda la informacion necesaia para armarme el pla de comidas. Importante que no te apures y te asegures de preguntarme todo lo necesario antes de sugerirme un plan.
```

## Tips de Prompt Engineering

* Usar el modo voz puede ser una muy buena estrategia para darle mas contexto a la IA cuando le escibo un prompt
* Pedirle a la IA que cuando me haga preguntas me las haga de a una

## ROL

### Tecnica de prompting

* Solapa 1
  * Prompt sin especificar Rol
  * "Me duele la panza? que hago?"
* Solapa 2
  * Prompt especificando Rol
  * "Actua como si fueras un doctor gastroentrologo expertos en dolencias de estomago y dime como evaluar y que hacer antes un dolor de panza"
* Solapa 3
  * Prompt especificando a una personjae especifico conocido
  * "Actua como si fueras Julio Iglesias (el cantante) y dime que hacer si me duele la panza"
* Solapa 4
  * Invocar un panel de espertos
  * "Quiero que armes un panel de expecialistas y cada uno me de su vision de como actuar cuando a una persona le de duele la panza. Que cada especialista me responda en unas pocas oraciones."

---

# Glosario

* System Prompt : Una instruccion oculta que le da el proppietario del modelo de lenguaje que determina su personalidad y manera de comportarse

* Grounding : Anclar la respuesta de la IA en fuentes verificables

* Censura : Capacidad que tienen los modelos de lenguaje de evitar desponder temas que son illegales e inapropiados
  * GuardRails : Mecanismo que tiene los LLM para bloquear peticiones y respuestas inapropiadas
