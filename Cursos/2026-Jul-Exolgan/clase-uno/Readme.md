# Clase Uno - 15 de Julio del 2026

# Roadmap

* Modulo 1 : Large Language Models
  * Funcionamiento de los LLM
  * Focalizarnos en Copilot
  * Que es un modelo de lenguaje (y como funciona)
  * Como personalizar la IA
  * Modelos Propietarios y Modelos Open Source
  * Elegir el modelo adecuado para la tarea en cuestion
* Madulo 2 : Prompt Engineering
  * Prompt
  * Tecnicas para obtener respeustas mas efectivas de la IA
  * Como utiliza la IA el contexto de la informacion
* Modulo 3 : Herramientas y Productividad
  * Generar Presentaciones
  * Generar Videos institucionales
  * Texto-A-Voz / Voz-A-Texto
  * (Lo vamos viendo transversalmente)
* Modulo 4 : IA Generativa Creativa/ Multimedia
  * Generacion de Videos
  * Generacion de Imagenes
  * Generacion de Audios/canciones
* Modulo 5 
  * IA Tradicional : Analisis de datos
  * Agentes
    * Agentes Preconstruidos
      * Ejemplos: Agentes Analista
    * Construir nuestro agente
  * Uso cororativo de la IA (Transversalmente)
    * Buenas practicas
    * Privacidad de datos y manejo de datos sensibles
    * Riesgos
    * Groundig (Anclar la respuesta de la IA en fuentes verificables)
    * Alucinaciones

---

# Conociendonos

* Usan Copilot
* Legales -> Asistencia en la lectura de documentos legales
* Desarrollo de Agente para legales
* Alfabetizar en IA

--

# Large Language Models (LLM)

* Propietarios
   * Copilot
      * URL : https://www.office.com/
      * Microsoft
      * No es un modelo propiamente dicho sino que es una pasarela a distitos modelos
   * ChatGPT
     * URL : https://chatgpt.com/
     * OpenAI
     * CEO : Sam Altman
   * Gemini
      * URL : https://gemini.google.com/
      * Google
      * Ventana de contexto ampliada a 1M tokens
   * Claude
     * URL : https://claude.ai/
     * Anthropic
   * Grok
     * URL : https://grok.com/
     * X (ex twitter)
     * El de Elon Musk
* Open Source
   * Se pueden descargar y utilizar localmente con una buena placa de video
   * Americanos
     * Familia Llama
       * Estan disponibles en Whatsapp
   * Chinos
     * DeepSeek
        * https://chat.deepseek.com/
     * Qwen
        * https://chat.qwen.ai/
   * Europeos
     * Mistral
        * https://chat.mistral.ai/chat

---

## Personalizacion

### Personalizacion de Copilot

* Entrar a Office.com
* Arriba a la derecha (...) -> Configuracion del Chat -> Personalizacion -> Instrucciones Personalizadas
* Me permite influir en el System Prompt :  en el tono  y la forma de responder

```
Quiero que me respondas en poesia. 
Tus repuestas siempre tienen que ser un poema con rimas.
Tiene que tener metadofas y una caliad literaria alta.
Que cada respuesta tuya sea un poema que me deslumbre
No se aceptan respuestas que no sean poemas.
```

* Luego le pregunto

```
Investigame y hablame de la empresa Exolgan
```

* Y me responde

