# Clase Cinco - 6 de Julio 2026

# Repaso

* LLM
  * Open Source
    * Importancia : Por la privacidad de los datos
* Open Source
    * Hugging Face
      * Spaces de Hugging Face
      * Optunidades de negocio alrededor del OS
          * Ejemplo del Comic Factory
* Herramientas
  * There is an AI for That
  * Speech-To-Texto
      * Taqtic
* Prompt Engineering
    * Partes: Tarea + Contexto + Ejemplo + Rol + Formato + Tono
    * Contexto
        * Personalizacion
        * Memoria
    * System Prompt

---

# Prompt Engineering

## Tecnicas de Prompting

> [!NOTE]
> Las tecnicas de prompting que vamos a estudiar se puede y se deben combinar (en general las vemos por separado)

### Contexto 

> [!NOTE]
> Importante para Gemini
> Es un modelo que se busca diferenciar por su tamanio de ventana de contexto (+1M tokens)

#### Interaccion 

* Plantilla
  * [TAREA].  Quiero que me hagas preguntas **de a una** hasta tener todo el contexto necesario para darme una repsuesta especifica para [OBJETIVO]

* AKA
  * Prompt Chainning
  * Encadenamiento de Prompts

* Sirve para evitar respuestas genericas y obtener respuestas mas utilies y especificas

* Abran dos solapas de Gemini
  * Pregunta sin el patron interaccion
    * "Armame una rutina de ejercicios para la semana"
  * Utilizando el patron interaccion
    * "Armame una rutina de ejercicios para la semana. Quiero que me hagas preguntas de a una hasta tener todo el contexto necesario para darme una repsuesta especifica a mis necesidades"

---

### Rol

> [!NOTE]
> Empiricamente me dio excelentes resultados que el rol apunte a la excelencia (el mejor en....)  (con mas de 50 anios de experiencia en...)

* Abrir 4 solapas de Gemini
  * Sin rol
    * "Quiero comprarme una dashcam. Dame recomendaciones"
  * Explicitando el rol
    * "Actua como un experto en gadgets com 20 anios de experiencia y el mas especialido en camaras del mundo.  Quiero comprarme una dashcam. Dame recomendaciones."
  * Una persona fisica real
    * "Actua como si fueras Elon Musk. Quiero comprarme una dashcam. Dame recomendaciones"
    
#### Panel de expertos

* Citamos a un panel de expertos

```
Quiero analizar la posibilidad de lanzar un nuevo seguro patrimonianles de riesgo como empresa. Me gustaria conformar un panel de expertos y que cada uno me de su vision sobre los aspectos a tener en cuenta para el nuevo lanzamiento. Que cada experto me de un parrafo con su aporte.
```

* Genero esta salida:
  * https://share.gemini.google/guBUPTO2Dq8b
 
---

### Formato + Tono

* Vamos a arrancar con este prompt:

```
Dame una lista de top 10 de  series sitcom. Quiero el nombre, el /los directorios, el anio de lanzamiento, la cantidad de temporadas, cantidad total de capitulos, si termino o fue cancelada, los nombres de los actores principales, puntaje en imdb.
```

#### Formatos Tecnicos

* Se utilizan cuando queremos una respuesta esctructurada en un formato estandar.
* Se utilizan mucho en sistemas y para cargar informacion en aplicaciones

* JSON
  * "Dame la lista y todos los datos que te pedi en json"
* XML

#### Formatos Pseudo-Tecnicos

* PDF
  * "Me podes generar un pdf para presetnar con la informacion"
  * Gemini genera pdfs bastante aceptables
  * Pero a veces tengo poco control sobre como quiero la salida
  * Gemini destaca en la generacion de los PDF (ChatGPT los hace con peor formato)
* PPT/Docs/ Sheets (Excel)
  * Recordemos que Gemini tiene completa integracion con el ecosistema de google y el google workspace
  * Especial para cuando hablamos de gemini
  * PPT (Genial Gabriela)
    * https://gemini.google.com/share/f65b8aa2ecfb?skid=8d0faba0-84c5-4ffa-90ae-e6183c14b4e9
* HTML
  * Lo uso cuando quiero hacer un pdf y me gustaria tener mayor control de la salida
  * "Me podes generar un documento html con la lista de series para imprimir en pdf que se vea profesional, elegante, responsive y destaque."
* CSV
  * Dame la lista en CSV
  * Formato muy utilizado en ciendia de datos

#### Generacion de Plantillas de respuesta

> [!NOTE]
> La IA es no deterministica. Mismo prompt no genera misma salida siempre

* Problema
  * Nunca les paso de generar un documento de word copiando la salida de la IA y despues tener que estar bastante tiempo actualizandole el formato y ajustando la salida como la deseo
  * No determiniso de la salida
* Solucion
  * Definir una plantilla especificando a la IA el formato exacto de la salida que deseo.
  * Ideal utilizar el formato Markdown que es el que utiliza internamente la IA para dalre formato a la salida que vemos en el chat
  * 
 

