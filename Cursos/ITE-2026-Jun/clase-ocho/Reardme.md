# Clase Ocho - 13 de Julio del 2026

# Repaso

* Agentes
  * Agentes conversacionales
    * Gems
    * Agentes de Copilot
      * Copilot Studio
  * Agentes automatizaciones
    * Power Automate / Power Apps
    * Make
    * N8n

---

# Vibe Codign

* Replit
  * https://replit.com/
* Lovable
  * https://lovable.dev/
* Bolt.new
  * https://bolt.new/
 
---

# IA Tradiciona

* A diferencia de la IA generativa la IA tradicional (Machine Learning) se encarga en hacer predicciones a partir de datos estructurado y por consiguiente poder explicar la relacion entre los datos
* Recursos
  * Teoria
    * https://www.instagram.com/p/C1ntRrRswAu/?img_index=1
  * Aprendizaje (Kaggle)
    *  https://www.kaggle.com/

## Setup

* Abrir una planilla de Google Sheets
* Instalar una extension https://simplemlforsheets.com/

## Ejercicio

> [!NOTE]
> A partir de los datos de un pasajero del titani quiero poder predecir si sobrevive o no y entender que variables son mas relevantes a la hora de evaluar la posibilidad de supervivencia

* Descargar el dataset del titanic
  * https://www.kaggle.com/datasets/brendan45774/test-file
  * Adentro te descargas un zip que tiene un archivo tested.csv
* Entendiendo los datos
    * Surived -> La columna que yo quiero predecir  -> Target, Label
    * Pclass, Sex, Age, SibSp,	Parch. Fare, Embarqued -> Features / Caracteristicas
    * PassengerID, Name, Ticket, Cabin -> Datos irrelevantes
* Preparar los datos
    * Elijo el label y los features
    * Convierto en numerico la columna
* Separar los datos de prueba de entrenamiento
    * Dusplicar la hoja con todos los datos
    * Eliminar de la columna "survived" el contenido de las primeras 35 filas
* Entrenar y Evaluar el modelo
    * Extensiones -> Simple ML For Sheets -> Start ->  Predict missing values
    * Elegimos el label
    * Elegimos las caracteristicas
    * Elegirmos el algoritmo
* Va a generar ls predicciones para las columnas faltantes
    * Si las constrastamos con la copia del libro que hicimos -> 100x100 efectividad
* Podes analizar los resultados
    * Sexo es la variable con mayor importancia

## ML con Python

*  Google Colab
  *  https://colab.research.google.com/drive/1r-eZ5BI-EGLMGfBEt_3Laudzi8sXT2RH?usp=sharing

* Prompt utilizado
```
Tengo este codigo de kaggle "import kagglehub


# Download latest version
path = kagglehub.dataset_download("brendan45774/test-file")


print("Path to dataset files:", path)". Voy a usar el daaset del titanic. Ademas hice el ejemplo en google sheets con estas intrucciones "* Descargar el dataset del titanic
  * https://www.kaggle.com/datasets/brendan45774/test-file
  * Adentro te descargas un zip que tiene un archivo tested.csv
* Entendiendo los datos
    * Surived -> La columna que yo quiero predecir  -> Target, Label
    * Pclass, Sex, Age, SibSp,	Parch. Fare, Embarqued -> Features / Caracteristicas
    * PassengerID, Name, Ticket, Cabin -> Datos irrelevantes
* Preparar los datos
    * Elijo el label y los features
    * Convierto en numerico la columna
* Separar los datos de prueba de entrenamiento
    * Dusplicar la hoja con todos los datos
    * Eliminar de la columna "survived" el contenido de las primeras 35 filas
* Entrenar y Evaluar el modelo
    * Extensiones -> Simple ML For Sheets -> Start ->  Predict missing values
    * Elegimos el label
    * Elegimos las caracteristicas
    * Elegirmos el algoritmo
* Va a generar ls predicciones para las columnas faltantes
    * Si las constrastamos con la copia del libro que hicimos -> 100x100 efectividad
* Podes analizar los resultados
    * Sexo es la variable con mayor importancia" Quiero el codigo en python para hacer lo mismo que hice en google sheets pero en python
```

