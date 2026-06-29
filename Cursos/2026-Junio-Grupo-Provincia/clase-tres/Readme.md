# Clase Tres - 29 de Junio de 2026

# Repaso

* LLM
  * Propietarios
    * Caracteristicas generales
      * Compartir conversaciones
      * Mutimodalidad
    * Copilot
    * ChatGPT
    * Grok
    * Gemini
      * Groundig : Buena integracion con el motor de busqueda
      * Gran ventada de contexto (destacado)
      * Integracion con ecosistema de google
      * Modo investigacion
  * Open Source
    * Se pueden ejecutar Locamente
    * Son importante al considerar la privacidad

---

# LLM

## Prompietarios

### Gemini

#### Modo Investigacion

* Investigacion realizada la clase pasada
  * https://share.gemini.google/TZOjKJGVuTrR* 

#### Modo thinking

* Gemini tambien incopora el modo "thinking" que vimos con deepseek

---

## Open Source

### Modelos Open Source

> [!NOTE]
> Si solo hubiera modelos propietarios habria una concentracion/monopolio de poder en cuanto a la IA
> La empresas que construyen modelos podria cobrar lo que quisiera por su usuo y concentrar su uso solo en lo que los pueden pagar

* Chinos
  * DeepSeek
  * Qwen
    * La copia Open Source de ChatGPT
    * Desarollado por AliBaba
* Americanos
  * Familia Llama
    * Los modelos de IA que vienen en Wsap
  * Google
    * Familia Gemma
    * Google hizo tambien modelos open source que se pueden probar en:
      * https://aistudio.google.com/prompts/new_chat

### DeepSeek

* Entrenar el primer modelo de lenguaje con el modo pensamiento
* Implementa internamente y de forma transparente una tecnica de prompting que se llama "Cadena de pensamiento" (chain of thoughts)
  * Se descubrio que cuando le hago una pregunta compleja a la Ia y le pido que explicite el razonmiento que utllizo para llegar a la respuesta la IA me da respuestas mas acerdas

 #### Modo pensado

 * Lo usamos cuando la respuesta depende del razonamiento mas que de consulta de datos
 * Para resolver un problema de logica, matematica, etc

## Ejecucion modelos Open Source Localente

* Ollama
  * https://ollama.com/
* LMStudio
  * https://lmstudio.ai/

---

# Evaluacion de modelos

* Ya sea Open Source o Propietario para evaluar en un momento determinado cual es el mejor modelo para una tarea especifica:
    * https://arena.ai/
* Vamos a hacer competir dos modelos con el sigueinte prompt

```
Quiero una investigacion sobre las leyes, normarivas y resoluciones y actualizacion de leyes, normarivas y resoluciones en Argentina a nivel nacional y provincial sobre los seguros de riesgo de trabajo. Quiero saber cuales fueron las ultimas actualizaciones de la ley a tener en cuenta. Acota la busqueda de actualizaciones al 2026. Una comparativa de qué cambió respecto a la resolución anterior que modifica la nueva resolución (de forma breve). Incluir riesgo de trabajo in itinere (camino al trabajo) 
```

* Ese ultimo prompt tardo un  moton entonces voy a probar con

```
Cual es el sentido de la vida?
```

---

# Herramientas

## Texto a Vos (TTS) 

### Natural Readers

* Url
  * https://www.naturalreaders.com/
* Caracteristica
  * Capacidad de converrtir e texto a voz
* Puntaje
  * 8 / 10

---
# Glosario

* Guardrails : Protecciones de seguridad que tienen los LLM para evitar generar contenido no apropiado.
