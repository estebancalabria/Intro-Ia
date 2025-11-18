# Clase Cinco - 18 de Noviembre del 2025

# Resumen

* Herramientas
  * Text-To-Speech : Natural Readers (https://www.naturalreaders.com/)
  * Speech/Vide0-To-Texto : Taqtic (https://tactiq.io/es)
  * Video Youtube-To-Texto : Unlimited Summary Generator for YouTube (https://chromewebstore.google.com/detail/unlimited-summary-generat/eelolnalmpdjemddgmpnmobdhnglfpje)
  * Clonar Voces : ElevenLabs (https://elevenlabs.io/)
  * Napkin : (https://www.napkin.ai/)
  * **NotebookLM** (La herramienta del momento) : https://notebooklm.google.com/
  * Compendio herramientas
      * https://theresanaiforthat.com/
      * https://huggingface.co/spaces
* La IA por dentro
  * Uso de la API Key desde Google Colab en Python con Groq (que es gratis)
  * Usar un LLM localmente
      * LMStudio
      * Ollama

# Uso de la API Key desde Javascript

* Ir a console.groq.com y sacamos una api key
* Ir a Claude y usar el siguiente prompt

```prompt
Quiero un artefacto (html+javascript) que sea un chatbot con groq. Arriba tiene un input para ingresar la api key de groq. Una vez que ingresaste y activaste la api key te permite chatear con groq. Te paso un ejemplo de la pagia de groq "import OpenAI from "openai";
const client = new OpenAI({
    apiKey: process.env.GROQ_API_KEY,
    baseURL: "https://api.groq.com/openai/v1", });  const response = await client.responses.create({     model: "openai/gpt-oss-20b",     input: "Explain the importance of fast language models", }); console.log(response.output_text);" aunque creo quen este caso lo vas a hacer directamtente con fetch. Generame el artefacto.
```

* Me genera el siguiente enlace del artefacto:

> https://claude.ai/public/artifacts/a4c46632-5185-43f2-be6a-18bb2f30b99c

* Poner la API key y probar
  

# IA Generativa Multimedia : Generacion de Imagenes
