# Clase Cuatro - 17 de Noviembre del 2026

# Repaso

* Prompt Enginerring
    * Anatomia del Prompt
      * Prompt = Tarea + Contexto + Rol + Formato + Tono + Ejemplo
    * Rol
      * Tecnica de persona
      * Decirle a la IA desde donde queremos que nos responda
    * Contexto
      * Encadenamiento de Prompts
        * Generar una conversacion con el contexto necesario
        * Interaccion: Pedirle a la IA que me haga preguntas
      * Plan
        * Generar una planificacion antes de generar la respuesta
      * Formato de Salida
        * Tecnicos
          * JSON
          * XML
          * Codigo Fuente
        * Pseudo-Tecnicos
          * Pdf
          * Html
            * Para generar pdf
          * CSV
            * Para interactuar con Excel
        * Markdown
          * Lenguaje que la IA usa por defecto para darle formato a la salida
          * Generar una plantilla para definir como queremos exatamente la salida
        * Mermaid
          * Generar graficos y Diagramas

---

# Herramienta de Productividad

## Generacion de Codigo Fuente

* Vamos a Claude
  * https://claude.ai/new

* Le pedimos

```
Quiero que me generes un unico artefacto entregable con el codigo del juego pong (en javascript y html) donde el jugador de la derecha se mueve con las teclas e cursor y el de la izquierda con la a y la z. El juego debe poder lleva la puntuacion. Se debe pode pausar con la barra espaciadora y reiniciar o continuar. Debe tener efectos visuales y de particulas y una esetica neon. Debe ser un proyecto tipo AAA lo mejor que se pueda. Que sea dinamico, moderlo y con buenos graficos.
```
* Genero este pongo
   * https://claude.ai/share/a08acc66-a167-45f6-88ae-efefc556211b
   * Que tambien esta subido en este repo

### Artefactos o Canvas editables
 
> [!NOTE]
> Un artefacto para claude es una previsualizacion (te divide en dos la pantalla) para ver en la misma interfaz como queda el resultado generado. Sirve para mermaid, html, documentos, markdowon

* En ChatGPT, en Copilot, Gemini
   * PAginas, canvas
   * Me ayuda un monton a editar parcialemente el resultado

* Por ejemplo en ChatGPT
```
Generame un texto con una historia corta. Generamelo en un canvas editable
```

* Puedo editar por parrafos, palabras secciones y no todo el contenido junto

--

## Vibe Coding  

* Generar aplicaciones para mi trabajo utilizando lenguaje natura
* Se generan utlizando los LLM que vimos (como Claude Sonnet) y algun entorno agentico especial para hacer esta apps
* Existen varios entornos de Vibe Coding
   * Lovable
      * https://lovable.dev/es/
   * Bolt.new
   * Replit

* Probamos este prompt en Lovable
```
Crear una aplicacion para cotizar automaticamente una propiedad. El uusario ingresa sus metros cuadrados, la cantidad de habitaciones, si tiene parque o no, el estado general de la propiedad y el sistema le devuelve un aproximoado del coste de la misma. Inventar el calculo.
```

* Con ese prompt hicimos este tasador
   * https://casa-worth-whisper.lovable.app/
 
----

## Text-To-Speech

* La IA tiene la capacidad de tomar texto y leerlo.
* Vamos a partir de la investigacion que hicimos con gemini
   * https://share.gemini.google/BQetqEiBJloi

* Suponganse como el texto es muy largo quiero que la IA me lo vaya leyendo
   * Puedo utilizar herramientas como Natural Readers
      * https://www.naturalreaders.com/

* Si necesitara calidad de voces mas profesionales
   * ElevenLabs
      * https://elevenlabs.io/
      * La opcion de generacion de texto a voz mas completa en el mercado
      * Se pueden generar bot automaticos que hablen con el cliente con esta generacion de voz
      * La version gratuita es muy limitada

---
Break
Hasta y 10
---
