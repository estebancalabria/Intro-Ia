# Clase Dos - 25 de Jundio del 2026

# Repaso

* Roadmap del Curso
* IA Resposable
* Diferencia entre IA Generativa y Tradicional
  *  IA Generativa
    *  Generar algo nuevo
  *  IA Tradicional
    *  Para hacer prediciones
    *  Trabaja sobre datos etructurados
* IA generativo
  *  Modelos de Lenguaje
    *  Funcionmiento del modelo del lenguaje
  *  Modelo de Imagenes
    *  Nano Banana
*  Conceptos de IA
  *  Grounding
  *  Prompt
  *  Token
  *  Alucinacion

----

# Repasar un poco el funcionamiento de los LLM

* Los modelos de lenguaje LLM son **Redes neuronales** digitales que emulane el funcionamiento del cerebro humano (neuronas y sinapsisis)
* Tamaño del modelo : Cantidad de neuronas y conexiones
* Los LLM funcionan prediciendo el proximo token.
    * "LA" ---> El proximo token puede ser  "Casa" o "Persona" equiprobablemente

## Distintos LLM

* Propietarios
  * Gemini
  * ChatGPT
  * Copilot
  * Claude
    * https://claude.ai/new
  * Grok
    * https://grok.com/
* Open Source
  * Llama (de Meta)
  * DeepSeek
  * Qwen

---

# Caracteristicas Gemini

* Google tiene distitnos modelos
    * Gemini 3.5 Flash
    * Gemini 3.1 pro
* Se diferencian en el tamaño (Cantidad de parametros)

* Diferencian en
    * El objetivo de para que fueron entrenados
    * El set de datos de entrenamiento
    * 

* URL
  * https://gemini.google.com/app
  * 
* Caracteristicas
  * Google
  * Modelos : Hay varios para elegir
  * Licenciamiento : Propietario
  

## Coparativa entre dos modelos de Gemini

* Le preguntamos al modelo Flash y al modelo Flash Lite
```
Que modelo sos? Como se llama tu modelo? Que tamaño tenes? Cuales son tus caracteristicas?
```

> [!NOTE]
> Gemini no me responde la cantidad de parametros porque al ser un modelo propietario no qiere dar detalles tecnicos sobre su construccion


# Glosario

* No determinismo de la IA : Ante un mismo prompt la IA puede dar respuestas distintas. Eso se llama No determinismo.
  * Es dificil lograr respuestas deterministicas de un LLM. Si deseo hacerlo tengo que generar un prompt que solicite una respuesta muy especifica y no de lugar a ninguna ambiguedad
* Multimodales
