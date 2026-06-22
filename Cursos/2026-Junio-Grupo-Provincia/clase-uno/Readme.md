# Grupo Pronvincia

# Clase Uno - 22 de Junio del 2026

# Roadmap

* Fundamentos de la IA
   * Tipos de IA (IA Generativa vs IA Traidcional)
   * Modelos de lenguaje (LLM)
     * Tipos de Modelo
   * Concptos Base: Token, prompt, alucinaciones, multimodalidad, agentes
   * Riesgos y las precauciones que tengo que tener a la hora de usar la IA
* Prompt Engineering
   * Tecnicas para obtener respeustas mas efectivas de la IA
   * Errores comunes
   * Buenas practicos (Tips)
* IA para potenciar el trabajo
  * Herrarmientas del Ecosistema Gemini
    * Ej: NotebookLM
  * Presentaciones y Documentos
  * Casos de uso del mundo real
* IA Generativa Multi Media
  * Generacion de Imagenes (Nanno Bannano)
  * Videos
  * Musica
  * Etica 

---

# Links

* https://gemini.google.com/app
* https://platform.openai.com/tokenizer
* https://aistudio.google.com/
* 

---

# Fundamentos de la IA

* IA Tradicional vs IA Generativa
  * IA Tradicional : Trabaja con datos estructurados (tipo tabla) para hacer predicciones
     * Se entrena un modelo estucturado con un gran volumen de dato que se usa para hacer prediciones sobre datos nuevos
     * Hoy en dia se usa mas que nunca cuando se vio el potencial general de la IA
  * IA Generativa
     * Genera contenido nuevo

* Large Language Models (LLM)
  * Redes Neuronales

# Como funciona la IA Generativa (Texto)

* Entrenamiento
   * (Dataset Enorme / Toda la info de intetnet)  ---> Entrena un modelo
     * Aprende cosas como cada vez que esta la palabra Hola sigue la palabra que (Hola que)
     * Dado un texto aprende a predecir el proximo token
   * Lleva tiempo y consume muchos recursos (dinero y tiempo)
   * El resultado es un archivo
* Uso
  * (Frase) ---> (Modelo)  ---> (Predecir el proxito oken)
  * "Hola" ----> (Modelo)  ----> "Hola que"
  * Para generar una respuesa completo lo anterior se repite muchas veces (iteracion)

> Le pregunté a gemini si entendía lo que decía y me respondió esto: Es una excelente pregunta. La respuesta corta es que no "entiendo" como lo hace un ser humano, sino que soy un modelo de lenguaje avanzado que procesa y relaciona palabras a un nivel extremadamente complejo.

## Implicaciones del funcionamiento

* Los modelos de lenguaje predicen tokens basado en lo que aprendieron antes en forma probabilista
  * No piensan
  * No razonan
  * No tienen experiencia
* Por eso la respuestas que dan:
  * Alucinacion : Muchas veces alucinan
  * Inventa
    * Grounding : Anclar la respuesta de la IA en fuentes verificables

> Google trata de dar el mejor grounding posible a las respeustas de Gemini y para ello utiliza mucho la busqueda web

## Otros modelos de IA Generativa

* Basados en imagenes
  * Nanno Bannano
* Basados en video
* Basados en Audio

## Modelos de IA Generativa de Texto

* Caracteristica
   * Arquitectura (Como estan organizadas las neuronas)
   * Tamaño del modelo (Cantidad de parametros) : Cantidad de conexiones entre neuronnas que tiene el modelo.
   * Tamaño de la ventana contexto : La cantidad de texto maxima que el modelo puede procesar
   * Licenciamiento : Propietarios y Modelos Open Source
      * Propietarios : La empresa que lo entreno mantiene el archivo del modelo bajo llave y solo lo deja usar por el portal web (o la api)
      * Open Source : Alguien entrena un LLM y pone a disposicion el archivo del archivo para que se pueda bajar, modificar y usar localmente
   * Tipo: Rapidos y los de pensamiento
 
  
> [!NOTE]
> Los modelos de Google se caracterizan por su capacidad de procesar mucha informacion a la vez. Se dice que tienen una ventana de contexto muy grande.

---

# Glosario

* Machine Learning : Se usa para entrenar modelos de IA Tradicional
* Prompt : La instruccion que el usuario le brinda a un modelo de IA generativa
* Token  : Subdivision de un prompt (palabra)
* Tokenizacion : Proceso de dividir un prompt en tokens.
* Limites de uso y costes basados en Tokenizacion.
* LLM : Large Language Model o Modelo de lenguage Grande
* Dataset : Conjunto de datos
* Entrenamiento de un LLM : Darle a una red neuronal que tiene la arquitectura trasnformer un monton de datos para que aprenda estadisticamente como es la relacion entre los disntitos tokens para que pueda predecir la proxima palabra
* Alucinacion : Cuando un modelo de lenguaje responde de una forma no coherente
