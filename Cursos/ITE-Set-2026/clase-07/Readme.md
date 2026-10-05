# Clase Siete - 5 de Octubre del 2026

# Repaso

* IA Generativa Creativa
  * Imagenes
    * Modelos
      * Nannno Bannana
      * Flux (Open Source)
    * Herrmientas
      * Leonardo
      * NanoBannana desde Gemini o Google Flow
      * Hugging Face Spaces
      * Ideogram
      * Microsoft Designer
        * Simil a Canva, generacion y  edicion
  * Videos
    * Herramientas
      * Pollo.ai
      * Pizverse
      * Qwen Video (Genracion basada en chatbot
      * ArenaAI (Gratis)
      * Copaginacion de Videos
        * Capcut
  * Cambiones
    * Herramientas
      * Suno
      * Udio (teniendo suno no convencio)
     
---

# Automatizacion con IA

* PPT del Profe
  * https://www.instagram.com/p/DIPbzoPOS6v/?img_index=1
* Formas de Automatizar
    * Tradicionalmente en Python
    * Herramientas No Code
* Metodologia
  * Automatizar herramientas de uso cotidiano (Whatsap, mail, teams, excel, sharepaint, calendar)
      * Me llega un correo, lo valido con la IA y si cumple ciertas caracteristicas creo un documento en sharepoint
  * Trigger
      * Una accion o evento que ocurre en alguna de las herramientas que comienza un flujo de automatizacion
      * Flujo, aka pipieline, son una serie de pasos como una receta o un algoritmo que ocurren automatimanente ante ese trigger
      * IA la potencia un monton la Automatizacion

## No code

* Es una tendencia hoy en dia que incrementa el uso de las herramientas no code
  * En microsoft tenemos Power Platform
  * App Inventor
    * https://apps.apple.com/es/app/mit-app-inventor/id1422709355
   
## Make

* https://www.make.com/
* Mirar los templates en
    * https://<xxxx>.make.com/templates
* 

### Primero una automatizacion SIN IA

* Enunciado
  * Vamos a generar una automatizacion donde completamos una planilla de google sheets (o recibimos un mail) y autmaticamente generamos la entrada en Google Calendar

* Setup
  * 3 Solapas
    * Make
    * Documento de Google Sheets
    * Calendar Abierto

* Google Sheets
  * Voy a crear un documento nuevo
  * Le voy a dar un nombre significativo
  * Crear tres columnas Evento, Inicio, Fin
  * Tanto al campo Inicio, como Fin poner formato tipo Fecha y Hora

<img width="640" height="396" alt="image" src="https://github.com/user-attachments/assets/3b20bedf-f0ba-4d83-9de9-0e935c5ba33e" />

*  Make
  *  Vamos a crear un escenario nuevo
    *  [Left Navbar] -> Scenarios -> + Create Scenario

* Configurar el Trigger
  * Cuando se ingrese una fila en el google sheets
  * Elijo como triiger Google Sheets
      * Elijo como accion "Watch New Row"
      * Conecto con la cuenta de Google donde tengo el sheet
      * Elegimos el archivo y el libro que vamos a observar

<img width="503" height="323" alt="image" src="https://github.com/user-attachments/assets/138004f0-b988-4118-a5a3-b77fa5a14d33" />

<img width="414" height="198" alt="image" src="https://github.com/user-attachments/assets/826be83a-db34-4e78-a0a2-e18c9e733f27" />

* Probar el Trigger
  * Agregamos una entrada en el google sheet
  * Podemos la formula =NOW() para completar el inicio y el fin, despues copiar valores y modificarlo manualmente
  * Ejecutar el triiger en make con el boton "Run Once"

<img width="547" height="355" alt="image" src="https://github.com/user-attachments/assets/48090db6-6665-4723-ae75-fd272e23e767" />

* Probar que al ejecutar dos veces la fila ya no vuelve a aparecer

* Generar el evento en Calendar
  * Elegimos en el + al lado del trigger para agregar un modulo y elegimos Google Calendar
      * Elegimos la accion "Creat an event"
          * In Detail
          * Primary Calendar
          * Even Name  -> Lo asocio con la variable "Evento" del paso anterio seleccionandola del popup emergente
          * Start Date  -> Lo asocio con la variable "Inicio" del paso anterio seleccionandola del popup emergente
          * End Date  -> Lo asocio con la variable "Fin" del paso anterio seleccionandola del popup emergente

<img width="278" height="373" alt="image" src="https://github.com/user-attachments/assets/ed47bf72-9d1c-4c20-8031-d781b8e133ed" />


* Prueno la automatizacion

> [!NOTE]
> Ojo como Make interpreta las fechas. Si no aparece el evento fijarse como interpreto la fecha tal vez interpreto el mes como el dia y viceversa

---
# BREAK hasta y 30
---

### Incorporar la IA a la automatizacion

#### Api Keys

* Contexto
  * Introducir un modelo tipo ChatGPT en el proceoso
  * Formas de interaccion con un modelo
    * Mediante su interfaz web
    * Mediante APi key (para llamar al modelo desde otras aplicaciones)
      * Es un clave lartga alfanumerica que identifica al usuario cuando quiere usar el modelo de IA desde otra aplicaciob
  * Limitante
    * La api key de modelos propietarios generalmente son pagas y no pemiten prueba gratuita
    * Podes utilizar una api key de un modelo open source (online) utilizando algun motoro de inferencia como Groq
      * https://groq.com/
    * Para el usuario final puede usar groq directamente desde aca
      * https://chat.groq.com/
    * Para el dearrollador
      * https://console.groq.com/
      * Ahi obtenemos la API KEY y la guardamos en un lugar

## Incorporar lo de la API Key en Make

* Agreamos un modulo en el medio de los dos (con boto derecho)
  * Elegimos el modulo de Groq
    * "Create Chat completion"
      * Para configurar la conexion le vamos a poner nuestra api key
      * Prompt
        * Convertime este nombre de evento "{{1.`0`}}" en un nombre de evento gracioso. Devolverme el nombre del evento gracioso sin acotar nada mas

<img width="269" height="440" alt="image" src="https://github.com/user-attachments/assets/12595cb3-2cc6-460e-9d97-99c61ee24145" />

* Modicar el nodo de la generacion del evento en el calendario para que incluya el chiste que nos dio la IA
  * En el event name ahora va la variable result del paso anterior

* Generar el evento en google sheets y probarlo


---
# Break hasta y 20
---

# IA Tradicional
