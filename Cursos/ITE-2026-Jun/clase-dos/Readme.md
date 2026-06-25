# Clase Dos - 25 de Junio 2026

# Repaso

* Roadmap del curso
* Fundamentos de los LLMS
  * Prompt
  * Token
  * System Prompt
  * Multimodales
* Uso responsable de la IA
  * Predecir el proximo token
  * Alucinaciones
  * Grounding
* Large languange Models
  * Propietarios
    * ChatGPT
    * Claude
    * Gemini
    * Copilot
  * Open Source
    * ...
  * Caracteristicas
    * Instrucciones Personalizadas
    * Uso de la Memoria
    * Uso de Herramientas
      * Busqueda web

---

# Large Language Models

## Fundamentos

* Copilot por detras usa ChatGPT el modelo de OpenAI
  * (copilot) <---> (Filtro de Seguridad de Microsoft / Guardarieles) <---> (Modelo Raiz : ChatGPT o Claudec)

## Compativa entre LLMs

* Propietario
  * ChatGPT
    * Generacion de texto como si fuera un humano.
    * La experiencia de usuario, que parezca que hablo con una persona (por eso tiene memoria, instrucciones personalizadas)
  * Claude (Anthropic)
    * Ideal para tareas tecnicas (progracion, respuestas tecnicas)
    * Fuerta control etico en las respuestas
  * Gemini (Google)
    * El grounding, la busqueda web
    * Integracion con el ecosistema de google
  * Copilot

> [!NOTE]
> Noticia sobre el enfoque resposable de la IA de Anthropic (Claude) y la disputa que tuve con el gobierno de Estados Unidos al respecto
> https://www.bbc.com/mundo/articles/cddnjd34p7no

## Propietarios

### Uso del Liezo, Canvas o Artefacto

* Para Gemini y ChatGPT lo llamamos Canvas

* Problema
    * Genero un texto con la IA. Por ejemplo un Correo
    * Hay una oracion que quiero que cambie, algo que no me cierra
    * Le pido a la IA que regenere la respuesta considerando el cambio solicitado
    * La IA me genera nuevamente el texto con el cambio solicitado peero sin que yo se lo pida cambia otra cosa
* Solucion
    * Es genrar un canvas
    * Un documento editable al cual le podes pedir cambios especificos y la IA solamente va a cambiar el texto o parrafo que seleccionaste dejando el resto como esta

* En ChatGPT

```
Quiero mandar un correo a mi jefe para pedirle un aumento. Quiero que me generes un canvas para que yo pueda ir modificando y actualizando tu propuesta inicial.
```
* Puedo seleccionar y pedirle a ChatGPT que me modifique solamente el texto seleccionado y dejar el resto como esta

> [!NOTE]
> No me deja hacerlo en gemini. Antes se podia

* El claude
  * Un artefacto es un cocepto en claude que divide la pantalla en dos
  * Se pude alternar entre la vista previa el codigo
  * Se pueden compartir con otros
  * Se puden versionar
  * Se pueden editar parcialmente

```
Quiero mandar un correo a mi jefe para pedirle un aumento. Quiero que me generes un artefacto para que yo pueda ir modificando y actualizando tu propuesta inicial.
```
> [!NOTE]
> A veces no te lo hace de una sino que tenes que insisitir

* Otro ejemplo de Artefacto en claude

```
Programame en un solo artefacto el juego pong en html y javascript. Que el jugador de la derecha se mueva con las teclas de cursor y el de la izquierda con la a y la z . Que se vea moderno, elegante, profesional y tenga efectos visuales.Lo quiero como artefacto en pantalla dividida
```

* Me genero este artefato
  * Los artefactos de Claude se pueden compartir 
  * https://claude.ai/public/artifacts/d3e95fa6-fb4d-4312-a2d2-c169a8fbc1a9

## Gemini

* URL
  * 
* Caracteristicas
  * Respuestas orientadas al conocimiento factico (hechos)
  * Modo Investigacion
    * 3 gratis por mes
    * Busca en 100+ de paginas web un tema especifico y genera un documento / resumen
  * Integracion con el ecosistema de googe

### Integracion con el Ecosistema de Google

#### Calendar

```
Agregarme un evento de una hora para hoy a las 17:00 que sea "Preparar clase del Az-400"
```

* Primero me pide confirmacion y despues le doy ok y verifico que efectivamente el evento aparece en mi calendario

#### Google Flights y Google Hotels

```
Quiero viajar al mundial a ver el proximo partido de Argentina. Estoy en Buenos Aires. Quiero que me busques en google flights opciones de vuelo y en google h otels opciones de Alojamiento.
```

* Me devolvio esta conversacion:
  * https://share.gemini.google/tKET4WsrqRgf

#### Google Drive (Sheets, docs)

```
Creame una tabla donde muestre en Spain la cantidad de mascotas por habitante por regiion y todos los datos que te parezcan relevantes para alquien que tenga un negocio de venta de alimentos para mascotas
```
---

###  Modo Investigacion

> [!NOTE]
> Estamos viendo gemini pero otros modelos como ChatGPT tienen algo parecido. En este ultimo se llama "Investigacion Avanzada"

* El modo investigacion esta basado en informacion extraida de la web

```
Quiero una investigacion sobre el mercado de venta de alimentos para mascotas en Spain
```

* Este modo de investigacion puede consultar 100+ web dependiendo el tema de investigacion elegido
* Investigacion de Gemini
  * https://share.gemini.google/seYCx6dCid3v
* Investigacion de ChatGPT (Altenativa)
  * https://github.com/estebancalabria/Intro-Ia/blob/main/Cursos/ITE-2026-Jun/clase-dos/Investigacion%20ChatGPT.pdf

  
---
## Open Source

---

# Glosario

## Accountability o Responsabilidad

* La IA es una herramienta y las personas son resposables de lo que hacen esa informacion. No vale hecharle la culpa a la IA

## Guardrails (Guardarailes)

* Restricciones que le pone el propietairio que da acceso al LLM para que las peticiones (prompts) esten alineadas con las politicas de seguridad establecidas.
