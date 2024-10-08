# 🛠️ Generación de ChatBots con OpenAI y Botpress

## 1️⃣ Introducción

En este laboratorio, aprenderás a crear y configurar un asistente de chatbot utilizando la plataforma OpenAI, integrándolo luego en Botpress para darle un frontend accesible. Al finalizar, tendrás un asistente funcional capaz de interactuar con los usuarios, responder preguntas y guiarlos en sus consultas.

Los chatbots son herramientas clave en la atención al cliente y en las ventas, ya que permiten automatizar interacciones y ofrecer respuestas rápidas y efectivas. ¡Vamos a empezar!

---

## 2️⃣ Programación del Asistente en OpenAI

A continuación, te explicamos los pasos para crear un asistente desde la plataforma de OpenAI.

### 2.1 Acceder a OpenAI

- Dirígete a [OpenAI Platform](https://platform.openai.com/) y regístrate si aún no lo has hecho.

### 2.2 Configuración Inicial

- Haz clic en la **Ruedita (Settings)** en la parte superior derecha de la pantalla.

### 2.3 Cargar Créditos (Opcional)

Para asegurarte de tener créditos disponibles para usar el servicio:

1. **Organización y Facturación**
   - Ve a la sección **Organization** > **Billing**. Asegúrate de que tengas créditos disponibles.

2. **Métodos de Pago**
   - Si deseas agregar créditos, ve a la pestaña **Payment Methods**. Allí puedes agregar una tarjeta, por ejemplo, de **Mercado Pago**.

3. **Agregar Créditos**
   - En la pestaña **Overview**, selecciona el botón **Add To Credit Balance** para cargar más créditos.

### 2.4 Crear el Asistente

- Haz clic en **Dashboard** en la parte superior y luego en **Assistants** en la barra lateral izquierda.
- Presiona el botón **Create** en la parte superior derecha.

> **Nota:** Los asistentes son personalizaciones de un modelo GPT con un propósito específico y tienen:
> - Un nombre
> - Un prompt especial
> - Acceso a una base de conocimiento
> - Capacidad para acceder a sistemas externos mediante una API (tools)

### 2.5 Configuración del Asistente

Vamos a crear nuestro asistente llamado **Mike**:

- **Nombre:** Mike  
- **Instrucciones del Sistema:** Eres Mike, un simpático vendedor de ropa con conocimientos de moda. Tienes la capacidad de encontrar la prenda ideal para cada perfil. Tu objetivo es informar al cliente sobre las prendas disponibles y sus precios. No hagas ninguna oferta y sé persuasivo para que la gente quiera visitar el local (Avellaneda 1600, CABA). Si te hablan de temas fuera de la ropa, declina la conversación.

### 2.6 Agregar Base de Datos de Conocimiento

- Carga la base de datos de conocimiento (prendas y precios).  
- Copia el archivo adjunto **Ropa.txt** y habilita la opción **File Search**.  
- En **+Files**, adjunta el archivo **ropa.txt**.

```
Catalogo de Prendas 

Remera Estampada S     Precio : 1000
Remera Estampada M     Precio : 1200 
Remera Estampada L     Precio : 1300
Remera Estampada XL    Precio : 1500

Pantalon Jean 40     Precio : 1000
Pantalon Jean 42     Precio : 1200 
Pantalon Jean 44     Precio : 1300
Pantalon Jean 48    Precio : 1500

Camisa S     Precio : 1000
Camisa M     Precio : 1200 
Camisa L     Precio : 1300
Camisa XL    Precio : 1500

Buzo S     Precio : 1000
Buzo M     Precio : 1200 
Buzo L     Precio : 1300
Buzo XL    Precio : 1500

Campera S     Precio : 1000
Campera M     Precio : 1200 
Campera L     Precio : 1300
Campera XL    Precio : 1500

Chomba S     Precio : 1000
Chomba M     Precio : 1200 
Chomba L     Precio : 1300
Chomba XL    Precio : 1500

Shorts S     Precio : 1000
Shorts M     Precio : 1200 
Shorts L     Precio : 1300
Shorts XL    Precio : 1500
```

### 2.7 Elegir el Modelo

- Selecciona el modelo **gpt-4o-mini** para tu asistente.

### 2.8 Probar el Asistente

- Dirígete a la opción **Playground** en la parte superior, luego a **Assistants**, y elige el asistente que creaste.
- **⚠️ Advertencia:** Si no tienes créditos cargados, recibirás un error.

### 2.9 Guardar el ID del Asistente

- Al crear el asistente, verás un ID con el formato **asst_....**. ¡Cópialo, lo necesitarás más adelante!

### 2.10 Obtener la API Key

- Ve a **Dashboard** > **Api Keys** y selecciona **+ Create new secret key**.  
- Asegúrate de copiar esta clave para usarla después.

---

## 3️⃣ Crear un Frontend para el Asistente

Ahora que tienes tu asistente en OpenAI, es hora de darle un frontend con **Botpress**.

### 3.1 Acceder a Botpress

- Visita [Botpress](https://botpress.com/) y loguéate con tu cuenta de Google.

### 3.2 Crear un Bot

- Haz clic en el botón **Create Bot**. Se generará un bot con un nombre aleatorio. Selecciona la ventana emergente **Open in Studio**.

### 3.3 Comenzar desde Cero

- Elige **Start from Scratch** y **Use Template** en la pantalla emergente.

### 3.4 Importar el Workflow

Para obtener las instrucciones sobre cómo crear un asistente, visita el siguiente enlace: [Botpress Blog](https://botpress.com/blog/deploy-openai-assistant-website).

- En el paso 2, encontrarás el workflow programado en este enlace:

  [Abrir Workflow Programado](https://studio.botpress.cloud/?install=hsk-098f7a89b1&_gl=1*1yvufe2*_gcl_au*OTAzMTkzNzIxLjE3Mjc0NTIwMjk.*_ga*MTA0MTUxNjM0OS4xNzI3NDUyMDMw*_ga_HKHSWES9V9*MTcyODM5NTA5My44LjEuMTcyODM5NTYzNy42MC4wLjg2NjAyNTE5Mw..)

- Haz clic en el enlace y selecciona **Install Workflow**.

### 3.5 Comprobar el Workflow

- A la derecha, en el mundo, busca **Card Hub**. Si haces clic, debería aparecer el workflow **Open AI Assistant API**.  
- Asegúrate de que el workflow esté instalado y selecciona **Make a copy and edit**.

### 3.6 Programar el Chatbot

- Ve a la opción **Flows** en la parte inferior (el ícono de la casita). Allí encontrarás **Open AI Assistant API - Copy**.
- En esta pantalla, podrás programar visualmente el chatbot y probarlo en la barra de chat de la derecha.

### 3.7 Limpiar los Nodos

- Borra todos los nodos, dejando solo el nodo de **START**. Haz clic derecho en cada nodo y selecciona **Delete Node**.  
- Si pruebas el chatbot ahora, mostrará el mensaje: "Sorry, an error occurred. Please try again later."

### 3.8 Conectar el Workflow

- Desde el nodo **START**, arrastra y selecciona **Execute Workflow**. En el menú emergente, elige el workflow **OpenAI Assistant API - Copy**.

### 3.9 Configurar Variables del Workflow

- Haz doble clic en el workflow creado a la derecha. Abajo, deberías ver **Workflow Variables**.  
- Busca **assistantID** y edítalo con el lápiz, colocando el ID del asistente que copiaste antes en **Default Value** (bajo **Additional Settings**).

- Repite los mismos pasos para **openAItoken**.

### 3.10 Probar el Asistente

- Prueba el asistente en el chat de la derecha seleccionando **New Conversation** y escribiendo "Hola". 

### 3.11 Publicar el Bot

- Finalmente, publica el bot para asegurarte de que funcione online. ¡Y listo! 🎉

---
