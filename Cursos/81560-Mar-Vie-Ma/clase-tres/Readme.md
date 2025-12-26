# Clase Tres - 23 de Diciembre de 2025

# Repaso

* Large Language Models
    * Modelos Propietarios
        * ChatGPT / Copilot
        * Claude
        * Gemini
        * Grok
        * Perplexity
    * Modelos Open Source
        * Chinos
            * Qwen
            * DeepSeek
            * Kimi-K2
        * Americanos
            * Familia LLama
        * Motor De Inferencia
            * Groq
* Herramienta
    * Napkin
    * Natural Readers

# Large Language Models

- ## Mistral

> https://mistral.ai/

* Modelo de lenguaje condenado a ser segundo
* Es el modelo insignia frances

- ## Comparacion de los Modelos 

> https://lmarena.ai/es

* Prompt Utilizado
```
Haceme un analisis sobre el consumo en redes sociales de adolescentes en buenos aires en Zona Oeste
```
* Hay leaderboard con todo lo que vota la gente

- ## Ejecutar modelo Localmente (offline)

> https://lmstudio.ai/

* Permite bajar modelos de lenguaje Open Source a mi computadora para ejecutarlo localmente offline
* Esta bueno tener una buena GPU (Placa de Video)
* Los LLM open source se bajan de Hugging Face

- ## Repositorio de Modelos Open Source

* El github de los modelos de modelos de IA Open Source
* Hay modelos de lenguaje y todo tipo de modelos, generacion de imagenes, etc...
* Crear una cuenta
* En https://huggingface.co/spaces se pueden probar los modelos que van subiendo
         * Ejemplo : https://huggingface.co/spaces/microsoft/TRELLIS.2
  
> https://huggingface.co/

# Prompt Engineering

* Teoria : https://www.instagram.com/p/C5MDsQiR5cG/?img_index=1

- ## Tips Prompt Egineering

* Darle a ChatGPT toda la informacion de contexto que se me ocurra. Esta bueno utilizar el modo voz.
* Doble Promting : Usar el mismo ChatGPT como Prompt Engineering
* Pedirle que te haga las preguntas DE A UNA.
* Pedirle. "Dame la respuesta para copiar y pegar sin acotar nada"
      * Dame un mail para pedir un aumento inventando todo. Dame solamente la respuesta para copiar y pegar sin acotar nada.

- ## Patron Persona

* 3 Solapas de Chrome
      * "Proponeme una receta de un trago para una fiesta familiar en navidad"
      * "Quiero que actues como bartender experto con varias estrellas michelin con mucha experiencia en armado de tragos y expecialista en el tema. .Proponeme una receta de un trago para una fiesta familiar en navidad"
      * Actua como Joaquin Levinton .Proponeme una receta de un trago para una fiesta familiar en navidad
* Panel de Expertos
      * Quiero analizar el consumo de los adolescentes en redes sociales de los ardolescentes de Zona Oeste de Gran Buenos Aires. Me gustarias que busques y que armes un panel de expertos con distintos roles y que cada experto de su vision y opinion del tema. Quiero al menos 10 expertos en materias distintas.
* Repositorio de Prompts
      * https://github.com/f/awesome-chatgpt-prompts
      * https://github.com/estebancalabria/Intro-Ia/tree/main/Prompt%20Engineering/Patrones%20de%20Prompting/Persona

- ## Patron Interaccion

* Consiste en pedirle a la IA que te haga preguntas para obtener toda la informacion de contexto necesaria.
* Parron para manejar el contexto
   * Armarme la dieta del dia
   * Armamr la dieta del dia como un experto en nutricion (Rol/Persona)
   * Quiero que me armes el menu para la cena navideña. Haceme preguntas DE A UNA para obtener toda la informacion necesaria para armarme la cena optima. No escatimes en preguntas. Recien cuando tengas toda la informacion necesaria procede a armarme el menu.  (Patron interaccion)

- ## Patron de Personalizacion de Salida

* Busca respuestas del LLM mas deterministas especificando en forma precisa como quiero la salida
* Primero le pedimos al LLM una lista de algo y luego se la vamos pidiendo en distintos formatos
   * Dame una lista de series estreno en 2026 que me tengo que reservar para ver. Quiero el titulo, actores principales, origen, genero, plataforma
* Formatos 
   * Tecnicos
      * JSON
         * Dame la lista en json
      * XML
         * Dame la lista en XML
   * Ideal Exportar a PDF
      * HTML
         * Dame la lista en html con un disenio moderno y elegante para luego exportarlo a pdf

# Glosario

* LLM : Son modelos de lenguajes de DeepLearning que usan billones de parametros para predecir la siguiente palabra
