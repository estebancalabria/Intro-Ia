# Clase Tres - 08 de Octubre de 2025

# Repaso

* LLM
  * Canvas : ChatGPT / Gemini ---- Artefactos : Claude
  * Modo Research o Investigacion : Gemini / ChatGPT
* Prompt Engineering
  * Patrones de Promting
    * Rol / Patron Persona
    * Interaccion
    * Personalizacion de Salida
    * Razonamiento / Chaing of thoughts
  * Tips
    * Optimidar de prompts
    * Utilizar a ChatGPT como prompt engineering
    * Contexto
    * Guardar Conversacion
* Herramientas
  * NaturalReaders

# LLM

* Claude
   * Multimodal : Capacidad de procesar imagenes ademas de texto
   * Fue el primero multimodal aunque ahora lo tiene todos
   * Realiza muy bien OCR (Optical Character Recognition)
* Gemini
   * Suele ser el que mayor tamanio de contexto tiene
 * Mixtral
   * Modelo insignia Frances
   * Condenado al segunndo lugar

# Prompt Engineering

## Patron de Personalizacion de Salida

* Pedirle a chatgpt una lista de algo
  * Prompt : "Haceme una lista de matematicas mujeres famosas. Su nombre. Su fecha de nacimiento, su tema principal, mini biografia corta de una oracion. Su nacionalidad."
   
* Transofrmar esa lista en distintos formatos
  * Solo Respuesta
   * Prompt : "Repondeme ... para copiar y pegar sin acotar nada mas"
  * JSON  (Para desarrolladores y  para otras aplicacions) - Ej. En PowerBi
    * Prompt : "Dame la lista en JSON"
  * XML  (Para desarrolladores y  para otras aplicacions)
    * Prompt : "Dame la lista en XML"
  * HTML
     * Prompt : "Dame la lista en HTML"
     * Me sirve para exportarlo a pdf
       * Copio el cntenido en un archivo con extension .html
       * O le puedo pedir a chatgpt que me lo descargue como archivo : "Me lo podes generar en un archivo para descargar"
     * Con Claude lo puedo previsualizar en un Artefacto
     * Si no uso claude...https://www.w3schools.com/html/tryit.asp?filename=tryhtml_basic
   * CSV
     * Prompt : "Generame la lista como un csv"
     * Texto separado por comas
     * Lo podes importar en google sheets o excel
     * FUNDAMENTAL para interfacear entre el LLM y la planilla de calculo
   * Markdown
     * https://es.wikipedia.org/wiki/Markdown
     * Los LLM lo usan internamente para formatear la salida
     * Me sirve para escribir plantillas exactas de que como quiero el formato de la respuesta
     * Tip : Tener el repositorio de plantillas markdown para tareas comumes
     * Se puede utilizar en la parte de instrucciones personalizadas

Prompt Utilizado para Markdown con plantilla
```txt
Generame la lista utilizando la plantilla que viene a continuacion. Generame la respuesta para copiar y pegar sin acotar nada mas. La plantilla es
# [Nombre]
- ## *[Fecha_De_Nacimiento]*
> [Biografia]
### Temas Principales
* [Tema 1]
* [Tema 2]
```

* Para graficos y diagramas
   * Mermaid
      * https://mermaid.live/
      * Ideal para generarlos con Claude
    * SVG (Scalar Vector Grafics)
       * Cuando mermaid no tiene el grafico que busco...
     * DOT
       * Especial para hacer Grafos
       * https://edotor.net/
       

Ejemplo Mermaid prompt ChatGPT
```txt
Generame un diagrama PIE en mermaid que se vea el PIB por pais de Europa. Dame el codigo del diagrama para copiar y pegar si acotar nada mas.
```

Ejemplo Mermaid que use en Claude
```txt
Dame un mermaid con un diagrama de bloque de tres niveles (maximo 3 recuadros por nivel) de la estructira del gobierno de Espania y sus responsables.
```

Ejemplo SVG que use en Claude
```txt
Generame un artefacto con un diagrama de bloques en SVG que muestre el PIB de los 5 paises con mayor PBI de Europa 
```

Ejemplo dot que use en ChatGPT
```txt
Me podes hacer un grafo en el lenguaje dot con los 5 paises principales de europa y sus fronteras. Devolver el codigo del grafo para copiar y pegar sin acotar nada mas.
```

# Uso de la API

# Herramientas

## Text to Speech

* Natural Readers : https://www.naturalreaders.com/

## Speech to Text

- ### Transcribir videos de Youtube
  
* Unlimited Summary Generator for YouTube™ : https://chromewebstore.google.com/detail/unlimited-summary-generat/eelolnalmpdjemddgmpnmobdhnglfpje

Puntaje : 10 / 10

- ### Transcribir reuniones y videos

Resumen de herramientas pra reuniones :  https://www.instagram.com/p/DBzb-kHxqae/?img_index=1

> El Microsoft Teams ya tiene esto incorporado

En general estas herramientas tienen dos opciones de uso
1. Tomando notas de las reuniones en forma automatica (a veces agregan un participante a la reunion(
2. Pasandole un video de la reunion una vez finalizada

* Herramienta Recomendada : https://tactiq.io/es

Puntaje : 8/10


