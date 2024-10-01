# 🛠️ Laboratorio de Automatización con Make

En este laboratorio, aprenderás a crear una automatización utilizando [Make](https://www.make.com/en), conectando un webhook que captura eventos desde una URL y lo convierte en un evento en Google Calendar, todo mediante la herramienta de Make. ¡Vamos paso a paso!

---

## 1️⃣ Ir a Make y loguearse

1. Visita [Make](https://www.make.com/en) y haz login en tu cuenta.

---

## 2️⃣ Crear un Nuevo Escenario

1. En el menú principal, dirígete a la sección **"Scenarios"**.
2. Haz clic en **"Create a New Scenario"**.

---

## 3️⃣ Crear un Trigger con "Custom Webhook" 

### ¿Qué es un trigger? 
> Un **trigger** es el evento que da inicio a una automatización. En este caso, usaremos un webhook que se activará cuando recibamos una solicitud HTTP.

1. Selecciona **"Custom Webhook"** como el trigger.
2. En la ventana emergente, selecciona **"Create Webhook"** y nómbralo como `"Nuevo-Evento-Calendario"`.

---

## 4️⃣ Copiar la URL del Webhook

1. Después de crear el webhook, Make generará una URL única para ti. **Cópiala** al portapapeles.
   
> **Ejemplo:** `https://hook.us1.make.com/guztnfpt42xf7bacy1fg4faubjmmu862`

---

## 5️⃣ Ejecutar el Escenario

1. Haz clic en **"Run Once"** en la parte inferior de la pantalla para dejar el escenario listo para capturar solicitudes.
2. El escenario estará en espera de un evento que active el webhook.

---

## 6️⃣ Probar el Webhook

1. En otra pestaña del navegador, pega la URL copiada y agrégale un query string con un evento.
   
> **Ejemplo:** `https://hook.us1.make.com/guztnfpt42xf7bacy1fg4faubjmmu862?q=Cita con el medico el 3 de Octubre de 10 a 12`

2. Presiona Enter para enviar la solicitud al webhook.

---

## 7️⃣ Verificar la Ejecución del Escenario

1. Regresa a la pestaña de Make y verifica que el escenario haya capturado el evento correctamente.
2. Revisa los resultados obtenidos.

---

## 8️⃣ Convertir el Resultado a JSON

1. Vamos a trabajar con una API de Groq. Dirígete a [Groq](https://console.groq.com/keys) y genera una API Key.

> **Ejemplo de API Key:** `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`

---

## 9️⃣ Añadir un Módulo de Groq

1. Haz clic en el botón **"+"** a la derecha del trigger y selecciona **"Create Module"**.
2. Busca **"Groq"** y elige **"Create Chat Completion"**.
3. Crea una nueva conexión a Groq utilizando el nombre que prefieras y la API Key obtenida.

> La conexión aparecerá en el menú de conexiones y podrá ser reutilizada en otros escenarios.

---

## 9.2) Configurar el Modelo de Groq

1. Selecciona el modelo adecuado y, como prompt en el campo **"User"**, usa el siguiente texto:

> Genera un JSON para un evento que tenga los campos inicio, fin, nombre. El inicio y el fin deben tener fecha y hora en formato UTC. Genera el JSON a partir de este texto: {{1.q}}

2. En las opciones avanzadas, selecciona que la salida sea en formato **JSON**.

---

## 🔄 Ejecutar el Escenario Nuevamente

1. Haz clic en **"Run Once"**.
2. Regresa a la pestaña del navegador y repite el proceso de enviar la URL con el query string.
3. Verifica que el segundo módulo (Groq) haya generado el JSON correctamente.
4. **Copia el resultado al portapapeles** para usarlo en los siguientes pasos.

---

## 🔍 Parsear el JSON

1. Añade un nuevo módulo y selecciona **"Parse JSON"**.
2. Haz clic en **"Create Data Structure"** y elige la opción **"Generate"**.
3. Pega el JSON generado en el campo **"Sample Data"** y haz clic en **"Generate"**.
4. Revisa la estructura generada y haz clic en **"Save"**.
5. En el campo **"JSON string"**, selecciona la variable `result` del paso anterior.

---

## 🗓️ Crear un Evento en Google Calendar

1. Añade un nuevo módulo y selecciona **"Google Calendar"**.
2. Elige la opción **"Create an Event"**.
3. **Conéctate a tu cuenta de Google** para permitir la creación de eventos en tu calendario.

---

## 12.2) Configurar el Evento

1. **Calendar ID:** Selecciona tu calendario principal.
2. **Event Name:** Relaciona este campo con el nombre del evento extraído del JSON parseado.
3. **Start Date:** Asocia este campo con la variable de inicio del evento.
4. **End Date:** Asocia este campo con la variable de fin del evento.

---

## 🎉 ¡Wiii! Automatización Completa

¡Felicidades! Has creado una automatización que captura un evento desde un webhook y lo convierte en un evento de Google Calendar. Puedes reutilizar y modificar este flujo para muchas otras automatizaciones.

---
