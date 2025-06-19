# Modelos Propietarios vs Modelos Open Source

## Modelos Open Source

Los modelos open Source se pueden descargar y utilizar en el ordenador propio.  
> El github de Modelos Open Source : https://huggingface.co/  

Tienen Spaces  
> https://huggingface.co/spaces/black-forest-labs/FLUX.1-dev  

Para ejecutar un modelo de lenguaje localmnente utilizo:  
> https://lmstudio.ai/  

Compendio de herramientas de IA  
> https://theresanaiforthat.com/  

## Prompt Engineering

Un prompt Tiene
* Tarea
* Contexto = Memoria mas conversacion actual
* Persona / Rol
* Ejemplo
* Formato
* Tono

### Patrones de Prompting

#### System Prompt

> Es una instruccion inicial oculta que la empresa que entreno el modelo de lenguaje le da inicialmente mediante la cual se parametriza la "personalidad" del llm y como se tiene que comportar
> No se puede conocer ni cambiar pero si se puede personalizar un poco en chatgpt en las opciones de personalizacion

#### Patron Persona / Rol (Relacionado con Rol)
> **Ejemplos**    
> **Sin Persona** 1) Explicame el cambio climatico    
> **Como un experto** 2) Actua como un cientifico experto en el clima y ecologista y experto en ciclos planetarios y eras terrrestres y quiero que me expliques el cambio climatico y que me des sugerencias como podemos prevenirlo    
> **Como un politico** 3) Actua como Donald Trump y explicame el cambio climatico

#### Patron Audience Persona / Publico Objetivo (Relacionado con el tono)
> **Ejemplo** Explicame el calentamiento global como para un nene de 5 anios

#### Patron Interaccion (Relacionado con el contexto)
> **Ejemplo**    
> Escribime un mail para pedirle un aumento a mi jefe.  Haceme preguntas de a una con toda la informacion que necesites para escribir el mejor mail que puedas y mas persuasivo. IMPORTANTE. Hazme las preguntas una por vez

#### Patron Interaccion (Relacionado con el Formato de la respuesta)

ChatGPT permite no solo manejar el formate de texto libre sino que puedo especificarle formatos especificos en los que quiero la respuesta. Formatos que podemos manejar con ChatGPT
* **Sin formato** : Haceme una lista de 10 lugares que debo conocer para vacacionar.
* **En Bullets** : Listas en bullets (Dame la lista en bullets sin acotar nada)
* **En JSON** : Dame la lista en json separando en otro campo el pais, y una descripcion. Devolver el json sin acotar nada.
* **En XML** : Dame la lista en xml
* **En HTML** : Dame la lista en una pagina html en una tabla con formato profesional y elegante
> Para previsualizar el html sin guardarlo en un archivo les dejo esta pagina : https://www.w3schools.com/html/tryit.asp?filename=tryhtml_basic
> Si guardo el html como un archivo con extension html lo puedo imprimir como pdf. Util para generar pdfs...

> * **En HTML** : Dame la lista en una pagina html en una tabla con formato profesional y elegante



### Tips de Prompt Engineering

#### Tip 1
> Iniciar una conversacion nueva cuando cambio de tema

#### Tip 2
> Contexto : No escatimar en palabras. Darle a chatgpt todo el contexto necesario para que tenga informacion con la que trabajar

#### Tip 3
> Pedirle que pregunte de a una vez : No escribas toda la conversación de una vez. Hazme las preguntas una por vez

#### Tip 4
> Pedirle a ChatGPT que me pregunte lo que no sabe para evitar que me invente y decirle que evite invertar cosas y que si no sabe me pregunte. **Esta bueno incluso cargarlo como parte del system prompt en la personalizacion**

#### Tip 5
> Terminar el prompt con "sin acotar nada" para que no haga una intro ni haga una pregunta de folow up.
