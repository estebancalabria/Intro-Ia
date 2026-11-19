# 🔌 APIs e Integraciones con Modelos de Lenguaje

Los modelos de lenguaje (LLMs) como los utilizados por ChatGPT, Claude, Gemini o Grok pueden utilizarse de dos maneras principales:

1. **Desde una interfaz web**, donde una persona interactúa directamente con el modelo.
2. **Desde una API**, donde una aplicación se comunica con el modelo mediante código.

Comprender esta diferencia es fundamental cuando queremos pasar de **usar Inteligencia Artificial** a **integrarla dentro de nuestras propias aplicaciones, automatizaciones y agentes**.

---

## 🌐 De la interfaz web a la API

Cuando utilizamos herramientas como ChatGPT, Claude o Gemini desde el navegador, estamos utilizando una aplicación construida por el propio proveedor.

Por ejemplo:

| Proveedor | Experiencia interactiva | Plataforma para desarrolladores |
|---|---|---|
| OpenAI | ChatGPT | OpenAI API Platform |
| Anthropic | Claude | Anthropic Console / API |
| Google | Gemini | Google AI Studio / Gemini API |
| Microsoft | Microsoft Copilot | Microsoft Foundry / Azure OpenAI |
| xAI | Grok | xAI API |
| Mistral AI | Le Chat | La Plateforme / Mistral API |
| Groq | GroqCloud Playground | GroqCloud API |
| DeepSeek | DeepSeek Chat | DeepSeek API |
| Cohere | Playground | Cohere API |

> **Nota:** esta separación entre una "web pública" y una "plataforma para desarrolladores" es conceptual. Cada proveedor organiza sus productos y plataformas de manera diferente.

Cuando utilizamos la interfaz web, es el proveedor quien se ocupa de realizar la comunicación con el modelo.

Cuando desarrollamos nuestra propia aplicación, **nosotros debemos realizar esa comunicación mediante una API**.

---

## 🤔 ¿Qué es una API?

**API** significa **Application Programming Interface** (Interfaz de Programación de Aplicaciones).

Una API permite que diferentes aplicaciones puedan comunicarse entre sí de una manera definida y controlada.

En el contexto de la Inteligencia Artificial, una aplicación puede enviar una solicitud a la API de un proveedor para utilizar uno de sus modelos.

El flujo simplificado sería:

**Aplicación → API del proveedor → Modelo LLM → Respuesta → Aplicación**

Por ejemplo, nuestra aplicación podría enviar:

> "Explicá qué es Machine Learning en tres párrafos."

La API recibe la solicitud, la envía al modelo correspondiente y devuelve la respuesta generada.

Esto permite utilizar modelos de lenguaje **sin necesidad de interactuar manualmente con una interfaz web**.

---

## 🚀 ¿Qué podemos construir utilizando APIs de modelos de IA?

Al acceder programáticamente a los modelos podemos incorporarlos dentro de prácticamente cualquier aplicación o proceso.

Por ejemplo:

- 💬 Chatbots
- 🤖 Agentes de IA
- 📄 Procesamiento de documentos
- 🔎 Sistemas RAG
- 📊 Análisis de información
- 📝 Generación y transformación de contenido
- ⚙️ Automatizaciones
- 🌐 Aplicaciones web
- 📱 Aplicaciones móviles
- 🔄 Workflows
- 🧑‍💻 Herramientas para desarrolladores
- 🔗 Integraciones con otros sistemas

También podemos integrar estas APIs con plataformas como **GitHub Actions**, **Make**, **n8n**, **Power Automate** o nuestras propias aplicaciones.

Pero aparece una pregunta importante:

**¿Cómo sabe el proveedor quién está intentando utilizar su API?**

Ahí aparece el concepto de **API Key**.

---

# 🔑 ¿Qué es una API Key?

Una **API Key** es una credencial utilizada para identificar y autorizar a una aplicación cuando intenta acceder a determinados servicios mediante una API.

Podemos pensarla conceptualmente como una **llave de acceso**.

Cuando nuestra aplicación realiza una solicitud, envía la API Key junto con esa solicitud.

El flujo sería:

**Aplicación + API Key → API del proveedor → Modelo LLM → Respuesta**

El proveedor puede utilizar esa credencial para determinar:

- Quién está realizando la solicitud.
- Qué servicios puede utilizar.
- Cuánto está consumiendo.
- Qué límites tiene asignados.
- Qué proyecto o cuenta está asociado al consumo.
- Qué costos puede generar ese consumo.

Por este motivo, una API Key debe considerarse **información sensible**.

---

## 🔐 Una API Key no es nuestra contraseña

Es importante diferenciar ambos conceptos.

Una API Key normalmente **no es la contraseña que utilizamos para iniciar sesión en la plataforma del proveedor**.

La contraseña permite que una persona acceda a su cuenta.

Una API Key permite que una **aplicación o proceso acceda programáticamente a una API**.

Por ejemplo:

**Persona → usuario + autenticación → plataforma web**

mientras que:

**Aplicación → API Key → API**

---

## 🏢 Cada proveedor administra sus propias credenciales

No existe una API Key universal para acceder a todos los modelos de Inteligencia Artificial.

Cada plataforma administra sus propias credenciales.

Por ejemplo:

- `OPENAI_API_KEY`
- `ANTHROPIC_API_KEY`
- `GOOGLE_API_KEY`
- `GROQ_API_KEY`
- `MISTRAL_API_KEY`

