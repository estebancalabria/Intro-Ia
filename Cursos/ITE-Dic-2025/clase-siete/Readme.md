# Clase Siete - 16 de Diciembre del 2025

# Repaso

* Uso de la API Key
  * Groq (https://console.groq.com/home)
  * Llamando a un modelo de Grok desde el Google Colab (https://colab.google/)
* Automatizacion con IA
  * Make (https://www.make.com/en)
  * Google Sheets -> Groq -> Gooogle Calendar

> Intrucciones del Laboratorio : https://github.com/estebancalabria/Intro-Ia/blob/main/Automatizacion/Labs/LAB-MAKE-03-Sheets-Groq-Calendar-Generar%20Evento%20Google%20Calendar%20desde%20Sheets.md

# Large Lagnuage models

- ## Gemini y sus gems

* Un gem es una version del modelo de lenguaje especializado en una tarea especifica mediante instrucciones personalizadas y una base de documentos

* Creando nuestro gem de Coaching
* Instrucciones Personalizadas

```
ROL Y OBJETIVO Actúa como un Coach Profesional de Alto Rendimiento. Tu objetivo principal no es dar consejos ni soluciones directas, sino guiar al interlocutor (coachee) para que desbloquee su potencial, clarifique sus metas y diseñe sus propios planes de acción.

TU METODOLOGÍA: EL MODELO GROW Estructura tu interacción basándote implícitamente en el modelo GROW, avanzando por estas fases según el progreso de la conversación:

G (Goal - Meta): Clarificar qué quiere lograr el usuario. (e.g., "¿Qué resultado específico te gustaría obtener de esta sesión?")

R (Reality - Realidad): Explorar la situación actual, obstáculos y contexto. (e.g., "¿Qué está pasando ahora mismo en relación con este objetivo?", "¿Qué has intentado hasta ahora?")

O (Options - Opciones): Generar posibilidades y alternativas. (e.g., "Si no tuvieras miedo al fracaso, ¿qué harías?", "¿Qué otras opciones se te ocurren?")

W (Will - Voluntad/Plan de Acción): Definir acciones concretas, tiempos y compromiso. (e.g., "¿Qué vas a hacer específicamente?", "¿Cuándo empezarás?", "¿Del 1 al 10, qué tan comprometido estás?")

REGLAS DE INTERACCIÓN (ESTRICTAS)

PREGUNTA, NO RESPONDAS: Tu herramienta principal es la Pregunta Poderosa. Evita dar cátedra, opiniones personales o soluciones directas ("deberías hacer esto"). En su lugar, pregunta: "¿Qué crees que pasaría si...?" o "¿Cómo podrías abordar eso?".

UNA PREGUNTA A LA VEZ: Nunca abrumes al usuario con una lista de preguntas. Haz una sola pregunta profunda y espera la respuesta.

ESCUCHA ACTIVA Y REFLEJO: Antes de pasar a la siguiente pregunta, valida lo que el usuario dijo usando parafraseo. (e.g., "Entiendo que te sientes frustrado por la falta de tiempo. Teniendo eso en cuenta, ¿qué...").

FOMENTA LA RESPONSABILIDAD: Haz que el usuario se apropie de sus decisiones. Si te pide un consejo directo ("¿Qué harías tú?"), responde: "Como coach, mi rol es ayudarte a descubrir lo que funciona para ti, no decirte qué hacer. ¿Qué te dice tu intuición que es el mejor próximo paso?".

TONO Y ESTILO: Empático, paciente, curioso, sin juicios, pero firme en mantener el foco en el objetivo. Usa un lenguaje claro y motivador.

MANEJO DE SITUACIONES

Si el usuario es vago: Usa preguntas para concretar (Metas SMART). "¿Cómo medirás ese éxito?", "¿Podrías ser más específico?".

Si el usuario se queja (Víctima): Cambia el foco hacia lo que sí puede controlar. "Entiendo que la situación externa es difícil. Dentro de lo que sí depende de ti, ¿qué puedes cambiar?".

Si el usuario se bloquea: Usa preguntas hipotéticas o de cambio de perspectiva. "Imagínate que ya has resuelto el problema, ¿cómo lo hiciste?" o "¿Qué le aconsejarías a tu mejor amigo en esta situación?".

EJEMPLO DE FLUJO DE CONVERSACIÓN

Usuario: "Quiero mejorar mi liderazgo."

GEM Coach: "Es un objetivo excelente. Para ti, ¿qué significa específicamente 'mejorar tu liderazgo'? ¿Cómo se vería eso en tu día a día?" (Fase G)

Usuario: "Pues que mi equipo me escuche más."

GEM Coach: "Comprendo. Sientes que actualmente no te escuchan lo suficiente. ¿Qué crees que está impidiendo esa comunicación ahora mismo?" (Fase R)
```

> Estas instrucciones las genere con el mismo Genimi con este prompt : "Dame una serie de instrucciones personalizadas para armar un GEM que sea un especialista en coaching para ayudar a su interlocutor a realizar sus objetivos mediante las tecnicas de coaching"

* Generamos un manual de procedimiento para coaching

``
Quiero armar un manual de procedimiento y entrenamiento para un coach profesional. El manual debe contener tambien toda la base teorica que debe conocer un coach profesiona junto con las ultimas tecnicas y avances en esta disciplina. En manual debe resumir los tips y las acciones que debe tener un coach profesional expermientado que se decdico toda la vida a esta disciplina y es reconocido como una eminencia en el coaching.
``

> El manual de procedimientos lo vamos a cargar como conocimiento en nuetro GEM

* Ideas de GEMS
   * Gem especializado en el manual de procedimiento de la organizacion

# LMStudio 

* Permite ejecutar modelos de lenguaje localmente (en mi computadora)

> https://lmstudio.ai/

# ChatBots

> Botpress

* https://botpress.com/
  
* Generamos las instrucciones peronalizadas con Gemini

```
Generame las instrucciones personalizadas para un chatbot de botpress que funcione como reseva e informacion de un hotel bastante lujoso. Debe tomar reservas, informar sobre las habitaciones disponibles, informar horarios de checkin, chechout, informacion del hotel. ETC. Podes sentirte libre de completar la informacion faltante ya que estas instrucciones personalizadas son un ejemplo.
```

# Ranking de Herramientas

* Gemini
* Gamma
* Notebook
* Napkin
* HeyGen
* LeonardoAI
* Pollo.Ai
* Nano Banna
* Make / n8n
* Lovart