* La IA me genero este codigo

```
# ============================================
# TITANIC - CLASIFICACIÓN SUPERVISADA
# Similar a Simple ML for Sheets
# ============================================

import pandas as pd
from sklearn.model_selection import train_test_split
from sklearn.ensemble import RandomForestClassifier
from sklearn.metrics import accuracy_score, classification_report

# ============================================
# 1. CARGAR LOS DATOS
# ============================================

df = pd.read_csv("tested.csv")

print("Filas:", len(df))
print(df.head())

# ============================================
# 2. SELECCIONAR FEATURES Y LABEL
# ============================================

features = [
    'Pclass',
    'Sex',
    'Age',
    'SibSp',
    'Parch',
    'Fare',
    'Embarked'
]

label = 'Survived'

# ============================================
# 3. LIMPIAR DATOS
# ============================================

# Edad faltante
df['Age'] = df['Age'].fillna(df['Age'].median())

# Tarifa faltante
df['Fare'] = df['Fare'].fillna(df['Fare'].median())

# Puerto de embarque faltante
df['Embarked'] = df['Embarked'].fillna(df['Embarked'].mode()[0])

# ============================================
# 4. CONVERTIR CATEGORICOS A NUMÉRICOS
# ============================================

df['Sex'] = df['Sex'].map({
    'male': 0,
    'female': 1
})

df['Embarked'] = df['Embarked'].map({
    'S': 0,
    'C': 1,
    'Q': 2
})

# ============================================
# 5. DEFINIR X e y
# ============================================

X = df[features]
y = df[label]

# ============================================
# 6. DIVISIÓN ENTRENAMIENTO / PRUEBA
# ============================================

X_train, X_test, y_train, y_test = train_test_split(
    X,
    y,
    test_size=0.35,
    random_state=42
)

print("Entrenamiento:", len(X_train))
print("Prueba:", len(X_test))

# ============================================
# 7. ENTRENAR MODELO
# ============================================

modelo = RandomForestClassifier(
    n_estimators=100,
    random_state=42
)

modelo.fit(X_train, y_train)

# ============================================
# 8. PREDECIR
# ============================================

predicciones = modelo.predict(X_test)

# ============================================
# 9. EVALUAR
# ============================================

accuracy = accuracy_score(y_test, predicciones)

print("\nAccuracy:")
print(f"{accuracy:.2%}")

print("\nReporte:")
print(classification_report(y_test, predicciones))

# ============================================
# 10. IMPORTANCIA DE VARIABLES
# ============================================

importancias = pd.DataFrame({
    'Variable': features,
    'Importancia': modelo.feature_importances_
})

importancias = importancias.sort_values(
    by='Importancia',
    ascending=False
)

print("\nImportancia de Variables:")
print(importancias)
```

---

# AI-900

* Inteligencia Artificial en la nube con Microsoft

 
* Azure Portal
  * Url
    * https://portal.azure.com/
  * Caracteristicas
  * Tiene un monton de servicios para desplegar aplicacion
    * Maqinas Virtuales
    * Bases de Datos
    
## Microsft Foundry

    * Los servicios de Azure que permiten crear Apllicaciones de IA
    * Tengo estos servicios:
      * Azure OpenAI
      * AI Search
      * Bot services
      * Computer vision
      * Custom vision
      * Content safety
      * Document intelligence
      * Face API
      * Health Insights
      * Machine Learning
      * Immersive reader
      * Language service
      * Speech service
      * Translator
    * Cada recurso de Azure de los anteriores se crea en el portal de Azure y se utiliza desde su portal especifico

### Machine Learning en Azure

* Una vez creado el recurso de ML puedo accer al portal especifico
  * https://ml.azure.com/

---

# NotebookLM

* URL
  * https://notebooklm.google.com/
