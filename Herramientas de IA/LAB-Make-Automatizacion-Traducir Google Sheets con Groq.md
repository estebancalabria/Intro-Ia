# 🛠️ Laboratorio: Automatización con Make y Groq 🌐

¡Bienvenido al laboratorio! En este ejercicio aprenderás a automatizar tareas utilizando Make, Google Sheets y la API de Groq. Sigue los pasos cuidadosamente y diviértete mientras automatizas. 🚀

---

## 📋 **Pasos del Laboratorio**

### 1️⃣ **Loguearse en Make**
1. Ingresa a [Make](https://www.make.com/) y accede con tu cuenta.
2. Explora las opciones disponibles para familiarizarte con la herramienta.

---

### 2️⃣ **Crear una Planilla de Google Sheets**
1. Abre Google Sheets y crea una nueva planilla. 
2. Dale un nombre descriptivo, como `Automatización Make`.

---

### 3️⃣ **Obtener una API Key de Groq**
1. Accede a tu cuenta de Groq.
2. Genera una API Key y guárdala en un lugar seguro para usarla más adelante.

---

### 4️⃣ **Crear un Escenario en Make**
1. En Make, selecciona la opción para crear un nuevo escenario.
2. Dale un nombre que describa tu flujo, como `Automatización de Traducciones`.

---

### 5️⃣ **Agregar un Trigger: "Add New Rows"**
1. Haz clic en el botón **`+`** dentro del escenario.
2. Elige Google Sheets como herramienta.
3. Selecciona el trigger **"Add New Rows"**.

---

### 6️⃣ **Crear una Conexión con Google Sheets**
1. Conecta tu cuenta de Google Sheets a Make.
2. Autoriza los permisos necesarios para acceder a tus archivos.

---

### 7️⃣ **Completar Parámetros del Trigger**
1. Selecciona:
   - **Archivo**: La planilla creada en el paso 2.
   - **Libro**: La hoja específica donde se agregarán los datos.

---

### 8️⃣ **Probar el Trigger**
1. Haz clic en **"Probar"** para asegurarte de que Make detecta los datos correctamente.

---

### 9️⃣ **Agregar un Nuevo Paso con Groq**
1. Haz clic en el botón **`+`** nuevamente.
2. Selecciona Groq como herramienta.
3. Elige la opción **"Create Chat Completion"**.

---

### 🔟 **Crear una Conexión con Groq**
1. Conecta Make con tu cuenta de Groq utilizando la API Key obtenida en el paso 3.

---

### 1️⃣1️⃣ **Configurar la Conexión a Groq**
1. Define los siguientes parámetros:
   - **Role**: `User`
   - **Content**: `Traducir el contenido de {{3.`0`}} al inglés. Solamente responder la traducción.`

---

### 1️⃣2️⃣ **Agregar un Nuevo Módulo: "Update a Row"**
1. Añade un nuevo módulo de Google Sheets.
2. Selecciona la opción **"Update a Row"**.

---

### 1️⃣3️⃣ **Completar el Módulo de Google Sheets**
1. Configura los siguientes parámetros:
   - **Row Number**: El número de fila correspondiente.
   - **Traducción**: Usa las variables generadas en los pasos anteriores.

---

### 1️⃣4️⃣ **Agregar Filas al Excel y Ejecutar la Automatización**
1. Ingresa nuevas filas en la planilla de Google Sheets.
2. Ejecuta el escenario en Make y observa cómo se completan automáticamente las traducciones. 🎉

---

## 🎯 **¡Misión Cumplida!**
Ahora has creado una automatización completa con Make, Google Sheets y Groq. Practica agregando más pasos y experimenta con nuevas configuraciones. 🚀
