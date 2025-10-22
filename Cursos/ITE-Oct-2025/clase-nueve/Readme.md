# Clase Nueve - 22 de Octubre del 2025

# Repaso 

* Machine Learning
  * Teoria : https://www.instagram.com/p/C1ntRrRswAu/?img_index=1
  * Web Para Aprender ML : https://www.kaggle.com/
  * Google Sheets : sheets.google.com
  * Simple ML For sheets : https://simplemlforsheets.com/
        * Funcionaba bien hasta datasets de 1 millon de Elementos
  * Google Colab : colab.google.com  
  * Casos de Uso
       * Clasificacion
           * Ejemplo del titanic
           * Ejemplo de Algoritmo : Gradineng Bootsted Trees
       * Regresion
           * Predecir el precio de una accion
       * Deteccion de Anomalias
* Uso de la IA en planillas de Calculos
  * Extension que llama : https://www.sheetgpt.ai/
  * Alternativas : https://gptforwork.com/
  * =GPT o GPTLIST("..prompt...")
  * Funcion propia
    * En Google Sheets se probgrma por medio de AppScript
    * Tutorial de como hacerlo : https://www.instagram.com/p/C9dWVhYRhrs/?img_index=1
    * Requiere una api key como la de Groq

# Agentes

* Agentes basado ChatBot
   * ChatGPT + (alguna de estas capacidades
      * Capacidad de Interactuar con el mundo exterior con herrameintas
      * Capacidad de ejecutar Codigo
      * Capacidad de Consultar una base de datos 
* Agentes Autonomos
      * Se ejecutan a partir de trigger (respondiendo a un estimulo o segun un schedule)
  
# Automatizacion con IA

## Teoria

> https://www.instagram.com/p/DIPbzoPOS6v/?img_index=1

Enfoques:
* Desarrollarlas en python (o cualquier lenguaje de programacion)
* Herramientas No-Code

Relacion Automatizacion con Agentes
* Las automatizaciones entran en la categoria de Agentes Autonomos
* Una automatizacion incluye una forma de implementar un agente
* Tambien puedo utilizar las herramientas de automatizacio para implementar un agente chatbot

## Herraminentas

* Make : https://www.make.com/en  --> Es la opcion que vamos a ver nosotros
* N8n : https://n8n.io/   --->  (Open Source, se puede ejecutar localmente, la rompe hoy en dia)
* Zappier : https://zapier.com/  ---> Fue por mucho tiempo la mas popular de todas
* ITTTF : https://ifttt.com/ (Sencilla funciona desde el celu)
* **NOVEDAD : Agent builder : https://platform.openai.com/agent-builder**
* Para domotica y automizar el hogar (IOT) por eventos : https://nodered.org/

## Laboratorio Make 

* Vamos a abrir tres solapas en el google Chrome
   * Make
   * Un documento de google Sheets
       * Tres Columnas: Evento, Inicio, Fin
       * Definir la columna Inicio y Fin de tipo Fecha y Hora (Date and Time) (Prestar atencion al formato)
   * El calendario de Google
* Aegurarse que el calendario y el google sheets usen la misma cuenta y tomar nota de que cuenta se esta utilizando
* Ir a make y crear un escenario nuevo
    * Al Escenario lo voy a llamar "Sheets-Groq-Calendar"
    * Agregar al escenario el Trigger de la herramienta "Google Sheets" llamado "Watch new Rows"
    * Conectarme con la cuenta de gooogle que tiene la hoja de calculo que voy a utilizar
    * Completar los campos eligiendo la hoja en el dialogo que aparece en la herramienta
    * Probar la herramienta
        * Agregar una fila nueva al google Sheets
        * Ejecutar la automatizacion a ver si toma la nueva fila (Run Once abajo
        * Pretar atencion a los formatos de fecha utilizados
        * Verificar que al ejecutar dos veces no vuelve a tomar la misma fila
    * Agregar la accion "Create Event" de "Google Calendar" en + al lado del trigger
       * Puedo volver a utilizar la conexion a Google que tenia antes
       * Vincular el nombre el evento, el start date y el end date con variables del paso anterior
    * Probar integracion
       * Agregar una fila nueva a nuestra planilla
       * Ejecutar mi automatizacion
       * Mirar mi calendario si se agrego el evento

# Chatbots
