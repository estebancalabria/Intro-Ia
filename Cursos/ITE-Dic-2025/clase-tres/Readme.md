# Clase Tres - 9 de Diciembre del 2025

# Repaso

* Large language Models
  * https://lmarena.ai/
* Prompt Engineering
  * Persona / Rol

# Prompt Engineering

- ## Patron de Prompting : Interaccion

* Prompt Utilizado
```
Actua como un nutricionista con mucha experiencia y quiero armar el menu de comida de la semana.
 Quiero que me hagas preguntas DE A UNA para obtener el menu optimo adaptado a mi persona.
Quiro que me hagas todas las preguntas que consideres necesarias y cuando tengas toda la informacion
necesaria para realizar el menu optimo para mi persona procede con la generacion del mismo.
```

* Tip importante : Solicitar que las preguntas me las haga **DE A UNA**

- ##Patron de Prompting : Personalizacion de Salida

* Sin Formato

```
Dame una lista de 10 libros clasicos que deberia leer antes de morir
```

* Formatos de Salida:
    * Tecnicos
        * XML
          * Ejemplos " Dame la lista en xml"
        * JSON
          * Ejemplo : "Dame la lista en json, Nombre, año, autor, genero, resumen_trama"
    * Formato para generar PDF
      * HTML
          * Ejemplo : "Me podes devolver la lista en html en un formato moderno y elegante"
    * Formato para generar Planillas de Calculo
      * CSV
        * Se puede abrir con el google sheets : sheets.google.com
    * Especificar la salida en una plantilla
        * 
