# Clase Dos - 17 de Julio 2026

# Repaso

* Large Language Models
  * Funcionalidades para sacarles el maximo provecho
    * Instrucciones Personalizadas
    * Memoria
  * Propietarios
    * Claude
    * ChatGPT
    * Gemini
    * Grok
    * Copilot
      * Modelo que usa su organizacion
    * Perplexity
  * Open Source
    * Famillia Llama
    * Mistral
    * Chinos
      * DeepSeek
      * Qwen

---  

# Large Langeuage Models

* Propietarios
  * Gemini
    * Google
    * Bueno para el conocimiento factico
    * Tiene muy buena integracion con el motor de busqueda (es google)
        * Agente investigador
    * Integracion con el ecosistema de google
      

## Memoria

> [!NOTA]
> Copilot como esta preparado para uso corporativo suele tener guardrails que evitan generar contenido ofensivo contra una persona en un ambiente corporativ

* Todos los llm tienen un registro de la memoria

* Le puedo decir a la IA que recuerde algo especifico y despues en la parte de configuracion puedo ver que recuerdos la IA decidio guardar sobre mi y los puedo borrar

---

## Respuestas editables

* AKA: Canvas o Artefactos (Claude)

* Problema
  * La IA me genera una respuesta y le pido que cambie algo puntual. La IA cambia eso que le pedi pero ademas cambia otra parte de la respuesta que no le pedi y a veces incluso le cambia el sentido de lo que decia antes
  * Esto hace que tenga que volver a chequear toda la respuesta entera y no peuda confiar en los cambios
* Solucion
  * Generar la respuesta como editable
  * Pedir los cambios concretos seleccionando la parte que quiero cambiar

* Ejemplo en ChatGPT

```
Generame una mail generico para mandar a mi jefe y pedirle un aumento. Dame la respuesta en un canvas editable para poder cambiar partes concretas.
```

* Genera un recuadro con un boton "Editar"

<img width="563" height="149" alt="image" src="https://github.com/user-attachments/assets/69a8e77b-3783-45f8-b6d4-9b967f659780" />


* ChatGPT
  * Se llama Canvas Editable
* Copilot
  * Se llama pagina
  * Se puede compartir para que varios usuarios trabajen sobre la misma pagina
  * Se pueden ver las paginas creadas en la biblioteca
* Claude
  * Se llaman artefactos

---

## Previsualizaciones

> [!NOTE]
> Las previsualizaciones son una extension de las respuestas edibables (canvas, artefactos) que cuando lo generado lo permite te muestra una previsualizacion

* Lo de las respuestas editables lo invento Claude (Anthropic)
* Pero ademas Anthropic permite una previsualizacion de la respuesta cuando se trata de
  * Paginas web
  * Aplicaciones Javascript
  * Diagramas mermaid (despues los vemos)
 
> [!NOTE]
> Claude es el mejor modelo hoy en dia para programar y para tareas tecnicas

### Claude

```
Generame un artefacto con el juego pong (en html y javascript) donde el jugador de la derecha se mueva con las teclas de cursor y el de la izquierda con la a y la z. Que tenga un estilo moderno con efectos especiales y se vea profesional.
```

* Los artefactos en claude se pueden publicar
  * https://claude.ai/public/artifacts/1c6645cf-e908-4722-8f1e-9a77994543d0

### Copilot

* Arriba a la izrquieda esta el desplegable para elegir el modelo y para tareas tecnicas ultimamente Microsof incorporo el modelo Opus

```
Quiero una aplicacion en html vainilla con previsualizacion que sea un dashboard interactivo sobre el avance de un proyecto. Muestra al principio datos de pueba.
```

* Copilot me dice:
  * La vista previa del código está deshabilitada por su seguridad; utiliza la última versión de Microsoft Edge para habilitar el acceso seguro.

---

## Integracion con ecosistema de herramientas

### Gemini

* Integracion con el ecosistema de google
  * Google Sheets
  * Google Docs
  * Google Calendar
  * Google Flights
  * Google Hotels
  * ...

#### Google Calendar

* Abro Gemini
* Abro Calendar

```
Me podes generar un evento en mi calendario que sea "Descasar" de 13 a 14
``'

* Confirmo y veo como se genera el evento en mi calendario

#### Google Flights y Google Hotels

```
Quiero ir a ver a la final de Argentina del mundial. Estoy en Buenos Aires. Quiero que uses google flights y google hotels para buscarme opciones de vuelos y alojamientos.
```

----

### Copilot

* Copilot tiene integracion como Gemini pero con todo el ecosistema de 365
 
##### Calendario de Outlook

* URL
 * https://outlook.cloud.microsoft/calendar/


---

## Agentes

* Un LLM genera una respuesta de texto a partir de una entrada y no hace mas que eso
* Cuando un LLM tiene un objetivo concreo y ademas tiene herramientas (como la busqueda web) estamos dando al llm caracteristicas Agenticas
* Despues vamos a hablar de agentes mucho mas

### Agentes preconstruidos

* Muchos proveedores generan agentes pre construidos con alguna finalidad concreta

### Researcher (agente investigador) 

#### En Gemini (Deep research)

  * Tres investigaciones gratuitas por mes
  * Consulta +100 fuentes en internet dependiendo el tema


<img width="551" height="266" alt="image" src="https://github.com/user-attachments/assets/c03a6f6b-86eb-4dd3-8f42-8422ecd6eadf" />

```
Quiero una investigacion sobre el dragado del canal del rio de la plata y sus caracteristicas. Que proyectos hay. Que licitaciones hay. Que tiene que tener en cuenta una epresa como exolgan sobre el tema. Riesgos y beneficios.
```

* Genero esta investigacion:
  * https://share.gemini.google/gMi4q5AD9NXH

#### En Copilot (Agente Investigador)

* Es un agente precargado de microsoft
  * Se llama Researcher o Investigador
* Es parecido al de gemini, usa bing en vez de google
* Se activa dentro de la parte de agentes
* Su peresencia depende de la licencia que tenga contratada la organizacion

<img width="152" height="304" alt="image" src="https://github.com/user-attachments/assets/dba7265b-f60e-4321-8f81-a9d41381aa27" />


#### Perplexity

* Utilizado para investigaciones academicas

---
Quiero ir a ver a la final de Argentina del mundial. Estoy en Buenos Aires. Quiero que uses google flights y google hotels para buscarme opciones de vuelos y alojamientos.
---

* Es el modelo que se usa en las universidades
* Cita fuentes como:
  * https://www.tandfonline.com/doi/pdf/10.1080/23863781.2022.2116367?needAccess=true
  * https://polipapers.upv.es/index.php/raet/article/view/25770


# Herrmientas

## Napkin

* URL
  * https://www.napkin.ai/
* Caracteristicas
  * Permite enriquecer texto con diagramas visualmente atractivos
* Puntaje
  * 9/10

# Glosario

* GuardRails (guardarieles) : Son censuras que los que entrenan al modelo ponen para evitar problemas legales
  * Grok es el modelo con menos censura de todos
* Vibe Codding
* Grounding : Anclar la respuesta de la IA en fuentes verificables
