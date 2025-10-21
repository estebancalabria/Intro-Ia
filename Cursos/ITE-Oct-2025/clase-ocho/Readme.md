# Clase Ocho - 21 de Octubre del 2025

# Repaso

* IA Generativa multimedia
  * Gamma.App
  * Generacion de Imagenes
      * Leonardo
  * Generacion de Video
      * Generacion de video a partir de texto
      * Generacion de video a partir de Imagenes
      * Generacion de Efectos
  * Generacion de Audio
    * Suno
    * Udio
    * ...lista de herramientas

# Machine Learning

* Teoria de Machine Learning : https://www.instagram.com/p/C1ntRrRswAu/?img_index=2
* Web de referencia para ML : https://www.kaggle.com/
    * RECOMENDADO EXPLORAR LA PAGINA PARA TODO ENTUSIASTA Y ESTUDIANTE DE ML

## Ejemplo aplicacion Metodologia Machine Learning

1. Obtencion del Dataset
    * Crear un documento nuevo en Google Sheet
    * Descargar el dataset de titanic : https://www.kaggle.com/datasets/brendan45774/test-file
    * Descomprimir el archivo tested.csv del zip que descargamos
    * Importar el archivo tested.csv en el documento de google sheets que creamos
2. Preparar los datos
    * Entender las columnas
    * Separar las columnas en features y labels
    * Labels:
        * Survived
    * Features
        * PClass
        * Sex
        * Age
        * SibSp
        * Parch
        * Fare
    * Datos Descartados
        * PassagenrID
        * Name
        * Ticket (Es una numeracion rara)
        * Cabin (Tiene muchos datos faltantes)
    * Forzar todas las columnas a valores numericos (que la edad y el fare lo tome como valore numericos)
    * Eliminar los que tienen datos faltante (los que no tienen edad)
    * Discretizar valores
    * Normalizar los datos (llevarlos a una escala entre 0 y 1)
3. Separar datos de prueba y entramiento
    * Elegir las primeras 40 filas y separar la columna survibed e una nueva "Expected Survived"
    * Borrar el contenido de la columnua survived a las primeras 40 filas (Datos de Prueba)
    * El resto van a aser datos de entrenamiento
4. Entrenar el modelo
    * Instalar la extension Simple ML for Sheets : https://simplemlforsheets.com/
    * En el menu extensiones elegir "Simple ML for Sheets" y luego "Start"
    * Elegir "Predict missing Values"
    * Elegir la columna survived como label y los features que definimos arriba
    * Darle al boton Predict
5. Analizar lso resultados

## Ejemplo Aplicacion Marchine Learning : Regresion

Hicimos un ejemplo de regresion con la formula : =GOOGLEFINANCE("TSLA","all","2025-09-01",TODAY(),"DAILY")

# IA en Google Sheets

> https://www.sheetgpt.ai/

Si no quiero usar ninguna herramienta lo puedo hacer yo\

> https://www.instagram.com/p/C9dWVhYRhrs/?img_index=1

