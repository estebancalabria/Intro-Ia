# Clase 9 - 21 de Agosto del 2026

# Repaso

* IA Creativa
  * Generacion de Videos
    * Pixverse
    * HF
    * Arena.AI
    * HeyGen (Videos basados en avatar instucionales / redes)
  * Generacion de Musica
    * Udio
    * Suno
  * Regalo del profe
    * https://passportai.app/

---

# IA para Analisis de Datos

## Setup / Preparacion para empezar a trabajar

* Crear un documento en google Sheets para Analisis de Datos
    * https://sheets.google.com/
    * Crear un documento nuevo

* Loggearse en Kaggle
  * https://www.kaggle.com/

* Descargarse el Dataset del Titanic (el todos usan para aprender ML)
  * https://www.kaggle.com/datasets/brendan45774/test-file
  * Descarga el dataset
  * Tengo que tener un archivo tested.csv

* Importar el tested.csv en una planilla de Google Sheets

* Duplicar el libro para tener una copia

* Instalar la extension simple ml for sheets
    * https://simplemlforsheets.com/
 
* Refrescar la hoja de calculo y verificar que aparece en el menu de extensiones

## Machine Learning

* Teoria
 * https://www.instagram.com/p/C1ntRrRswAu/?img_index=1

* Preparacion de datos
  * Elegir Columnas
    * Elegir Label (Objetivo)
       * Survived
       * La pintamos de Verde
    * Elegir Features (Variables de Interes)
       * PClass
       * Sex
       * Age
       * SibSP
       * Parch
       * Fare
       * Embarqued
    * Columnas Descartadas
       * PassangerID
       * Name
       * Ticket
       * Cabin (Muchos datos faltantes)
  * Asegurarnos que todos los datos sean numericos
     * Asegurar que la columan Age se interprete como un numero
        * Columna seleccionada -> Format -> Number -> Number
     * Asegurar que la columna Fare se interprete como numero tambien

* Separar los datos de prueba de los de entrenamiento
  * Borrar de la fila 2 a la 35 el contenido de la columna Surived

* Enternar el modelo (y predecir los datos de prueba)
   * Extensions -> Simple ML for Sheets -> Start
     * Predict missing values
       * Column with empty cells : Survived
       * Source Column
         * Elegimos las columnas que pintamos con amarillo
         * No debe haber ninguna columna de tipo Text
       * Se puede ver que hay varios algoritmos de ML para elegir
       * Predict
   * Agrego una columna : Pred:Survived
 
* Evaluar el modelo (a ojo)
  * Comparar la comluna Pred:Survived con la columna Survived de libro que me copie
  * Vemos una eficiencia del 100x100 (algo que en la realidad no pasa mucho)

> [!NOTE]
> Una vez que tengo el modelo entrenado puedo sacar informacion de el en el menu advaced "explain" de la extension
   
---

# Agente de Recuperacion de Datos

* Vamos a crear un agente con
  * https://notebook.google.com/
 
* Vamos a armar un agente / notebook con estos documentos
* https://raw.githubusercontent.com/estebancalabria/Intro-Ia/refs/heads/main/Cursos/2026-Jul-Exolgan/clase-uno/Readme.md
* https://raw.githubusercontent.com/estebancalabria/Intro-Ia/refs/heads/main/Cursos/2026-Jul-Exolgan/clase-dos/Readme.md
* https://raw.githubusercontent.com/estebancalabria/Intro-Ia/refs/heads/main/Cursos/2026-Jul-Exolgan/clase-tres/Readme.md
* https://raw.githubusercontent.com/estebancalabria/Intro-Ia/refs/heads/main/Cursos/2026-Jul-Exolgan/clase-cuatro/Readme.md
* https://raw.githubusercontent.com/estebancalabria/Intro-Ia/refs/heads/main/Cursos/2026-Jul-Exolgan/clase-cinco/Readme.md
* https://raw.githubusercontent.com/estebancalabria/Intro-Ia/refs/heads/main/Cursos/2026-Jul-Exolgan/clase-seis/Readme.md
* https://raw.githubusercontent.com/estebancalabria/Intro-Ia/refs/heads/main/Cursos/2026-Jul-Exolgan/clase-siete/Readme.md
* https://raw.githubusercontent.com/estebancalabria/Intro-Ia/refs/heads/main/Cursos/2026-Jul-Exolgan/clase-ocho/Readme.md
* https://raw.githubusercontent.com/estebancalabria/Intro-Ia/refs/heads/main/Cursos/2026-Jul-Exolgan/clase-nueve/Readme.md

* Una vez armado el notebbok podemos hacer preguntas como

```
Que herramientas de generacion de vieos vimos?
```

* Apretar todos los botones de la barra derecha

 
 ### Infografia resumen del curso

 <img width="2752" height="1536" alt="image" src="https://github.com/user-attachments/assets/686da738-6c24-4155-b00c-c43a7474b7ba" />


---