```
En Dock Sud alza su puerto como un faro colosal,  
donde el río y el comercio tejen su ritual.  
**Exolgan** es su nombre, gigante del litoral,  
una puerta de contenedores en constante movimiento naval. [\[exolgan.itl.com.ar\]](https://exolgan.itl.com.ar/), [\[ar.linkedin.com\]](https://ar.linkedin.com/company/exolgan-container-terminal)

Sobre tierras de Avellaneda, junto al Plata señorial,  
opera la terminal de contenedores más importante de Argentina según su presentación institucional.  
La empresa indica que concentra más del 40% del volumen de contenedores del Puerto de Buenos Aires,  
como un corazón de acero que impulsa el comercio nacional. [\[exolgan.itl.com.ar\]](https://exolgan.itl.com.ar/), [\[exolgan.itl.com.ar\]](https://exolgan.itl.com.ar/?lang=en)

Pertenece al grupo **ITL (International Trade Logistics)**,  
un entramado de compañías de espíritu logístico y estratégico.  
Su propuesta integra servicios portuarios, depósitos, transporte ferroviario y soluciones de importación y exportación,  
como un gran tablero donde cada pieza encuentra su ubicación. [\[exolgan.itl.com.ar\]](https://exolgan.itl.com.ar/), [\[globalports.com.ar\]](https://www.globalports.com.ar/business-directory/exolgan-itl/)

La empresa destaca la tecnología como parte de su identidad,  
desarrollando sistemas para seguir operaciones en tiempo real con claridad.  
También resalta la innovación, la infraestructura y la seguridad como pilares esenciales,  
cual brújulas que orientan sus recorridos comerciales. [\[exolgan.itl.com.ar\]](https://exolgan.itl.com.ar/), [\[exolgan.itl.com.ar\]](https://exolgan.itl.com.ar/?lang=en)

En los últimos años anunció un ambicioso plan de inversión de **US$ 180 millones**,  
destinado a modernizar la terminal y prepararla para buques de mayor dimensión.  
Entre las mejoras informadas se encuentran nuevas posiciones para contenedores refrigerados, ampliaciones de acceso y equipamiento avanzado,  
como si forjara un puerto del mañana sobre el horizonte cotidiano. [\[tradenews.com.ar\]](https://tradenews.com.ar/exolgan-informo-avances-en-su-plan-de-inversion-por-180-millones-de-dolares/)

Si lo miramos desde la economía argentina,  
Exolgan es más que una empresa portuaria.  
Es una bisagra entre fábricas, campos y mercados lejanos,  
un puente de metal donde cada contenedor cuenta una historia. [\[exolgan.itl.com.ar\]](https://exolgan.itl.com.ar/), [\[ar.linkedin.com\]](https://ar.linkedin.com/company/exolgan-container-terminal)

Y así termina este retrato, con aroma a mar y sal,  
de una firma que mueve mercancías en un engranaje global.  
Como un río que nunca duerme bajo la luna austral,  
Exolgan acompasa el pulso del comercio nacional. 🌊🚢📦

```

* Algunos ejemplos de Instrucciones Personalizadas
  * Cuando necesito minimizar las alucinaciones
     * https://github.com/estebancalabria/Intro-Ia/blob/main/Large%20Language%20Models/instrucciones-personalizadas/protocolo-verdad.md
  * PAra que sea mas critico y analitico, no tan condescendiente
     * https://github.com/estebancalabria/Intro-Ia/blob/main/Large%20Language%20Models/instrucciones-personalizadas/asistente-analitico.md

### Personalizacion en otros LLM

* ChatGPT
  * Tambien tiene lo mismo
  * (Nombre de usuario abajo a la izquierda) ---> Personalizacion --> Instrucciones PErsonalizadas
* Claude
  * Tambien lo mismo
  * (Nombre de usuario abajo a la izquierda) ---> Configuracion --> Instrucciones Para Claude
* Gemini
 * Tambien lo mismo
 * (Ruediga abajo a la izquierda) -> Personal Intelligence -> "Instructions for Gemini"
* ...

---

## Memoria

* Los LLM tienen una base interna por usuario donde "recuerdan" datos espcificos de la persona con la que estan hablando

* ChatGPT

'''
En base a la informacion que tengas de mi, haceme un roast
'''

* Copilot
  * Como es corporativo, te censura el roast, pero le puedo preguntar algo mas formal

```
En base a la informacion que tengas de mi, haceme un informe de mi perfil para RRHH
```

# Glosario

* Prompt : Instrucciones que uno le da al LLM para generar una respuesta
* System Prompt : Instruccion oculta que define la personalidad y el tono con el que  me responde el LLM
   * Es el responsable que los LLM sean tan amables y condescendientes
* Tamanio del Contexto : Longitud de la coversacion
* Alucinacion : Cuando la IA genera una respuesta que puede incluso parecer que es real pero esta inventada

# Proxima Clase

> Vamos a seguir hablando de la memoria, ver que cosas los LLM saben de mi y como controlarlo
