# Clase 01 - 21 de Septiembre 2026

# Roadmap

* Modulo 1 : Fundamentos de la IA
    * Como funciona la IA
    * Tipos de IA
        * IA Generativa
        * Machine Learning
    * Impacto de la IA hoy (Riesgos, etica, leyes)

* Modulo 2 : LLM (IA Generativa)
    * Que LLM usamos segun el contexto
    * Prompt Ingeneering

* Modulo 3 : Agentes
    * Chatbots con una mision especifica
    * Chatbots de atencion al publico
    * Tipos de Agentes
        * Agentes Pre consstruidos
        * Agentes propios

* Modulo 4 : Herramientas de IA
    * Herrmientas para potenciar la productividad
    * Generacion de PResentaciones
    * Texto-Voz y Voz a Texto
    * Transcripcion de reuniones
    * Mejorar la visual de  un documento
    * Videos instucionales basados en Avatar

* Modulo 5 : IA Creativa
  * Generacion de Audios
  * Generacion de Imagenes
  * Generacion de Videos
      * Creativos
      * Avatar
  * IA para Disenio Grafico 

* Modulo 6 : Automatizacion
  * Herramientas No Code
  * Panorama general de automatizacion
 
* Modulo 7 : Generacion de Agentes
  * Construccion de agentes propios
  * Desarrollo con IA

* Modulo 8 : AI-900 - Certificacion Oficial De Microsoft

# Requerimiento

* Cuenta de GMail
    * Recomendacion. Sacarse una cuenta de GMail para probar las herramientas del curso asi no reciben correo no deseado de todas las herrameintas que probamos

* Seguir el Profe en Instagram
   * https://www.instagram.com/mct.esteban.calabria/
   * https://www.linkedin.com/in/esteban-calabria-7a44401a/


# Metodologia

* 100x100 practico
* Mini Breaks (1 de 15 o 2 de 10 dependiendo la Clase) 
* Actividades de Preguntas y respuestas

---

# Modulo 1 : Fundamentos IA


## Licenciamiento de la IA

  * Propietarios
      * Solamente se pueden utilizar mediante su portal web o los mecanismos que la empresa que provee el modelo nos da
  * Open Source
      * Muy importante en la privacidad de los datos
      * Los puedo descargar a mi computadora y ejecutarlos localmente en un a pc con una grafica lo suficientemete potente

* Costo de entrenamiento de un llm
   * https://www.instagram.com/p/DKhQrTvuFcw/?img_index=1

## Modelos de Lenguaje

* OpenAI
    * ChatGPT
        * Chat 3.6
        * ChatGPT SOL
        * Chat ASTRA
* Open Source
    * Qwen
        * Qwen 3.7 Plus
        * Qwen 3.8 Max

> [!NOTE]
> Cada modelo es mas adecuado para una tarea especificas. Algunos modelos son mas rapidos, otros razonan mejor, otros son mejores para conversaciones humanas, otros son mejores para tareas tecnucas
> Es improtante saber elegir el modelo adecuado segun la tarea que vamos a realizar

## Funciona la IA

"Hola"  -> (IA) -> "Hola que" -> (IA) -> "Hola que tal"

* LA IA generativa es un modelo predictivo al que le damos una frase y me predice el proximo token (palabra)
* La IA Genera token a token

* En realidad es mas complejo, no se le pasa solo el prompt

(Prompt) + (Memoria) + (System Prompt) + (Instrucciones Personalizadas) + (Llamadas a Herramientas / Busqueda Web) + ...

---

# Caracteristicas LLM

## Memoria

```
En base al conocimiento que tenes de mi, haceme un roast (una gastada)
```

* La memoria siempre se puede editar en las opciones de personalizacion

## Instrucciones personalizadas

* Al igual que se puede administrar la memoria, la IA me permite instrucciones personalizadas

```
Quiero que me respondas en poema. Todo lo que respondes tiene que estar en versito. Todo con rima. Que tu respuesta sea una poesia, llena de metraforas. Una obra de arte literaria
```

* Algunas instrucciones personalizadas son:
   * https://github.com/estebancalabria/Intro-Ia/tree/main/Large%20Language%20Models/instrucciones-personalizadas

# Glosario

* Alucinacion : Cuando la IA da una respuesta en apariencia correcta pero que no lo es
* FOMO : Fear of missing out
  * Los que quieren estar en todos los sitios y no pderderse una
* Token : La unidad minima de texto generado por la IA (en general es una palabra)
    * Para medir la logintud de la entrada
    * Para medir la longitud de la respuesta
    * Como unidad de cobro
* Tokenizacion : Dividir un texto en tokens
* No determinismo : El mismo prompt no siempre da las mismas respuestaws
* Prompt : Instrucciones que le damos a la IA para que genere una respuesta
* System Prompt:
   * Un prompt oculto que le da el fabricante del modelo de lenguaje para definir el tono y la personalidad del mismo
   * Es el responsable que ChatGPT sea tan halagador
* Grounding
   * La ia puede responder solamente basada en su conocimiento y su entrenamient el riesgo de generar una alucinacion es mayor
   * Generar la respuesta de la IA basandose en fuentes verificables
   * En concreto cada parrafo que responde la IA se considera que tien grounding cuando aparece un recuadro gris que dice de donde salio la informacion
   * Muchas veces el gorundig no es algo que esta en la web sino archivos que nosotros les damos a la IA como referencia para que a partir de ellos me arme una repsuesta

<img width="614" height="191" alt="image" src="https://github.com/user-attachments/assets/d62933c7-ee66-44c9-a2a2-d6faa46a9e20" />

> [!NOTE]
> "Si ves que la respuesta de la IA te chirria, hay que pedirle siempre que te aclare y busque fuentes en base a cual justifica la respuesta

# Proxima Clase

* Ver todos los LLM que hay y para que sirve cada uno
