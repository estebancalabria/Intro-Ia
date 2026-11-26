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
      * DEscargar dataset de https://github.com/estebancalabria/Intro-Ia/blob/main/Cursos/ITE-Nov-2026/clase-nueve/tested.csv
      * Importar el archivo test.csv en el google sheets
          * File -> Import -> Upload -> (Elijo el archivo tested.csv) -> Reemplazar hoja actual
  * Preparar los datos
      * Columna Age -> Format -> Number -> Number
      * Lo mismo para la columna Fare
      * Clasificar columnas
        * Label (Quiero predecir)
          * Survived
        * Features (Columnas que uso para predecir)
          * PClass
          * Sex
          * Age
          * SibSP
          * Parch
          * Fare
          * Embarqued
        * Descartadas
          * PassengerID
          * Name
          * Cabin
            * Muchos valores faltante
          * Ticket
     * Separar datos de prueba y entrenamento
         * Duplicar el libro original (para no perder los datos originales)
         * De la celda 2 a la cenda 30 borrar el conenido de la columna survived
            * Estos van a ser mis datos de prueba
     * Entrenar y evaluar el modelo
         * Extensiones -> SimpleML for Sheets -> Start -> Predict Missing Values
            * Columna con Celda vacia (Label) : Survived
            * Source Columns (Features) : Sacamos PaggenterID, Name, Cabin, Ticket

> [!NOTE]
> Verificamos que el modelo pudo predecir correctamente los que se salvan

---
# BREAK hasta y 25
---

## IA Tradicional y Codificacion

* Esto mismo que hicimos con SimpleML for Sheets lo podemos hacer con el Intrprete de codigo que traen los llm
  * Los mostramos con el agente analista de Copilot que requiere licencia 365
* Si lo quisieramos hacer en una escala masica tendriamos que usar el rescuero de Azure ML
