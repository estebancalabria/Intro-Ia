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
* Los modelos tienen tambien un tamaño de contexto expresado en cantidad de tokens

> [!NOTE]
> Los modelos manejan informcion hasta el ultimo momento que fueraon entrenados.

* Los modelos pueden usar herramientas (tools)
 * La herramienta de busqeda de internet permite a los modelos contestar con informacion actualizada (y verificable)

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

* Caracteristicas comunes a todos los LLM
 * Todos tienen la capacidad de compartir una conversacion

---

# Caracteristicas Gemini

* Google tiene distitnos modelos
    * Gemini 3.5 Flash
    * Gemini 3.1 pro
* Se diferencian en el tamaño (Cantidad de parametros)

* Diferencian en
    * El objetivo de para que fueron entrenados
    * El set de datos de entrenamiento
      

* URL
  * https://gemini.google.com/app
* Caracteristicas
  * Google
  * Modelos : Hay varios para elegir
  * Licenciamiento : Propietario
  * Cantidad de Parametros (Tamaño) : ???? (La empresa no lo revela)
  * Tamaño Contexto :
    * 1M tokens de Entrada (Toda la saga de libros de Harry Potter)
    * 65K tokens de Salida
   * Llamada a herramientas

## Caracteristicas Gemini

### Integracion con el ecosistema de Google

* Ecosistema de Google
 * Google Calendar
 * Google Drive (Sheets, Docs)
 * Google Maps
 * Google Hotels
 * Google Flights

#### Integracion con calendar

```
Generame una evento de una hora hoy a las 17:00 en mi google calendar que sea  "Preparar clase AZ-400"
```

* Luego confirmo y verifico que efectivamente se haya generado el evento

---

#### Integracion con Groogle Flights y Google Hotels

```
Quiero ir al mundial a ver el proximo partido de Argentina. Quiero que me busques opciones de Vuelos en google flights y de alojamiento en google hotels.
```

* Se conecta mediante el uso de herramienta con Google Flights y Google Hotels

---

#### Integracion con Google Drive (sheets)

```
Me podes generar una tabla con los datos de la inflacion en los ultimos 12 meses para exportar a google sheets
```

* Esto me genera una tabla que abajo tiene un boton con tres puntitos (...)
* Ese boton me permite la opcion "Export to Sheets"
* Una vez generada la planilla me aparece una notificacion emergente que si le doy click me abre la planilla

---

### Modo Investigacion (Grounding)

* Permite explorar cientos de paginas web sobre un tema especifico y generar un informe
* La version gratuita te permite hasta tres investigaciones por mes

```
Quiero una investigacion sobre las leyes, normarivas y resoluciones y actualizacion de leyes, normarivas y resoluciones en Argentina a nivel nacional y provincial sobre los seguros de riesgo de trabajo. Quiero saber cuales fueron las ultimas actualizaciones de la ley a tener en cuenta.  Acota la busqueda de actualizaciones al 2026.  Una comparativa de qué cambió respecto a la resolución anterior que modifica la nueva resolución (de forma breve). Incluir riesgo de trabajo in itinere (camino al trabajo)
```





---

## Coparativa entre dos modelos de Gemini

* Le preguntamos al modelo Flash y al modelo Flash Lite
```
Que modelo sos? Como se llama tu modelo? Que tamaño tenes? Cuales son tus caracteristicas?
```

* Conversacion Modelo Flash
  * https://share.gemini.google/YvYjzkvx82wZ
* Conversacion Modelo Flash-Lite
  * https://share.gemini.google/obD3NxYEJDK7
* Conversacion con DeepSeek (Open Source y compartia la cantidad de parametros)
  * https://chat.deepseek.com/share/va6nd33o9tmv12qvw1

> [!NOTE]
> Gemini no me responde la cantidad de parametros porque al ser un modelo propietario no qiere dar detalles tecnicos sobre su construccion
> Si le pido esa informacion a Deep Seek Me la da


# Glosario

* No determinismo de la IA : Ante un mismo prompt la IA puede dar respuestas distintas. Eso se llama No determinismo.
  * Es dificil lograr respuestas deterministicas de un LLM. Si deseo hacerlo tengo que generar un prompt que solicite una respuesta muy especifica y no de lugar a ninguna ambiguedad
* Multimodalidad : Capacidad del modelo de interpretar imagenes, pdt, etc... ademas de texto plano
* RAG (Retrival Augmented Generation)

# PRoxima clase

* Hablar del modo pro y cuando se usa
