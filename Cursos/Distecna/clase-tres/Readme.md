# Clase Tres - 28 de Noviembre del 2025

# Repaso 

* LLM
  * LLM Propietarios
    * ChatGPT
    * Gemini
    * Grok
    * Perplexity  << Para investigacion con Citas
  * LLM Open Source
    * Los Modelos Open Source Se suben a Hugging Face y te lo podes bajar
        * **IMPORTANTE: LOS SPACES : https://huggingface.co/spaces**
    * Para ejecutar un modelo Open Source Localmete
        * LMStudio
        * Ollama
    * Mistral (FRACIA SEGUNDO)
    * Groq
      * https://chat.groq.com/
    * Familia LLama
    * Chinos
      * Qwen
      * DeepSeek
* Comparar LLM
  * LMArena
* Prompt Engineering
  * Patron Persona

# Prompt Engineering

> Explicacion General + Super Formula : https://www.instagram.com/p/C5MDsQiR5cG/?img_index=1

- ## Patron Persona / Rol

* Abri 3 Solapas de Chrome con ChatGPT
* Vamos a hacer el mismo prompt
   * Directo

```
 "Dame consejos para dormir mejor"
```

   * Preguntandole a un Rol especifico

```
"Actua como un especialista en suenio, somnologo medio profesional y buenos habitos y dame tips fundamentados de como lograr una mejor salud del suenio."
```

* Preguntandole a una persona especifica
```
 "Actua como Lili suyos y dame consejos para dormir mejor"
```

> Pueden explorar muchos ejemplos del patron Persona en : https://github.com/f/awesome-chatgpt-prompts

- ## Contexto : Patron Interaccion

"Quiero que me hagas preguntas DE A UNA POR VEZ para..." (A veces le agrego que me haga preguntas de respuestas cortas)

Ejemplo

```
Actua como un especialista en suenio, somnologo medio profesional y buenos habitos y dame tips fundamentados de como lograr una mejor salud del suenio personalizada para mi. Quiero que me hagas preguntas DE A UNA POR VEZ para conocerme y hacerme el mejor plan de suenio adapatado a mi vida. Haceme todas las pregutnas que consideres necesarias para obtener el mejor plan de suenio optimo adaptado a mi persona
```

Ejemplo (De Soledad)

```
Actua como el mejor especialista en comunicacion organizacional y dame consejos fundamentales de como lograr la mejor comunicacion dentro de la empresa como especialista en rrhh. QUiero que me hagas una pregunta a la vez para conocer la empresa y obtner el mejor plan de comunicacion dentro de la empresa
```

Tips de Contexto
* Nuevo tema, Nueva conversacion
* Guardar conversaciones frecuentes para no tener que repetir todo el contexto

# Formato : Personalizacion de Salida

* Formatos de Salida
   * Sin Formato : "Dame una lista de las 10 mejores series policiales"
   * Tecnicos
      * json
      * XML
      * TOON
   * Tecnico / Exportar a PDF
      * HTML : "Dame la lista en html en un formato profesional para luego generar un pdf"
   * Tecnico / Interactuar con Excel o Google sheets
      * CSV (Comma Separated Values) : Dame la lista como un CSV
         * Este es un formato MUY importante porque me permite interactuar desde y hacia excel
   * Markdown
      * https://es.wikipedia.org/wiki/Markdown
      * Plantilla MArkdown para especificar EXACTAMENTE como queremos la salida
```
---

# [TITULO]

## Detalles

* **Genero** : [GENERO DE LA SERIE]
* **Año** : [AñO DE LA SERIE]
* **Plataforma** : [PLATAFORMA PRINCIPAL]

## PORQUE VERLA

> [TRAMA DE LA SERIE]

## ACTORES PRINCIPALES

1. [ACTOR 1]
2. [ACTOR 2]
...
N. [ACTOR N]

---
```      
      
 * Mermaid
    * https://mermaid.live/
    * Ideal para usarlo en Claude

```
Armame un mermaid que muestre un diagrama de pie que muestre el presupuesto de cada una de las series
```

Salida

```mermaid
pie
    title Presupuesto Conceptual de las 10 Series Policiales (Valores Ficticios)
    "Mindhunter (Netflix)" : 50
    "True Detective (S1 - HBO)" : 40
    "Mare of Easttown (HBO)" : 35
    "Bosch (Prime Video)" : 30
    "Sherlock (BBC/HBO)" : 25
    "Luther (BBC/HBO)" : 22
    "The Wire (HBO)" : 20
    "The Bridge (Nordic)" : 18
    "Line of Duty (BBC)" : 15
    "The Killing (Nordic)" : 12
````
  
Otro Ejemplo

```
Me compre un terreno y quiero hacer una casa. Armame un artefacto con mermaid el Gant de todo el proyecto hasta que este la casa terminada...
```

```mermaid
gantt
    title Proyecto de Construcción de Casa
    dateFormat YYYY-MM-DD
    
    section Planificación y Trámites
    Proyecto arquitectónico           :p1, 2025-01-01, 30d
    Estudio de suelos                 :p2, after p1, 15d
    Planos definitivos                :p3, after p2, 20d
    Aprobación municipal              :p4, after p3, 45d
    
    section Preparación del Terreno
    Limpieza del terreno              :t1, after p4, 5d
    Replanteo y nivelación            :t2, after t1, 3d
    Excavación para cimientos         :t3, after t2, 7d
    
    section Estructura
    Cimientos y bases                 :e1, after t3, 15d
    Columnas y vigas                  :e2, after e1, 20d
    Losa de entrepiso (si aplica)     :e3, after e2, 12d
    Estructura de techo               :e4, after e3, 15d
    
    section Albañilería
    Levantamiento de paredes          :a1, after e4, 25d
    Techos y cubiertas                :a2, after a1, 10d
    Contrapisos                       :a3, after a2, 8d
    
    section Instalaciones
    Instalación eléctrica             :i1, after a3, 15d
    Instalación sanitaria             :i2, after a3, 15d
    Instalación de gas                :i3, after i1, 8d
    Instalación de agua               :i4, after i2, 8d
    
    section Terminaciones Gruesas
    Revoques exteriores               :tg1, after i4, 20d
    Revoques interiores               :tg2, after tg1, 25d
    Carpeta de pisos                  :tg3, after tg2, 12d
    Colocación de aberturas           :tg4, after tg3, 10d
    
    section Terminaciones Finas
    Pintura exterior                  :tf1, after tg4, 10d
    Pintura interior                  :tf2, after tf1, 15d
    Colocación de pisos               :tf3, after tf2, 15d
    Colocación de revestimientos      :tf4, after tf3, 12d
    Mesadas y muebles de cocina       :tf5, after tf4, 8d
    
    section Detalles Finales
    Sanitarios y grifería             :df1, after tf5, 5d
    Artefactos eléctricos             :df2, after df1, 5d
    Limpieza final                    :df3, after df2, 3d
    Inspección y entrega              :df4, after df3, 2d
```
