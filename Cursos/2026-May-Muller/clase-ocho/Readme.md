# Clase Ocho - 14 de Julio del 2026

# Repaso

* IA Generativa Multimedia
  * Tips
    * Prompts en Ingles
  * Generacion de Imagenes
    * Usando un LLM multimodal
      * NannoBannana en Gemini
      * GPTImage en ChatGPT
    * Leonardo
      * Generador de Imagenes de Cabecera.
      * Pasarela a varios modelos
      * 150 creditos diarios
    * Ideogram
      * Generacion de Imagenes con Texto
  * Generacion de Video
    * Pollo
      * Pasarela a modelos de Video
      * Muy usado por los creadores de contenido
      * Tiene motion control
    * Qwen
      * Opcion Gratuita rapida
      * Antes usabamos grok pero ahora es pago
    * Pika.art
      * Generacion de efectos 
  * Generacion de Canciones
    * Suno

---

# Obsequio del profe

* Pasarela de modelos de IA de la FIUBA
  * https://passportai.app/

# Labs Google

* URL
  * https://labs.google/
* Caracteristicas
  * Proyectos experimentales que llevan adelante los empleados de Google
  * Muchos de estos proyectos si tienen exito se transforman en aplicaciones mainstream dentro del ecosistema de google

---
# IA Generativa Mutlimedia

## Pixverse

* URL
  * https://pixverse.ai/es
* Caracteristica
  * Es una pasarella para modelos de generacion de Video\
  * Tiene un modelo propio pixverse

## Google Flow

* URL
  * https://labs.google/fx/tools/flow
* Caracteristicas
  * Hoy x hoy te permite generar imagenes ilimitadas con NannoBannana
  * Los creditos se renuevan diariamente
* Forma de Trabajo
  * Primero creo un personaje
  * Luego en el prompt referencio con el @ a mi personaje
* Puntaje
  * 8.5/10

---

# Agente

## Agente Conversacional y un LLM

* LLM
  * Genera texto a partir de una entrada
  * No tiene informacion con el mundo exterior
  * No tiene acceso a ninguna otra informacion mas alla de la que fue entrenado
* Agentes Conversacionales
  * LLM
  * System prompt personalizdo
    * El agente no es de uso general sino que cumple un objetivo concreto
    * El system prompt del agente define su objetivo y como tiene que comportarse
  * Capacida de consultar ciertas fuente de imformacion
    * Grouiding a las respuesta
    * RAG (Retrival augmented Generation) : Busqeudas semanticas en esas fuentes de informacion
  * Capacidad de llamar herramientas
    * Permiten al agente interactuar con el mundo exterior
    * Ejemplo : Busqueda web
    * Ejemplo : Gemini y su capacidad de interactuar con el calendario de Google
  * Orquestador

### Ejemplo : Agente de Reserva de turno

* System Prompt
  * "Eres un asistente de reserva de turmos del doctor Juan Perez que es un odontologo...
  * ...
  * Si te hablan de algo que no es reserva de turnos rechaza amablemente la solicitud"
* Dataset (RAG)
  * Documento con los tratamientos que hace el doctor
  * Documento con la disponibilidad del doctor
  * Documento con los listados de las obras sociales conlas que trabajar
  * Documeno con los requerimientos para atenderse segun la obra social
* Tools
  * Herramienta para reservar el turno y anotarlo en el google calendar
  * Herramienta para consultar la disponibilidad del doctor
* Orquestador
* LLM
  * Elegimos un modelo que sea adecuado a la tarea y no necesariamente sea el mas caro

---

# NotebookLM

* URL
  * https://notebooklm.google.com/
* Caracteristicas
  * Es un agente que tiene la posibilidad de generar una base de conocimiento
  * Tiene herramientas para generar documentacion audiovisual sobre esa base e conocimiento
* Base de Conocimiento
  * https://raw.githubusercontent.com/estebancalabria/Intro-Ia/refs/heads/main/Cursos/2026-May-Muller/clase-uno/Readme.md
  * https://raw.githubusercontent.com/estebancalabria/Intro-Ia/refs/heads/main/Cursos/2026-May-Muller/clase-dos/Readme.md
  * https://raw.githubusercontent.com/estebancalabria/Intro-Ia/refs/heads/main/Cursos/2026-May-Muller/clase-tres/Readme.md
  * https://raw.githubusercontent.com/estebancalabria/Intro-Ia/refs/heads/main/Cursos/2026-May-Muller/clase-cuatro/Readme.md
  * https://raw.githubusercontent.com/estebancalabria/Intro-Ia/refs/heads/main/Cursos/2026-May-Muller/clase-cinco/Readme.md
  * https://raw.githubusercontent.com/estebancalabria/Intro-Ia/refs/heads/main/Cursos/2026-May-Muller/clase-seis/Readme.md
  * https://raw.githubusercontent.com/estebancalabria/Intro-Ia/refs/heads/main/Cursos/2026-May-Muller/clase-siete/Readme.md
  * https://raw.githubusercontent.com/estebancalabria/Intro-Ia/refs/heads/main/Cursos/2026-May-Muller/clase-ocho/Readme.md
