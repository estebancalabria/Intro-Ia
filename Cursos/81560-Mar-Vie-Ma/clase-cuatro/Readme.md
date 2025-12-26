# Clase Cuatro - 26 de Diciebre 2026

# Repaso

* Large Laguage Models
    * Mistral
    * LMarena 
* Prompt Engineering
    * Receta de prompts Efectivos : https://www.instagram.com/p/C5MDsQiR5cG/?img_index=1
    * Patrones de Prompting
        * Persona / Rol
        * Interaccion
        * Personalizacion de Salida
          * json
                * JSON Prompting: https://www.youtube.com/watch?v=GNNUdlG22ZA&t=198s
          * xml
          * html  >>> Para generar PDFs
* Open Source
  * Hugging Face
      * Spaces
  * LMStudio

# Prompt Engineering

- ## Personalizacion de Salida : CSV (Cooma Separated Values)

* Me permite representar como texto una planilla de calculos
* Tanto excel como Google Sheets interpretan de forma nativa

```
Haceme una lista de 10 series de estreno para el 2026 . Quiero nombre. Temporada. Actore Prinicipal, plataforma, genero, resumen argumento, fecha planeada estreno.
```

* Pasamos la lista a csv

```
Dame la lista en formato csv
```

* El contenido generado por el LLM lo guardo en un archivo con extension .csv
* Creo un documento de google sheets en : https://sheets.google.com/
  * File...Import...Upload...Replace Current Sheet

- ## Personalizacion de Salida : Plantillas con Markdown 

* Permite definir una plantilla con el formato exacto en el quiero la salida
* Aumenta determinismo de la IA
* Markdown : https://es.wikipedia.org/wiki/Markdown
* Ejemplo de plantilla mardkdown
* Te ahorra horas de formateo a mano

```
# [Titulo Serie]

## Informacion

* **Plataforma** : [PLATAFORMA DONDE SE EMITE]
* **Fecha** : [FECHA DE RELEASE]
* **Genero** : [GENERO DE LA SERIE]
* **Temporadas** : [CANTIDAD TEMPORADAS]

## Actores

* Actor 1
* Actor 2
* ...
* Actor N

## Argumento

> [ARGUMENTO SERIE]

---
```
* El prompt completo
```
Devolveme las series utilizando esta plantilla "
# [Titulo Serie]

## Informacion

* **Plataforma** : [PLATAFORMA DONDE SE EMITE]
* **Fecha** : [FECHA DE RELEASE]
* **Genero** : [GENERO DE LA SERIE]
* **Temporadas** : [CANTIDAD TEMPORADAS]

## Actores

* Actor 1
* Actor 2
* ...
* Actor N

## Argumento

> [ARGUMENTO SERIE]

---" devolveme la lista para copiar y pegar sin acotar nada mas
```
* Se puede poner en un google docs aca : https://docs.google.com/

# Personalizaciond de Salida : Mermaid

* 