También existen plataformas que ofrecen acceso a múltiples modelos mediante una misma infraestructura o API.

Por este motivo debemos distinguir entre:

**El modelo que queremos utilizar**

y

**El proveedor mediante el cual estamos accediendo a ese modelo.**

No siempre son necesariamente la misma empresa.

---

# 💰 API Key, consumo y costos

Cuando utilizamos una API de Inteligencia Artificial, el consumo puede generar costos.

Dependiendo del proveedor y del modelo utilizado, pueden intervenir factores como:

- Cantidad de tokens de entrada.
- Cantidad de tokens de salida.
- Modelo seleccionado.
- Cantidad de solicitudes.
- Imágenes, audio u otros tipos de contenido procesados.
- Herramientas o servicios adicionales utilizados.

Por eso una API Key no solamente representa acceso.

También puede estar asociada a **consumo y facturación**.

Si otra persona obtiene nuestra API Key y comienza a utilizarla, podría consumir recursos asociados a nuestra cuenta o proyecto.

---

# ⚠️ Nunca publiques una API Key

Una de las reglas más importantes cuando trabajamos con APIs es:

> **Nunca colocar una API Key directamente dentro del código que vamos a publicar.**

Por ejemplo, esto es una **mala práctica**:

```python
api_key = "mi-api-key-secreta"
```

Si posteriormente subimos ese archivo a un repositorio público de GitHub, nuestra credencial podría quedar expuesta.

Incluso eliminar posteriormente la línea del archivo puede no ser suficiente, ya que la credencial podría permanecer dentro del **historial de Git**.

Si una API Key fue publicada accidentalmente, debemos considerarla potencialmente comprometida y **revocarla o rotarla desde la plataforma correspondiente**.

---

# 🌱 Variables de entorno

Una alternativa habitual consiste en almacenar las credenciales utilizando **variables de entorno**.

Por ejemplo:

```text
OPENAI_API_KEY=...
ANTHROPIC_API_KEY=...
GROQ_API_KEY=...
```

Nuestra aplicación puede obtener la credencial desde el entorno en lugar de escribirla directamente dentro del código.

Conceptualmente:

**Código → Variable de entorno → API Key → API**

De esta manera podemos separar:

**Código**

de

**Credenciales**

---

## 📁 Archivos `.env`

Durante el desarrollo local también es común utilizar un archivo:

```text
.env
```

Por ejemplo:

```text
OPENAI_API_KEY=...
GROQ_API_KEY=...
```

La aplicación puede cargar esas variables cuando se ejecuta.

Sin embargo, existe una regla fundamental:

> **El archivo `.env` que contiene credenciales reales no debe subirse al repositorio.**

Por eso normalmente se agrega al archivo `.gitignore`:

```text
.env
```

También podemos incluir en el repositorio un archivo de ejemplo:

```text
.env.example
```

Por ejemplo:

```text
OPENAI_API_KEY=
GROQ_API_KEY=
```

Este archivo documenta qué variables necesita la aplicación **sin publicar ninguna credencial real**.

---

# 🏭 ¿Y en producción?

Las variables de entorno y los archivos `.env` son útiles para comprender el concepto y trabajar en entornos de desarrollo.

En escenarios profesionales existen mecanismos específicos para almacenar y administrar secretos.

Por ejemplo:

- **GitHub Actions Secrets**
- **Azure Key Vault**
- Servicios de administración de secretos de otros proveedores cloud
- Sistemas de gestión de secretos utilizados por las organizaciones

Una posible evolución sería:

**Laboratorio local → Variables de entorno → GitHub Secrets → Secret Manager / Azure Key Vault**

El principio sigue siendo el mismo:

> **Las credenciales deben mantenerse separadas del código.**

---

# ✅ Buenas prácticas

Cuando trabajes con API Keys:

- 🔐 Tratalas como información sensible.
- 🚫 No las escribas directamente dentro del código.
- 🚫 No las publiques en GitHub.
- 🚫 No incluyas archivos `.env` con credenciales reales en el repositorio.
- 🌱 Utilizá variables de entorno durante el desarrollo.
- 🔑 Utilizá mecanismos específicos de administración de secretos en producción.
- ♻️ Revocá o rotá una API Key si sospechás que fue comprometida.
- 📊 Revisá periódicamente el consumo asociado a tus credenciales.
- 💰 Configurá límites o alertas de consumo cuando el proveedor lo permita.
- 🧪 Cuando sea posible, utilizá credenciales diferentes para desarrollo y producción.
- 👤 Evitá compartir una misma credencial entre múltiples usuarios o aplicaciones.

---

# 🧠 La idea más importante

Utilizar ChatGPT, Claude, Gemini, Grok u otros servicios desde sus interfaces es solamente una de las formas de trabajar con modelos de lenguaje.

Cuando queremos construir nuestras propias soluciones necesitamos acceder a los modelos **programáticamente**.

Ahí aparecen tres conceptos fundamentales:

**LLM → API → API Key**

La **API** permite que nuestra aplicación se comunique con un servicio.

La **API Key** permite identificar y autorizar ese acceso.

Y una correcta **gestión de secretos** permite hacerlo de manera más segura.

Este es el punto de partida para comenzar a integrar modelos de Inteligencia Artificial dentro de nuestras propias aplicaciones, automatizaciones, workflows y agentes.
