# 🤖 Laboratorio: Automatización con Google Sheets, Groq y Google Calendar usando Make

En este laboratorio, aprenderás a crear una automatización utilizando [Make](https://www.make.com/en) que:

1. Detecta nuevas filas en una hoja de cálculo de Google Sheets 🧾
2. Utiliza **Groq** para generar automáticamente un título creativo para el evento mediante IA 🤖
3. Crea un evento en Google Calendar 📆

¡Vamos paso a paso!

---

## 🧭 Resumen del flujo

| Paso | Acción |
|------|--------|
| 1️⃣ | Crear el documento de Google Sheets |
| 2️⃣ | Conectar Google Sheets con Make usando el módulo "Watch New Rows" |
| 3️⃣ | Utilizar Groq para generar el nombre del evento |
| 4️⃣ | Crear el evento en Google Calendar |
| 5️⃣ | Probar todo agregando nuevas filas |

---

## 🔐 1. Iniciar sesión en Make

1. Visita [Make](https://www.make.com/en) y accede con tu cuenta.

---

## 📄 2. Crear un documento de Google Sheets

1. Abre una nueva pestaña en Chrome y crea una hoja de cálculo de Google.
2. Agrega las siguientes columnas:
   - `Evento`
   - `Inicio`
   - `Fin`
3. Cambia el tipo de dato de las columnas **Inicio** y **Fin** a **Fecha y Hora**.
4. Asigna un nombre significativo a la hoja (por ejemplo: `Eventos Automatizados`).

---

## 📆 3. Abrir Google Calendar

1. En otra pestaña, abre [Google Calendar](https://calendar.google.com/) con la misma cuenta de Gmail.

---

## 🛠️ 4. Crear un nuevo escenario en Make

1. Vuelve a Make y dirígete a la sección **"Scenarios"**.
2. Haz clic en **"Create a new Scenario"**.

---

## 🧲 5. Agregar el Trigger "Watch New Rows" (Google Sheets)

1. Haz clic en el **"+"** y busca **"Google Sheets"**.
2. Selecciona **"Watch new rows"**.
3. Conecta tu cuenta de Google cuando se te solicite.

---

## ⚙️ 6. Configurar el trigger

1. Selecciona el archivo de Google Sheets que creaste.
2. Indica el nombre de la hoja correctamente (respetando mayúsculas y minúsculas).
3. Elige usar la primera fila como encabezado.

---

## ➕ 7. Agregar una fila de prueba

1. Completa una fila en tu hoja de Google Sheets.
2. Ingresa un evento, una fecha/hora de inicio y de fin.

---

## ▶️ 8. Ejecutar el escenario

1. Vuelve a Make y haz clic en **"Run once"**.
2. Verifica que el trigger se active y lea correctamente la fila.

---

## 🧩 9. Agregar una acción "Create an Event" (Google Calendar)

1. Haz clic en **"+"** después del módulo de Google Sheets.
2. Busca y selecciona **"Google Calendar" > "Create an event"**.
3. Reutiliza la conexión con tu cuenta de Gmail.

---

## 🧷 10. Parametrizar el evento

1. En el campo **Summary** o **Event name**, selecciona la variable `Evento`.
2. En **Start Date**, utiliza la variable `Inicio`.
3. En **End Date**, utiliza la variable `Fin`.

---

## 🔑 11. Obtener una API Key de Groq

1. Inicia sesión en [https://console.groq.com/keys](https://console.groq.com/keys).
2. Genera tu API Key. Ejemplo:

   ```
   gsk_xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
   ```

> **Nota:** Guarda tu API Key en un lugar seguro. No la compartas públicamente.

---

## 🤖 12. Agregar un módulo de Groq: "Create Chat Completion"

1. Haz clic en el botón **"+"** entre los módulos de Google Sheets y Google Calendar.
2. Busca **"Groq"** y selecciona **"Create Chat Completion"**.
3. Si es la primera vez que lo usas, haz clic en **"Add"** para crear una nueva conexión:
   - **Nombre de la conexión:** Elige un nombre descriptivo (por ejemplo, `Groq-Automatización`).
   - **API Key:** Ingresa tu clave de API de Groq (por ejemplo, `gsk_xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx`).

---

## ⚙️ 13. Configurar el módulo de Groq

1. **Model:** Selecciona el modelo `llama3-8b-8192`.
2. **Messages:**
   - **Item 1:**
     - **Role:** `user`
     - **Content:** Ingresa el siguiente prompt:

       ```
       Me gustaría generar un título para un evento de Google Calendar con el siguiente formato [Categoría]-[Nombre], donde la categoría puede ser Trabajo, Salud u Ocio, y que el nombre sea gracioso. Responder solamente el nuevo nombre del evento y nada más. El nombre del evento original es: {{1.Evento}}
       ```

3. **Response Format:** Selecciona `Text`.

---

## 🔁 14. Modificar el módulo de Google Calendar

1. En el módulo de **"Create an Event"** de Google Calendar:
   - **Event Name:** Reemplaza el valor anterior por la salida generada por el módulo de Groq (por ejemplo, `2.choices[0].message.content`).
   - **Start Date:** Mantén la variable `Inicio` del Google Sheets.
   - **End Date:** Mantén la variable `Fin` del Google Sheets.

---

## 🧪 15. Probar el flujo completo

1. Agrega una nueva fila en tu hoja de Google Sheets con un evento de prueba.
2. Vuelve a Make y haz clic en **"Run once"** para ejecutar el escenario.
3. Verifica que:
   - El módulo de Groq genere un nuevo nombre para el evento.
   - Se cree correctamente el evento en Google Calendar con el nombre generado.

---

¡Listo! Ahora tienes una automatización que utiliza inteligencia artificial para generar nombres creativos para tus eventos en Google Calendar. 🎉
