# Clase Nueve - 2 de Diciembre del 2025

# Repaso

* Machine Learning
    * En Google Sheets
    * Simple ML For Sheets
    * https://www.kaggle.com/
* Usar IA en Google Sheets

# Automatizacion con Make

> https://www.instagram.com/p/DIPbzoPOS6v/?img_index=1

* Setup
  * Abrir una Solapa con el Calendario de Google
  * Abrir otra solapa con una planilla de Google Sheets (Ponerle un titulo)
      * Columnas
          * Evento
          * Inicio  (Formato Fecha)
          * Fin     (Formato Fecha)
  * Loguearnos a la herramienta make
          * https://www.make.com/en
* Automatizacion
  * Crear un scenario nuevo
  * Agregar un trigger
    * Google Sheets
      * Watch new Rows
      * Loguearte con tu cuenta de google
        * Conectarte con la hoja de google sheet
        * Choose Where to Start : All
        * Save
  * Probar que ande todo hasta ahora
      * Crear una fila
      * Darle Run Once en make
  * Agregar Modulo Nuevo
      * Google Calendar
      * Create an event
      * Revalidar Autenticacion
      * Elegir Calendario
          * Event Name : Celda A
          * Inicio : Celda B
          * Fin : Celda C
  * Probar que ande todo hasta ahora
      * Crear una fila
      * Darle Run Once en make
  * Scar una API key de GROQ
      * https://console.groq.com/home
  * Agregar un modulo entre las dos acciones que tenemos
    * Groq
    * Create Chat Completion
    * Create A connection
        * Copiarle la API KEY
  * Elegir el modelo
  * En messages agregar uno
  * Como prompt poner
      * Dame una frase graciosa para registrar el evento de calendar llamado {{1.`0`}}. Devolver solamente el nombre del evento gracioso sin acotar nada mas.
      * Deleccionar la celda anterior como parte del prompt
  * Darle Save
  * Actualizar el nodo del calendario
    * Cambiar el Event Name por el Result de Groq
  * Darle Save
 * Probar que ande todo hasta ahora
      * Crear una fila
      * Darle Run Once en make

* Puntaje 10 / 10

# Chatbots

> https://botpress.com/

* Para poder desplegar chatbots Facilmente


