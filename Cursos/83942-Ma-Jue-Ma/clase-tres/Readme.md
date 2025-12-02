# Clase Tres - 2 de Diciembre 2025

# Repaso

* LLM
  * LLM Propietarios
    * Perplexity
    * Grok
  * LLM Open Source
    * LLama
    * Groq
    * Chinos
      * DeepSeek
        * Modo Razonamiento
      * Qwen
* Herramientas
  * Text-To-Speech
    * NaturalReaders
    * Coquitts
   
# Prompt Engineering

> https://www.instagram.com/p/C5MDsQiR5cG/?img_index=1

## Patrones de Promptimg

- ### Formular De Prompting Experto

> https://www.instagram.com/p/C5MDsQiR5cG/?img_index=1

- ### Tips Prompt Engineering

* Guardarse una base con los prompts habituales que utiliza
* Cada conversacion tiene una Direccion Unica.
   * Guardar conversaciones de temas que utilizo frecuentemente para evitar tener que repetir todo el contexto
   * Cuando cambio de tema iniciar una conversacion nueva para no confundir el contexto
* Pedirle el resultado "Dame el resultado para copiar y pegar directamente sin acotar nada mas"
   * Elimina la introduccion y la pregunta de seguimiento del final
   * Me pone solamente lo que me intersa para copiar y pegar

- ### Persona / Rol

* Abrimos Tres Solapas de ChatGPT
* Pensar un prompt
    * Directa
      * "Decime una cena para hoy"
    * Desde un Rol
      * "Actua como un chef gourmette de un restaurante con 3 estrellas michelin y recomiendame que cenar hoy"
    * Como una persona conocida
      * "Actua como German Martitegui y recomiendame que cenar hoy"

* Links
> https://github.com/f/awesome-chatgpt-prompts

* Otro ejemplo del patron persona por Oscar (**PROMPT CHAINING**)
> (PROMPT 1) Perdile la conformacion de un comite tecnico experto en (ESTA MATERIA) y determinar los distintos perfiles que puedan opinar
> > (y una vez que tengo el comite tecnico externo)...
> (PROMPT 2) Preguntarle los distintos puntos de vistas de las profesiones para (ESTE TEMA)
> **UTIL (CRUZAR EXPERTOS)**

- ### Patron de Interaccion

* Consiste en decirle a ChatGPT que me haga pregutnas DE A UNA para determinar la informacion que necesita para darme la respuesta optima

```
Actua como un chef gourmette de un restaurante con 3 estrellas michelin y recomiendame que cenar hoy. Quiero que me hagas preguntas DE A UNA para obtener el menu optimo para mi cena. Una vez que termines de hacer TODAS las preguntas necesarias ahi si procede a hacerme la recomendacion.
```

**Otro Ejemplo**
 
* No es lo mismo decirle a la A
```
Actua como un Personal Trainner y armarme una rutina de ejecicios fisicos. 
```

* Que esto
```
Actua como un Personal Trainner y armarme una rutina de ejecicios fisicos. Quiero que me hagas preguntas DE A UNA para obtener la rutina de ejecicios optima para mi persona.
```

- ## Patron : Personalizacion de Salida

Para empezar pidamosle una lista de algo
```
Dame una lista de actividades para hacer en mendoza. Quiero saber nombre, duracion, descricpcion, costo estilado (barato, caro, gratis), tipo de actividad, (y los datos que se te ocurran)
```

* Formatos
  * Tecnicos 
     * JSON (Javascript Object Notation)
        * "Dame la lista en formato json"
     * XML (eXtensive markup language)
        * "Dale la lista en XML"
   * Por Ejemplo : Para Generar PDF
      * HTML
         * "Me generaas la lista en un html moderno y elegante"
          * Copio el html y lo pego en un bloc de notas
          * Salvo con extension html ej "Mendoza.html"
          * Le doy doble click en el archivo y lo abro...
          * Ese html los puedo imprimir (Ctrl+P) y generar asi un pdf
    * Por Ejemplo : Exportar a Word
       * Markdown
         * https://es.wikipedia.org/wiki/Markdown
         * Lo usamos para crear plantillas del formato exacto en el quiero la respuesta

```
# [Titulo De LA Actividad]

## Detalles

* **Duracion** : [DURACION ACTIVIDAD]
* **Precio** : [DURACION ACTIVIDAD]

## Descripcion

> [DESCRIPCION DE LA ACTIVIDAD]

---
```

Ejemplo prompt completo

```
Dame una lista de actividades para hacer en mendoza. Quiero que respondas respetando la siguiente plantilla markdown "# [Titulo De LA Actividad] ## Detalles * **Duracion** : [DURACION ACTIVIDAD] * **Precio** : [DURACION ACTIVIDAD] ## Descripcion > [DESCRIPCION DE LA ACTIVIDAD] ---"Dame el resultado para copiar y pegar directamente sin acotar nada mas
```

# Herramientas

## Herramienta para generar documentos lindos : Napkin

> https://www.napkin.ai/

* Se le puede pegar el logo despues como imagen
* Puntaje : 10 / 10
