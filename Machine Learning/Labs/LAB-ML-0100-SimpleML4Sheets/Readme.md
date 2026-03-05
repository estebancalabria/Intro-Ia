# 🧪 LABORATORIO

# **Introducción al Machine Learning con Google Sheets**

## 🎯 Objetivo

Simular un escenario real de análisis de datos donde se utiliza **Machine Learning para predecir resultados a partir de información histórica**.

En este laboratorio los estudiantes utilizarán **Google Sheets + Simple ML for Sheets** para entrenar un modelo de Machine Learning que permita **predecir si un pasajero del Titanic habría sobrevivido o no**, utilizando variables demográficas y socioeconómicas.

El objetivo es comprender de forma práctica:

* Qué es un problema de **clasificación**
* Cómo se **prepara un dataset**
* Cómo se **entrena un modelo**
* Cómo se **evalúan predicciones**
* Cómo se interpretan las **variables más importantes del modelo**

---

# 🧩 Estructura del Laboratorio

---

## 0️⃣ Exploración Inicial — Problemas de Machine Learning

Antes de comenzar, reflexionar sobre distintos tipos de problemas que resuelve el Machine Learning.

Ejemplos comunes:

### Clasificación
Predecir una categoría.

Ejemplos:

* Clasificar imágenes (gato / perro)
* Predecir si un usuario verá o no una película
* Detectar si un correo es spam
* Clasificar pacientes de riesgo durante una pandemia

### Regresión
Predecir un valor numérico futuro.

Ejemplos:

* Predecir ventas futuras
* Estimar el precio de una casa
* Predecir cantidad de asistentes a un evento o curso

### Detección de Anomalías
Detectar comportamientos fuera de lo normal.

Ejemplos:

* Transacciones fraudulentas
* Comportamientos sospechosos en sistemas financieros
* Fallas en sensores industriales

El laboratorio que realizaremos corresponde a un **problema de clasificación**.

---

## 1️⃣ Obtención del Dataset

Para entrenar modelos de Machine Learning necesitamos **datos**.

Uno de los repositorios más importantes para aprender ML es:

https://www.kaggle.com/

Kaggle contiene miles de datasets reales utilizados en ciencia de datos.

Para este laboratorio descargar el siguiente dataset:

https://www.kaggle.com/datasets/brendan45774/test-file

Pasos:

1. Descargar el archivo ZIP
2. Descomprimirlo
3. Ubicar el archivo **tested.csv**

Este archivo contiene información de pasajeros del Titanic.

---

## 2️⃣ Importación de Datos en Google Sheets

Abrir **Google Sheets**.

Crear una nueva hoja de cálculo.

Luego:

File → Import → Upload

Subir el archivo:

tested.csv

Una vez importado, tendremos una tabla con distintas columnas que describen a cada pasajero.

---

## 3️⃣ Instalación de la Extensión de Machine Learning

Para poder entrenar modelos directamente en Google Sheets vamos a utilizar una extensión especializada.

Instalar:

https://simplemlforsheets.com/

Luego de instalarla:

1. Volver al Google Sheets
2. Refrescar la página
3. Verificar que aparezca en el menú:

Extensions → Simple ML for Sheets

Esta herramienta permite entrenar modelos sin necesidad de programar.

---

## 4️⃣ Comprender el Dataset

El dataset contiene múltiples columnas, pero **no todas son útiles para el modelo**.

Debemos clasificar las columnas en tres tipos:

### Label (Lo que queremos predecir)

Survived

Indica si el pasajero sobrevivió o no.

Este será el resultado que el modelo intentará predecir.

---

### Features (Variables que el modelo usará para aprender)

Pclass  
Sex  
Age  
SibSp  
Parch  
Fare  
Embarked

Estas columnas describen características del pasajero.

El modelo buscará patrones entre estas variables y el resultado de supervivencia.

---

### Columnas que descartamos

PassengerId  
Name  
Ticket  
Cabin

Motivos:

PassengerId  
Es solo un identificador.

Name  
Texto libre sin valor predictivo.

Ticket  
No tiene formato uniforme.

Cabin  
Tiene demasiados valores faltantes.

---

## 5️⃣ Preparación de los Datos

Antes de entrenar un modelo debemos asegurarnos de que los datos tengan el formato correcto.

Algunas columnas deben ser numéricas.

Seleccionar la columna **Fare**

Luego:

Format → Number

Repetir lo mismo con la columna **Age**.

Esto asegura que el modelo interprete los valores correctamente.

---

## 6️⃣ Separación de Datos de Entrenamiento y Prueba

Un paso fundamental en Machine Learning es **separar datos para evaluar el modelo**.

Primero:

Duplicar el documento completo para conservar una copia original.

Luego, en el archivo de trabajo:

Eliminar el valor de la columna **Survived** en los **primeros 15 registros**.

Esto significa que esos registros se usarán como **datos de prueba**.

El modelo intentará predecir esos valores.

Luego podremos comparar si acertó o no.

Es importante entender que en Machine Learning **no buscamos perfección**, sino modelos **lo suficientemente buenos para ser útiles**.

---

## 7️⃣ Entrenamiento del Modelo

Ahora entrenaremos el modelo.

Ir a:

Extensions → Simple ML for Sheets → Predict Missing Values

Configurar:

### Column With Missing Values

Survived

### Source Columns

Pclass  
Sex  
Age  
SibSp  
Parch  
Fare  
Embarked

Es importante verificar que las columnas estén identificadas como:

Num (numéricas)  
Cat (categóricas)

No deben aparecer como texto libre.

Luego presionar:

Predict

---

## 8️⃣ Interpretación de Predicciones

El sistema generará automáticamente una nueva columna:

Pred:Survived

Esta columna contiene **las predicciones del modelo**.

Comparar estos resultados con el archivo duplicado que contiene los valores reales.

El objetivo es observar:

* Cuántos aciertos tiene el modelo
* En qué casos se equivoca
* Qué tan útil podría ser este modelo

En este dataset el modelo suele funcionar muy bien.

Pero en la vida real **los modelos rara vez son perfectos**.

Cada organización debe decidir **qué nivel de precisión es aceptable para su negocio**.

---

## 9️⃣ Interpretar el Modelo

Más allá de las predicciones, también podemos entender **qué variables influyen más en el modelo**.

Ir a:

Extensions → Simple ML for Sheets

Start → Advanced Tasks → Understand a Model

Elegir el modelo entrenado.

Luego abrir la pestaña:

Variable Importance

Aparecerá algo similar a:

Variable Importance: INV_MEAN_MIN_DEPTH

1. Sex  
2. Fare  
3. Age

Esto indica que esas variables son las que más influyen en la predicción.

---

## 🧠 Reflexión Final

Este resultado coincide con un hecho histórico conocido del Titanic:

"Women and children first"

Las variables relacionadas con **sexo y edad** tuvieron un impacto directo en la probabilidad de supervivencia.

Esto demuestra cómo el Machine Learning puede **descubrir patrones en los datos que reflejan comportamientos del mundo real**.

---

# 🎯 Criterios de Evaluación

* Correcta importación del dataset
* Preparación adecuada de los datos
* Uso correcto de la extensión Simple ML for Sheets
* Comprensión del concepto de Features y Label
* Capacidad de interpretar las predicciones del modelo
* Capacidad de interpretar la importancia de variables
