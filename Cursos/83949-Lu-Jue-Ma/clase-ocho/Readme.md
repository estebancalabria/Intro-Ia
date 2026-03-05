# Clase Ocho - 5 de Marzo del 2026

# Repaso

* Generacion de Videos
  * Herramientas
    * Grok / Imagine
    * RunwayML
    * PolloAI
    * Pixverse
    * Pika Art
  * Modelos
    * Sora
    * Veo
    * Seeddr
    * eam

# Machine Learning

> https://www.instagram.com/p/C1ntRrRswAu/?img_index=1

* Ejemplos de Machine Learning
  * Clasificacion
    * Clasificar Fotos
    * Predecir si un usuario va a ver o no una pelicula
       * https://www.instagram.com/p/DQH8J2eAbgO/
    * Clasificar pacientes de Riesgo en el COVID
  * Regresion (Predecir datos futuros)
     * Predecir cantidad de asistentes de una clase
     * Predecir ventas
  * Deteccion de Anomalias
     * Detectar transacciones fraudulentas

* Conseguirlo datos
  * https://www.kaggle.com/ <<<<< El recurso mas importante para aptender Machine Learning
    * De aca vamos a descargar : https://www.kaggle.com/datasets/brendan45774/test-file
    * Bajamos un zip y descomprimimos un archivo tested.csv

* Abrir Google Sheets
   
* Importamos en google Sheets
  * File... Import... Upload
 
* Instalar la extension Simple ML For Sheets
  * https://simplemlforsheets.com/
  * Luego de instalar la extension hay que "Refrescar" el google Sheets y tiene que aparecer en el menu extensiones "Simple ML for Sheets"
 
* Clasificamos las columnas en "Features y Labels"
  * Label
     * Survived
  * Features
     * Pclass
     * Sex
     * Age
     * SibSp
     * Parch
     * Fare
     * Embarked
  * Columnas Descartas
     * PassengerId
     * Name
     * Ticket (Porque no hay uniformidad en el tipo de dato)
     * Cabin (Hay muchos datos Faltantes)

* PReparar los datoss
   * Agarro la columna Fare... le pongo.. Format...Number (PAra forzar que sea numerica)
   * La columna edad lo mismo...Format...Number...

* Separar datos de prueba y entrenamiento 
      * Duplicar el libro para tener un backup de los datos
      * En el original le borro la columna survived a los primeros 15 registros
         * Cuando eliminamos la columna survived para un registro significa que lo vamos a usar como dato de prueba para predecir que tan bien funciona el modelo.
         * No estamos hablamdo de modelos que tienen un 100x100 de efectividad. Siempre buscamos modelos que sean "lo suficientemente buenos"

* Entrenar el modelo y evluarlo
   * Extensions...Simple ML For Sheets...Predict Misssing Values
   * Columna con Celda Vacia
      * Survived
   * Source Columns
     * Pclass
     * Sex
     * Age
     * SibSp
     * Parch
     * Fare
     * Embarked
     * (Me tengo que asegurar que sean de tipo Num o Cat, no text)

* Dale a predict y aparece columna nueva : Pred:Survived
  * Comparar el resultado con los datos originales que tenia en el documento duplicado

> OJO: Este ejemplo da PERFECTO, pero en la vida real no todos los modelos de ML tienen tanta efectivicdad, uno debe definir el grado de efectividad aceptable en su negocio

* Ver informe del Modelo
   * Repetimos el proceso Extensions...SimpleML.. Start...Advanced Tasks...Understand a Model...
      * Elegir el modelo que viene por defecto
      * Ir a la solapa "Variable Importance"

```
Variable Importance: INV_MEAN_MIN_DEPTH:
    1.      "Sex"  1.000000 ################
    2.     "Fare"  0.431494 #
    3.      "Age"  0.425176 #
```

> Vemos que para este ejemplo esas son las variables mas importantes, por eso decian "Las mujeres y los ninios primero" !
