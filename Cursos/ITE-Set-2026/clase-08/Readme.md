# Clase Ocho - 7 de Octubre del 2026

# Repaso

* Automatizacion
  * Herramientas
    * Make
    * N8n
  * Make
    * Automatizacion sin IA
    * Automaticacion con IA
* Consumir modelos por API Key
* IA desde Planillas de calculo
  * Excel
    * Copilot para Excel
    * Requiere licencia
  * Google Sheets
    * Gemini para google sheets
    * Ia por medio de una extension tipo SheetGPT

---
   
# IA Tradicional

* LA IA genreativa se encarga de crear contenido nuevo.
* La IA tradicional (Machine Learning) se encarga en Analizar Datos y hacer predicciones
  * Regresion
    * Predecir el valor a futuro de una accion
  * Clasificacion
    * Determinar si un cliente es potencial comprador, Tal vez, no compra
  * Deteccin de anomalias
    * Detectar productos defectuosos en una linea de produccio

* REcurso por excelencia para aprender ciencia de datos
  * https://www.kaggle.com/
  * Aqui a obtener el dataset

## Proceso de ML

<img width="408" height="413" alt="image" src="https://github.com/user-attachments/assets/043da375-ef9f-4198-8a48-7efb5090b373" />


## Setup

* Loguearse en Kaggle
* Crear una planilla de google Sheets vacia (no excel)
  * Instalar una extension de google sheets
    * https://simplemlforsheets.com/
    * https://workspace.google.com/marketplace/app/simple_ml_for_sheets/685936641092
  * Verificar en la planilla que la extension este instalada (puede requerir refrescar la planilla)
 
<img width="864" height="299" alt="image" src="https://github.com/user-attachments/assets/5ad93b34-bfea-4080-b675-7e51f12131a7" />

## Obener el Dataset

* Vamos a buscar el dataset de titanic y descargarlo
  * https://www.kaggle.com/datasets/brendan45774/test-file
  * Le ponen arriba a la derecha "Download" y en la ventana emergente "Donwloa dataset as Zip"
  * Lo descomprimo y me queda un archivo llamado tested.csv

* Importar en el google sheets

## Preparar los datos

* Entender el problema
  * Lo que vamos a querer predecir es si dadas las caracteriscas del pasajero se salvaria o no en el titanic (Survived)
  * Problema de Clasificacion
* Elegir las columnas con las que vamos a trabajar
  * Label / Catetgoria:
    * Survived
  * Features:
    * PClass
    * Sex
    * Age
    * SibSp
    * Parch
    * Fare
    * Embarqued
  * No nos interesan:
    * PasengerID
    * Name
    * Ticket
    * Cabin
* Convertir todas columnas en valores numericos
  * Los modelos de IA tradicional no trabajan bien con columnas alfanumericas salvo que sean categricas
      * Masculino / Femenino  -> Categorica -> OK
      * Descripcion del producto -> Descriptiva -> No sire
    * Para Age hacer format.. number..number
    * Para Fare hacer format...number...number

<img width="501" height="137" alt="image" src="https://github.com/user-attachments/assets/74575865-1532-4e59-b020-a7beea754bfb" />

* Duplicar e libro para tener una copia de los datos originales

## Separar los datos de prueba y entrenamiento

* PAra hacerl en excel borro el contenido de la columna surivides de la fila 2 - 30 -> Datos de Prueba
* El resto de los datos (De la 31 al final) -> Datos de entrenamiento

## Entrenar y probar un modelo

* Extensiones... Simple ML For Sheets ... Start... Predict missing values

<img width="254" height="353" alt="image" src="https://github.com/user-attachments/assets/1743f3cf-713e-4936-9e45-9d8ce0d9d2ad" />

## Explicar el modelo

* Ir a explain model
 * Vemos que la variable mas importante es sex


---
Break hasta y 30
---


# Agentes

* LLM
  * Solo genera texto en base a su entrenamiento
* Agente
 * LLM + Esteroides
 * LLM + Capacidad de consultar fuentes de conocimiento + Capacidad de usar herramientas
 * Capacidad de accion mediante sus herramientas
    * Un ejemplo de herrmienta es la busqueda web
 * Capacidad de Consutar documentacion especificas
 * System prompt (instrucciones personalizadas) epecializadas para la tarea para lo que fue concebido
   * En general LLM -> Uso General, Agente -> Objetivo especifico

## Gemini Notebook (Notebook LM)

* URL
  * https://notebook.google.com/
* Caracteristica
  * Reunir una fuente de informacion para poder tener un chatbot expecializado en esa fuente de informacion
  * Poder generar material audiovisual a partir de esa informacion
  * Ideal para estudiantes y manejar proyectos con informacion relacionada en empresas!
* Enunciado
  * Vamos a armar un notebooklm con toda la informacion/aputes que fuimos tomando en el curso
    
