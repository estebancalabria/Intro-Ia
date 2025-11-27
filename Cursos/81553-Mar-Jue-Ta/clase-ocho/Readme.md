# Clase Ocho - 27 de Noviembre 2025

# Repaso

* Generacion de Imagenes localmente o con el Colab
    * Foocus
* Generacion de Video
    * Modelos
        * Sora
        * Veo3
    * Herramientas
        * Grok (Rapidisima, divertida, Videos desde imagenes sin esfuerzo)
        * Pollo.AI (La que va)
        * PixVerse (Muy buena Alternativa)
        * Pika Art (Para los efectos)
        * Runway (De las clasicas)
        * Kling (Una china)
* Geneacion de Canciones
    * Suno
    * Udio
      
# Herramienta NUEVA!

* Text-To-Speech (Clonado de voz Facilisimo)
> Puntaje 10 / 10

# Machine Learning

* Ver Carousel Super Fachero Del profe (y dejar me gusta) : https://www.instagram.com/p/C1ntRrRswAu/?img_index=5
* Recursos principal para aprender Machine Learning : https://www.kaggle.com/ 

Manos a la obra con Machine Learning

* Crear una planilla de Google Sheets en Blanco
* Loguearse a Kaggle : https://www.kaggle.com/ 
* Ir a la pagina del Dataset de Titanic https://www.kaggle.com/datasets/brendan45774/test-file
* Descargar el Zip del dataet
* Descomprimir el archivo tested.csv
* Importar el archivo en nuestra planilla de Google Sheets
* Seleccionar Features Labels
    * Label : Marcar la columna Surved con un color (Verde) Seria nuestro LABEL (Lo que queremos predecir)
    * Feature : PClass, Sex, Age, SibSP, Parch, Fare, Embarqued
    * Fuera : PassengerID, Name, Ticket, Cabin (muchos valores nulos)
* Instalar la extension de Google Workspace Simple ML For Sheets
    * https://simplemlforsheets.com/
    * https://workspace.google.com/marketplace/app/simple_ml_for_sheets/685936641092
    * Una vez instalada refrescar el google sheets y en meu extensioens debe aparecer "SimpleML for Sheets"
* Separ datos de Prueba y de entrenamiento
    * Tomar Las primeras/ultimas N filas (ej 30) y copiarlas a otra hoja
    * Borrar el contendio de la columna survived para las prieras N filas (tenemos un bakcup en la otra hoja)
* Extensiones...SimpleML For Sheets...Start
    * Elegimos "Predict Missing Values"
    * Column with empty cells : "Survived"
    * Source Columns : PClass, Sex, Age, SibSP, Parch, Fare, Embarqued
        * (Si alguna de las columnas anteriores aparece como tipo Date y Nun hay que corregir el tipo de dato)
          * Elegir Columna + Format + Number + Number
        * Depende de la configuracion regional
* Comparar Resultados con Expectativas para verificar la efectividad del m odelo

> Puntaje : 9.323223 / 10

# Usar la IA en Google Sheets

* Abrir un Google Sheets Nuevo
* Crear un documento nuevo con dos columnas Paies y Capitales
* Instalar extension
    * https://www.sheetgpt.ai/
    * https://workspace.google.com/marketplace/app/sheetgpt_ai_and_chatgpt_for_sheets/1071108744264?_gl=1*cm434d*_gcl_au*ODIzNTQzOTU2LjE3NjEwNzAxNTI.
* Darle Extensios...SheetGPT... Enable
* En la primer Columna debo del titulo poner la siguiente formula
    * =GPTLIST("Dame una lista de los paises de LATAM ordenados Alfabeticamente")
* Luego el la celda B2 poner el siguiente prompt:
    * =GPT("Dame la capital del siguente pais. Devolver solamente el nombre de la capital sin acotar nada mas. Quiero la capital de : " & A2)
* Arrastrar esa celda a todalas la de abajo
* Copiar el prompt como nota y copias y pegas solo valoras (Par que no recalcule)
