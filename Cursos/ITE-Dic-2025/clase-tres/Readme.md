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

- ## Patron de Prompting : Personalizacion de Salida

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
        * Ideal utilizar el formato markdown

```
# [Titulo]

## Detalle

* **Año** : [Año PUBLICACION]
* **Autor** : [Autor]

## Trama

> [Resumen de la trama]

## Personajes

* Personaje 1
* Personaje 2
...
* Personaje N
---
```

* Mermaid
  * Lenguaje para generar Diagramas
     * https://mermaid.live
  * Claude puede previsualizar Mermaid como artefacto.

* Ejempo diagrama flowchart
```
Generame un digrama mermaid de flowchart para mostrar el organigrama del gobierno de Espania
```

* Ejempo diagrama de PIE
```
Haceme un artefacto con un diagrama pie en mermaid del pib de los paises de Euorpa (modo claro)
```

* Cualquier lenguaje de programacion

```
Generame en matplotlib el codigo que muestre un diagrama de lineas con la evolucion del PIB de espania en los ulitmos 15 anios.
```

---

# Herramientas de IA

## Generacion de Presentaciones

> https://gamma.app/signup?r=cjucljp9heegmkv

* Generamos esta presentacion

 > https://gamma.app/docs/Requerimientos-Fiscales-en-los-Paises-Vascos-g2b81q50y577rg0

* Tambien podemos generar Sitios Web

* Puntaje : 10 / 10

--- 

# IA Generativa Multi Media : Generar Imagenes

> Tip: Los prompts para generacion de imagenes en general funcionan mejor en ingles y se pueden generar en ChatGPT

 - ## Leonardo AI

* Generando imagenes a partir de Texto...

> https://leonardo.ai/

- ## Ideogram

* Generar imagen con texto

> https://ideogram.ai/
- 
