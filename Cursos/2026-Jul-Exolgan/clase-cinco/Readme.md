# Clase Cinco - 7 de Agosto del 2026

# Repaso

* Large Language Models
  * Open Source
    * Super importantes cuando hablamos de privacidad de datos
    * Ejecucion de modelos Localmente
      * LMStudio
      * Ollama
    * Hugging Face
      * Spaces
    * Groq
  * Propietarios
    * Gemini
      * Modo Investigacion
* Herramientas
  * Text-To-Speech
    * Natural Readers
  * Visualizacion
    * Napkin
* Prompt Engineering
    * Tips
      * Usar a la IA como experto en prompt engineering
      * Usar el modo voz para dale mas contexto
    * Prompt
      * Tarea + Contexto + Ejemplos + Rol + Formato + Tono
    * Contexto
      * (prompt) -> (+ memoria) -> (+ herramientas) -> (+ conversacion actual/pasadas) -> (+ Instrucciones personalizadas/System Prompt) -> (llm)
    * Tecnica de promting
      * Prompt Chainning / Interaccion
        * Generar una conversacion con todo el conexto necesario
      * Rol/Persona
        * Rol / Persona PArticular / Panel de Expertos

---

# Prompt Engineering

## Formatos de Salida

* Como le puedo pedir a la IA que responda

* Pedirle a la Una lista de algo sin formato
  * "Quiero una lista de 10 terminales como Exolgan que trabajen con contenedores estimando ubicacion, cantidad de contenedores que pueden almacenar, volumen diario de traslados, importancia en el sector y otros datos que sean relevantes. Investigar en internet."
* Tecnicos
  * JSON
    * "Dame la lista en JSON
  * XML
    * "Dame la lista en XML
* Pseudo Tecnicos
  * Generar un pdf
    * Lo hace pero es visualmente muy limitado
  * Generar un Word
    * Generamelo en word
  * HTML
    * "Me podes generar la lista en un unico html para presentar que se vea moderno, profesional, si es posible con imagenes, que sea apto para imprimit y que pueda madar a un cliente o un jefe."
    * ChatGPT hace una previsulizacion (parecido a los artefactos de Claude)
    * Tiene mucha mejor pinta visual que el pdf que generamos antes
    * Se puede descargar, lo abris y lo imprims con ctrl+p
    * Se puede iterar sobre el formato, el contenido, etc...
* Representacion Tabular
  * Como Tabla
    * Generarme la informacion como una tabla
  * En CSV
    * Es un formato portable que excel interpreta nativamente
    * "Dame la lista en csv"
    * Se puede compatir
      * https://chatgpt.com/s/t_6a75e46839e8819199d899423ff3922c
    * "Dame el csv para descargar" (Lo tuve que hacer con claude gaste mis tokens del dia para chatgpt)
    * Lo puedo abrir con Excel
* Sencillos
  * La idea es que podes controlar el formato de salida
  * En bullets
  * En cartas

### Markdown

* Es el formato en el que esta escrito este documento
    
---

# Glosario

* No Determinismo : El mismo prompt no produce siempre la misma respuesta
