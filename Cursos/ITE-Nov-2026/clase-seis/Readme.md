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
Break
---

# Automatizacion con IA

* Vamos a agregarle IA al ejemplo de la clase pasada de MAKE
  * Lo que quiero es que ahora la IA me calcule una prioridad para el evento (ALTO, MEDIO, BAJO, DESCONOCIDO) y cuando complete la  planilla de excel le ponga la prioridad calculada
 
* Setup
  * Abrirl el Calendar
  * Crear un xls
  * Loguearnos en make
 
* Creo Escenario nuevo y hacemos lo mismo que la clase pasada

<img width="508" height="245" alt="image" src="https://github.com/user-attachments/assets/bb27b00e-4e83-48fe-8b0b-676720af7e4a" />

* Vamos a agregrle IA
 * Si bien make tiene IA nativa, esta te la cobran. En nuestro caso para abaratar costos y ademas entender nos conviene usar lo de la api key que vimos

* Prompt
```
Quiero que analices el evento de calendar basado en su despcripcion y me devuelvas una prioridad que puede ser ALTA, MEDIA, BAJA o INDETERMINADO.
Los eventos que tienen que ver con ocio, salidas, diversion y entretenimiento tienen que tener prioridad BAJA
Los eventos que tienen que ver con tareaas laborales tienen que tener prioridad MEDIA
Los eventos que tienen que ver con cuestiones de salud tienen que tener prioridad ALTA
Si no podes determinar la prioridad devolver INDETERMINADO
Devolver solamente el valor de la prioridad una sola palabra sin acotar nada mas
LA descripcion del evento dice : 

```


* En el medio de los dos voy a poner un modulo que se llama Groq
  * Si no tenemos una api key la saco de vueta en : https://console.groq.com/keys
  * Agregar un modulo en el medio que sea "Create Chat Completion"

<img width="615" height="449" alt="image" src="https://github.com/user-attachments/assets/d28c1911-03d0-4838-84e2-7e916d5d45be" />

* Modifico el nodoo que agrega la columna a Google Sheets para que complete la prioridad que le devolvio la IA

<img width="657" height="455" alt="image" src="https://github.com/user-attachments/assets/1e3f61ee-645e-4d52-bd57-e6bb9d22c88e" />

* La autmatizacion me queda asi:

<img width="671" height="301" alt="image" src="https://github.com/user-attachments/assets/55f96be2-ba59-4ac2-8fc3-054cfbe9e5aa" />



