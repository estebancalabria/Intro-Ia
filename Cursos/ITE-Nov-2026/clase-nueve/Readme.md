# Clase Nueve - 26 de Noviembre de 2026

# Repaso

* Azure
  * Plataforma de Microsoft de Pago
      * Generalmente modalidad pago por uso
      * Subscripcion
  * Creabamos recursos
      * Agrupaban en un Grupo de Recursos o Resource Group
  * Microsoft Foundry
    * Marca que agrupa todos los servicios de IA de Azure
    * Se crea el rescurso en el portal de Azure y despues la gran mayoria tiene un portal aparte para que se pueda probar
    * Servicios con Modelos Pre-Entrenados
        * Microsoft Foundru
            * Permite desplegar modelos OS y Propietarios
            * Los podemos usar por medio de la API KEY
            * Tiene su portal : https://ai.azure.com/
        * Computer Vision
        * Language Service
        * Translator
        * Speech Service
        * Face API
    * Servicios para entrenar tus propios modelos
        * Custom Vision
          * Entrenar modelos con nuestras propias imagenes
        * Machine Learning

# IA Tradicional (Machine Learning)

* Teoria
  * https://www.instagram.com/p/C1ntRrRswAu/?img_index=1
* Seguir el prceso de ML
  * Setup
      * Abrir una planilla nueva de google Sheets
      * Instalo la extesion de Simple ML For Sheets
        * https://simplemlforsheets.com/
      * Refrescr el google sheets y verificar que aparece la extension instalada
  * Obtener los datos
      * Ir a Kaggle y loguearse : https://www.kaggle.com/
      * Ir al dataset : https://www.kaggle.com/datasets/meeratif/titanic
      * Descargar el DataSet
          * Descarga un archivo que se llama achived.zip
          * Extraemos un test.csv
      * Importar el archivo test.csv en el google sheets
          * File -> Import -> Upload -> (Elijo el archivo test.csv) -> Reemplazar hoja actual
  * Preparar los datos
      * Columna Age -> Format -> Number -> Number
      * Lo mismo para la columna Fare
