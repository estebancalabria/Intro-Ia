# Clase Seis
# Primera Clase del 2026
# Ultima Clase

# Repaso

* Herramientas 
    * HeyGen
    * Gamma
* IA Generativa
  * Generacion de Imagen
    * Leonardo.AI
    * Ideogram
    * Nano Banana
  * Generacion de Video
    * Pollo.AI
    * ...


# Machine Learning

> https://www.instagram.com/p/C1ntRrRswAu/?img_index=1

- ## Entrenando un modelo de Clasificacion

* Abrir un documento de Google Sheets Nuevo
* Obtener los datos de Kaggle (https://www.kaggle.com/)
  * Descargar el dataset de titanic : https://www.kaggle.com/datasets/brendan45774/test-file
      * Se descarga un zip que adentro tiene un archivo que se llama tested.csv
  * (Alternativamente el profe lo manda por chat)
* Importar en el Google Sheets
  * File...Import...Upload...(Elegir el archivo).."Replanzar Hoja Actual"
* Preparo los datos
  * Selecciono la columna Age... Formar... Number... Number....
  * Lo mismo columna Fare
* Entender los datos y elegir que columnas son features y cuales labes
  * Label
      * Survided
  * Features
      * PClass
      * Sex
      * Age
      * SibSb
      * Parch
      * Fare
      * Embarqued
* Separar Datos de Prueba y Entrenamiento
  * Duplicar el documento
  * De la fila 2 a la 30 borro el contenido de Survived (lo resguarde en la copia)
* Entrenar el modelo
  * Instalar la extension Simple ML for Sheets : https://simplemlforsheets.com/
  * Refrescar la hoja de calculo
      * Debe aparecer en el menu "Extensiones"... Siple ML for Sheets
  * Le damos Start a la Extension
      * Predict missing Values

       * Elegimos Columns with empty cells: Survived
      * Elegimos Source Columns: PClass, Sex, Age, Sibsb, Pach, Fare, Embarqued
      * Damos Predict
      * Me devuelve una columnua nueva
* Evaluar el modelo
    * Comparar lo que predijo el modelo con la columna que nos copiamos

# Automatizacion y Chatbots

> https://www.instagram.com/p/DIPbzoPOS6v/?img_index=1

- ## Enunciado

* Quiero que al agrebar una fila en una hoja de google sheets se me agregue automaticamente un evento en mi google calendar.
* Quiero que en el medio la IA haga algo (primero sin IA y luego con IA)

- ## Pasos

* Abrir una solapa con hoja de google Sheets Nueva...
  * Ponerle un nombre a la hoja de excel
  * Agregar columnas Evento, Inicio, Fin
  * Configurar la columna Inicio y Fin de tipo FechaYhora
* Abrir otra solapa con el calendario de Google
* Loguearnos en make (https://www.make.com/en)
* Explorar la parte de plantillas/templates para ver ejemplos de automatizaciones que se pueden hacer
* Crear un escenario nuevo
* Completar un registro nuevo en el excel
* ...https://github.com/estebancalabria/Intro-Ia/blob/main/Automatizacion/Labs/LAB-MAKE-03-Sheets-Groq-Calendar-Generar%20Evento%20Google%20Calendar%20desde%20Sheets.md
* Darle run Once...
* Agregar un paso nuevo, integracion con Calendar
  * Actualizar la conexion
  * Completar los campos del dialogo
* Agregar un evento nuevo al calendar
* Probar...
* Sacar una api key en groq : https://console.groq.com/home
* 
  
* 



# Chatbots
