# Clase Seis - 19 de Noviembre del 2026

# Repaso

* Videos Instutucionales
  * HeyGen
* Interprete de Codigo dentro de los LLM
    * Para hacer graficos con MAtPlotLib
    * Para calculos matematicos sobre todo sobre planillas de calculo
* Automatizacion (Sin IA)
  * Herrientas
      * Zappier
      * N8n
        * Estandar Open Source
      * Make
      * PowerAutomate
  *  Conceptos comunes
    *  Trigger
    *  Integracion con herramientas de terceros
    *  No-Code / Low-Code
  * Ejemplo en Make
      * Pasar de Google Calendar a Sheets

---

# Recomendacion

* App de Colegas
  * https://passportai.app/
  * Te permite usar muchas herramientas en un solo lugar
  * Aprovechar a usarle los creditos gratuitos

# Larger Languge Models

* Cuando en LMStudio o en donde figure el nombre del modelo muchas veces van a ver que los modelos tienen [Nombre Modelo]-XXX b
    * Ej 20b, 120b 
    * El b es la candida de parametros -> 30b seria 30 billones de parametros
    * Esto nos habla del tamaño del modelo
    * Son la cantidad de parametos / conexiones entre neuronas del modelo
    * Los LLM son redes neuronales que emulan el funcionamiento del cerebro : neuronas y conexiones
        * Cuanto mas parametros es mas grande el modelo
    * Mas parametros -> Mayor capacidad de computo necesaria -> MAs tiempo para generar respuesta -> Mas caro el token

* Pueden revisar
  * https://www.instagram.com/p/DaV3CEPFXkF/?img_index=1
  * Obligado si pasan dejar un MG

# Integrar al IA

* En general vimos que cada modelo de lenguaje tiene un web particular para interacturar con el

* Si queremos integrar una solucion (automatizacion, aplicaion, un chatbot) con algun modelo de lenguaje (LLM)
  * Descar el modelo localmente
  * Consumir el modelo online mediante una api key
 
* API Key
    * API (Aplication Program Interface) : Interfaz no visual que permite consumir algun servicio
    * KEY (Clave que da acceso a ese servicio)
 
* Los proveedores de IA tienen dos web
    * Usuario Final
    * Desarrollador
    * OpenAI
        * Usuario Final : https://chatgpt.com/
        * Desarrollador : https://platform.openai.com/home
        * Api Key : https://platform.openai.com/api-keys
    * Claude
        * Usuario Final : https://claude.ai/
        * Desarollador : https://platform.claude.com/
        * Api Key :
    * Gemini
        * Usuario Final : https://gemini.google.com/
        * Desarrlador : https://aistudio.google.com/

> [!NOTE]
> Lamentablemente el uso de la api key es generalmente pago 

* Pero podemos usar un motor de inferencia
    * Groq (conq)
        * https://groq.com/
        * Usuario Final : https://chat.groq.com/
        * Desarrollador : https://console.groq.com/
        * Api Key : https://console.groq.com/keys
          
> [!NOTE]
> Vamos  a guardar la api key en un lugar seguro y no compartimos con nadie. Por lo general la api key se muestra una sola vez.  

* Vamos a usar nuestra API Key
    * https://cbsnagur.github.io/byok-chat/
        * Base URL : https://api.groq.com/openai/v1/

---

# Automatizacion con IA
