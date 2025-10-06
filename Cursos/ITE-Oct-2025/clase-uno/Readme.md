# Clase Uno - 6 de Octubre del 2025

## Requisitos y recomendaciones

* Tener una de Cuenta de Google
* **Recomendacion** : Crear una cuenta nueva de google para probar las herramienta
* * **Recomendacion** : Crear una cuenta de Github

## Resumen de Los temas

Roadmap : https://www.instagram.com/p/C9LE2JRx0SJ/?img_index=1

* LLM (ChatGPT y Altenativas) : https://www.instagram.com/p/DKhQrTvuFcw/?img_index=4
    * Prompt Engineering
    * Invocar un LLM desde python
    * Como ejecutar un LLM localmente
* Modelos Propietarios Vs Modelos Open Source
* Text to Speech y Speech to Text
  * Herramientas de IA para reuniones Online
* IA en la oficina
* IA Generativa Multimedia
  * Artistico
    * Imagenes
    * Videos
    * Audio
  * Profesional
    * Videos Institucionales
    * Presentaciones
    * Disenio de Marca
  * RedesSocial
* Herramientas de IA
* Automatizacion
* Machine Learning
* Agentes y Chatbots
* Etica e IA lo que es LA IA  : https://www.instagram.com/p/DOqu-k8Dvfb/?img_index=1
* Ai-900 : Azure AI Fundamentas (Las ultimas 5 horas) : https://www.instagram.com/mct.esteban.calabria/p/DDs51pdOBI6/
* Extra : IA para desarrollo 
  

## Definiciones

* LLM , Modelo de Lenguaje Grande : Una red neuronal enorme de tipo deep learning que se entreno para genenerar lenguaje
  
* Prompt : La instruccion que uno le da a un modelo de Lenguaje para que de una respuesta
* Prompt Engineering : Estudia la forma de redactar prompts para obtener una respuesta mas efectiva del LLM
  
* System prompt : Un prompt base o raiz que determina la personalida y la forma de responder que tienen los modelos de lenguaje. Por lo general el system prompt lo define el propietario del modelo y no lo podemos conocer (es privado) pero algunos modelos como ChatGPT permiten cierta parametrizacio
   * Cuando generas tu propio chatbot generalmente desde python lo podes cambiar...
  
* GPU : Los procesadores Graficos que tradicionalmente se utiliban para juegos y hoy en dia cumplen un rol fundamentan en todo lo que es entrenar y ejecutar modelos de Inteligencia Artificial
  * NVIDIA : Es la empresa principal que fabrica los GPU
    
* JailBreak de un Modelo : Es ejecutar un prompt que permita romper la censura que traen los modelo de lenguaje

## Mercado

* Empresas
  * OpenAI : Empresa que hizo ChatGPT
  * Anthropic : Empresa que hizo el LLM Claude competencia directa de ChatGPT
  * Meta : Empresa que hizo facebook se especializa en modelo de lenguaje Open Souce la familia LLama

## Modelos de Lenguaje

* Modelos de Lenguaje Propietarios
    * ChatGPT : https://chatgpt.com/
        * Ideal para conversaciones humanas
        * Tiene memoria de quien la usa : Sabe cosas sobre uno
            * Ir a Personalizacion...Memoria...
        * Puede ser bastante amigable e informal y hasta sarcastico
        * Es bastante personalizable su personalidad (mas que otros llm)
           * En el menu de personalizacion donde esta la memoria podes influir sobre el System Prompt de Chatgpt en la parte de Instrucciones Personalizadas
    * Gemini : https://gemini.google.com/app
       * Se especializa en conocimiento Factico porque busca envententualmente reemplazar el buscador
          * Por ejemplo para hacer una investigacion sobre la revolucion francesa
       * Buena integracion con las herramientas de Google
          * Integracion con Calendar, Flights, Hotels,
       * Generacion de Imagenes con Nano Banana (es uno de los modelos de generacion de imagenes mas avanazdos
       * En general funcionan mucho mucho mejor en ingles
    * Claude : https://claude.ai/new
       * Se destaca en la generacion de artefactos y previsualizaciones
       * Destaca mucho para la programacion
    * Grok : https://grok.com/
* Modelo de Lenguaje Open Source
    * DeepSeek : https://www.deepseek.com/en
    * Qwen : https://chat.qwen.ai/
    * Modelos Familia Llama (Los primero exponentes del Open Source hechos por meta)
        * Si en una conversacion de wsap escribp @meta le puedo preguntar a la Ia de Mark Zuckemberg
        * Los modelos Open Source se pueden ejecutar desde la web de Groq (con q) que es un motor de inferencia : https://chat.groq.com/

## Ejemplos

### ChatGPT

- #### Uso de memoria en ChatGPT
Incluir el siguiente prompt
```
Basado en tu memoria y conocimiento sobre mi quiero que me hagas un roast
```

- #### Uso de Instrucciones personalizadas
En el menu de instrucciones personalizadas poner:
```
Eres mala onda. Te molesta todo. Hasta eres casi ofensivo con quien con tu interlocutor
```
Se puede buscar en Internet ejemplos de Instrucciones peronalizadas pero lo mas comun es ir experimentando y armando la propia

### Gemini

- #### Integracion con Google Calendar

  Puedo crear eventos en mi calendario de google con Gemini
  ```
  Me podes crear un evento hoy a las 16:00 que sea ir a entrenar?
  ```

- #### Integracion con Google Flights y Google Calendar

Uso este prompt
```
Queiro viajar la semana que viene de Buenos Aires a Madrid y quedarme una semana. Me gustaria que me hagas una planificcacion y un presupuesto usando Google Flights y Google Hotels.
```

### Claude

- #### Generacion de artefactos

Probamos con el siguiente prompt
```
Generarme un artefacto para una web completa que sea el juego pong en html y javascript. El jugador de la derecha se mueve con las teclas de cursor y el de la izquierda con la a y la z
```
Me Genero esto:
> https://claude.ai/public/artifacts/a9711f6c-a8e8-4ac2-a96f-c4d2e6fe533a


## Casos de uso para modelo de lenguaje

Infinitos pero podemos detacar
* Corregir y redactar mejor correos
  * Ojo con redactar todo el correo con Ia y ni leerlo
* Programar
* Dudas Tecnicas
* Resumir Texto (pdfs)
* Generar Ideas Nuevas
* Escribir informes Tecnicos
* 

## Tips uso de LLMS

* Iniciar una nueva conversacion cuando cambio de Tema
