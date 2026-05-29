# Clase Nueve - 29 de Meyo del 2026

# Repaso

* IA Generativa Creativa
  * Workflow para crear videos
  * Como crear Videos
    * Herramientas
      * Flow
      * Pollo
      * Pixverse
    * Casos de Uso
      * Motion control
  * Crear Musico
    * Herramientas
      * Udio
      * Suno
  * Heramientas
    * https://passportai.app/
    * Laboratorios de Google
* IA y Productividad
  * IA en Google Sheets
  * IA en excel con copilot

---

# IA Tradicional : Machine Learning

> Analisis de datos, toma de decisiones, predicciones, relacione entre variables

* Teoria
  * https://www.instagram.com/p/C1ntRrRswAu/?img_index=1
* En lugar de Python vamos a trabajar con Google Sheets
    * Vamos a crear una hoja de google Sheets Nueva
      * https://sheets.google.com/
* Vamos a conseguir datos y un problema
    * https://www.kaggle.com/
    * Bajamos el dataset del titani de : https://www.kaggle.com/datasets/brendan45774/test-file
        * Archivo tested.csv

* Enunciado
    * Primero .Veo los datos, los entiendo
    * Determinar dadas las caracteristicas del pasajero si se salva o no (surivved). Las chances de sobrevivir dada las caracteristicas
 * Preparar los datos
   * Clasificar las columnas
       * Features o Caracteristicas (los datos que voy a usar para predecir)
         * Pclass
         * Sex
         * Age
         * SibSp
         * Parch
         * Fare
         * Embarked
       * Labels (Los datos que quiero predecir)
         * Survived
       * Columnas Descartadas
         * PassengerID
         * Name
         * Ticket (No tiene una logica)
         * Cabin  (Tiene muchos datos faltantes)
   * Ordenar los datos
       * Sacar filas con datos faltantes
       * Poner formato de numero a todas las columnas
 
* Instalar una extension de google sheet
    * Para no tener que usar python
    * https://simplemlforsheets.com/
 

* Para resguardo y chequear todo vamos a hacer un backup de la hora
  * Duplicar hoja
 
* Separar datos de entrenamiento y prueba
    * Para este ejercicio separar los datos de entrenamiento y prueba es borrar los datos de columna survived a los datos de prueba
 
* Entrenar el modelo y hacer predicciones
    * Dio perfecto!!
 
* No solo voy a predecir, sino que voy a usar el modelo para sacar conclusiones de los atos

---

# Agente de recuperacion de datos con NotebookLM

> https://notebooklm.google.com/

> Puntaje : 11/10

## Otra alternativa de google para agentes

* Se pueden hacer los Gems 
