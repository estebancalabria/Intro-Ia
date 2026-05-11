# Clase Nueve  - 11 de Mayo 2026

# Repaso

* Azure
  * AI Foundry
      * https://portal.azure.com/
          * Aqui se crea la cuenta y la subscripcion
      * Un conjunto de herramientas que se utilizan cunaod quiero desaroolar mi aplicacion de IA
      * Servicios de Agentes
          * Claude, ChatGPT, Gemini
          * https://ai.azure.com/
          * Agente
              * Chatbot que tiene System Prompt personalizado
              * Fuente de informacion especificada (como NotebookLM)
              * Configurar Hiper Parametros (Temperta, TopP)
          * Generar Imagenes, videos, audio
      * Servicios Especializados
        * Face APi
        * Computer Vision
        * Language Service
        * ...
          
---

# Ai-900

## Forma de Trabajo

* Administrador de Sistemas: El el portal creo el recurso para darselo a los Desarrolladores que crean la aplicacion
* Desarrollador : Mediante el portal especifico de cada recurso lo pureba
    * Agente ===> ai.azure.com
    * Machine Learning ====> https://ml.azure.com/
    * Otros servicios
      * Computer Vision ===> https://portal.vision.cognitive.azure.com/
      * Custo vision ====>  https://www.customvision.ai/
      * Language Service ====> https://language.cognitive.azure.com/
      * ...

## Servicio de Machine Learning

* Una vez que el administradro crear el recurso, el Cientifico de datos puede utilizarlo mediante
  * https://ml.azure.com/
* Los cientificos de Datos que trabajan con Machine Learning tiene 2 formas de trabajar
    * Con notebooks en python (programando)
    * Con herramientas No Code (arrastra y solantaldo)
* Lo primero que hay que hacer es reservar la cantidad de computo

* En un notebook de ML hicimos

```python
# ============================================
# EJEMPLO COMPLETO DE MACHINE LEARNING
# Predicción de precios de casas
# ============================================

# Importamos librerías
import pandas as pd

from sklearn.model_selection import train_test_split
from sklearn.linear_model import LinearRegression
from sklearn.metrics import mean_absolute_error

# ============================================
# 1. DATOS
# ============================================

# Dataset creado directamente en código
datos = {
    "metros": [50, 60, 80, 100, 120, 150, 200, 220, 250, 300],
    "habitaciones": [1, 2, 2, 3, 3, 4, 4, 5, 5, 6],
    "antiguedad": [30, 25, 20, 15, 10, 8, 5, 4, 3, 1],
    "precio": [
        50000,
        65000,
        90000,
        120000,
        150000,
        180000,
        250000,
        280000,
        320000,
        400000
    ]
}

# Convertimos a DataFrame
df = pd.DataFrame(datos)

print("========== DATASET ==========")
print(df)

# ============================================
# 2. FEATURES Y TARGET
# ============================================

# Variables de entrada
X = df[["metros", "habitaciones", "antiguedad"]]

# Variable objetivo
y = df["precio"]

# ============================================
# 3. TRAIN / TEST SPLIT
# ============================================

X_train, X_test, y_train, y_test = train_test_split(
    X,
    y,
    test_size=0.2,
    random_state=42
)

# ============================================
# 4. CREAR MODELO
# ============================================

modelo = LinearRegression()

# Entrenamiento
modelo.fit(X_train, y_train)

# ============================================
# 5. PREDICCIONES
# ============================================

predicciones = modelo.predict(X_test)

print("\n========== PREDICCIONES ==========")

for valor_real, valor_predicho in zip(y_test, predicciones):
    print(
        f"Real: {valor_real} | "
        f"Predicción: {round(valor_predicho, 2)}"
    )

# ============================================
# 6. EVALUACIÓN
# ============================================

error = mean_absolute_error(y_test, predicciones)

print("\n========== ERROR ==========")
print(f"Error promedio: {round(error, 2)}")

# ============================================
# 7. NUEVA PREDICCIÓN
# ============================================

# IMPORTANTE:
# Creamos DataFrame con nombres de columnas
# para evitar el warning de sklearn

nueva_casa = pd.DataFrame({
    "metros": [140],
    "habitaciones": [3],
    "antiguedad": [6]
})

precio_estimado = modelo.predict(nueva_casa)

print("\n========== NUEVA CASA ==========")
print(nueva_casa)

print("\n========== PRECIO ESTIMADO ==========")
print(round(precio_estimado[0], 2))
```

## Servicios Especializados

### Computer Vision

* https://portal.vision.cognitive.azure.com/
* Casos de Uso
  * Detectar Caras en una imagen
  * Verificar si es la persona del DNI
  * ...

 ## Language Service

* https://language.cognitive.azure.com/
* Casos de uso
   * Analisis de Sentimiento
   * Resumir Texto
   * Extraer informacion Sensible
   * Extraer entidades conocidas

 ## Custom Vision

 * https://www.customvision.ai/
 * Casos de uso
  * Entrenar un modelo de IA para que reconozca categoria de imagenes y las clasifique
