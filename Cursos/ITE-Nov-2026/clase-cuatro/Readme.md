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

## IA para generar Diagramas y Presentaciones

### Mermaid

* Ya vimos que la IA puede generar diagramas utilizando mermaid

### Napkin

* Herramienta para generar diagramas a partir de texto
* URL
   * https://www.napkin.ai/es/
* Vamos pegarle el texto de la investigacion de gemini y enriquecerla con diagramas

<img width="666" height="357" alt="image" src="https://github.com/user-attachments/assets/09d10d6a-4a78-4322-bcd9-a932f9f491c0" />

> [!NOTE]
> Ahora le agregaron la capacidad de hacer presentaciones que no lo habia probado. Probemoslo juntos!

* Subimos aca el pdf y el ppt generado por napkin

### Gamma

* Esta herramienta es la opcion mas popular para generar presentaciones con IA
* URL
   * https://gamma.app/signup?r=cjucljp9heegmkv
* Caracteristicas
   * No solo genera presentaciones
   * Paginas Web / Landings
   * Contenido para redes sociales
* Generamos esta presetacion
   * https://gamma.app/docs/Nvidia-tras-Jensen-Huang-escenarios-y-estrategia-de-inversion-dr87cbpcckehqa7

### PowerPoint

* Dentro de 365 (con licencia) tambien podemos generar presentaciones pon Powerpoint directamente
* Necesito la licencia de 365
* Generamos esta presentacion

---
# Break
Hasta y 15.
Luego comparamos
---

## Verificacion Cruzada con Claude

* Tengo 3 presentaciones hechoa con 3 IA distinta
* Voy a crizarlas con Claude para evaluar cual es mejor
   * Claude al ser un modelo tecnico resulta muy efectivo para correcciones y validaciones cruzadas

```
TE adjunto 3 presentaciones. Ademas te adjunto el texto que utilice para generar las presetaciones (Contenido adjunto). quiero que analices las tres presentaciones en de detalle, las contraste con la investigacion en las cuales fueron basada, me hagas un analisis y me digas cual te parece mejor
```

* El resultado
   * https://claude.ai/share/32d0fd09-35d6-4194-b425-87ca9c771889

## Compedio de Herramientas

* Repositorio de Herramientas
   * https://theresanaiforthat.com/
* Catalogo de Herramientas de IA (Como las que vimos hoy)

## Videos Institucionles basados en Avatar (Hey Gen)

* URL
   * https://www.heygen.com/

## Recomendacion

* Herramienta de IA que incluye varias
* Se las recomiendo para que la explorer
* Es mas facil pagar una subscripcion a una sola herramienta que a varias
   * https://passportai.app/

# PRoxima Clase Creamos un video con Hey Gen
