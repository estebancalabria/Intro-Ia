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

**(Por Politicas el artefato no funciona desde claude lo tuve que bajar y ejecutar localmente)**

> https://github.com/estebancalabria/Intro-Ia/blob/main/Cursos/81553-Mar-Jue-Ta/clase-cinco/groq-chatbot.html

* Poner la API key y probar
  
# IA Generativa Multimedia : Generacion de Imagenes

> TIP Importante : Los prompts pa generar imagenes mejor en ingles en cualquier modelo. Generar los prompts con ChatGPT
> TIP Importante : Las herramientas que mostramos tienen muchas mas funcionalidades que las que vemos en clase, los invito a explorarlas en profundiad

* Casos de Uso generacion de Imagenes

- ## Generar Imagenes localmente (todas las que quiero gratis)

**No se hace con LMSudio**

  * Fooocus
      * https://github.com/lllyasviel/Fooocus?tab=readme-ov-file
  * Confy
      * https://www.comfy.org/
  * Automatic1111
      * https://github.com/AUTOMATIC1111/stable-diffusion-webui
  * Google Colab o python

- ## A partir de texto (prompt)
       * Gemini (Nano Banana)
       * ChatGPT
       * La de Whatsapp
       * Leonardo AI (https://leonardo.ai/)
          * Puntaje 9/10 (Si la probamos mejor tal vez un 10)
  
```prompt
Epic battle between Goku and Superman, ultra-detailed, dynamic action scene, intense energy clash, Goku in Super Saiyan form powering up a Kamehameha, Superman charging his heat vision, dramatic lighting, explosive background, cinematic angle, wind and debris flying, muscles detailed, realistic anime-comic hybrid style, hyper-realistic, 8k, ultra-sharp, legendary showdown, highly dramatic, vibrant colors, epic atmosphere
```

 - ## Imgagenes con Texto (prompt)

* Leonardo AI (https://leonardo.ai/)
* Ideogram (https://ideogram.ai/)
  * Puntaje 9/10

```prompt
Mouthwatering gourmet chorizo sandwich (Argentinian choripan), juicy grilled sausage in artisan bread, fresh chimichurri dripping, styled like high-end food photography, cinematic lighting, ultra-realistic, glossy texture, delicious and tempting. Big bold central text: “CHORIPAN GOURMET” — premium food advertisement, elegant typography, modern style, 8k, high detail, professional food ad
```

- ## Modificacion Imagen Existente

  * Nano Banana : https://gemini.google.com/app (Modelo Fast)
  * Groq : groq.com

Cargar dos imagenes y usar el siguiente prompt
```prompt
Place both people in the same image with a modern and elegant background. Make their posture look natural, standing slightly closer to each other and both looking at the camera. Maintain a consistent color tone so they appear on the same layer.
```
    
```prompt
Quisiera que cambies el escenario total de la foto, por un paisaje de una playa de ensueño, con un mar increible de aguas cristalinas y transparentes, misma postura de la fotografia, el cielo con un azul europeo nitido con luces y sombras que iluminan a la modelo, con un desenfoque de una camara DSRL de 85mm, que tenga armonia el cuerpo, toda la foto que sea con sombras naturales de un dia soleado, El cabello es largo y liso con un peinado natural; maquillaje suave pero llamativo con brillo en la piel. La foto debe estar tomada con una camara DSRL con flash, replicando el estilo característico de esta cámara: iluminación directa y cálida, el sujeto iluminado con flash, colores intensos y un estilo editorial-glamoroso. Alta resolución, realismo fotográfico, conservar los detalles del rostro y facciones sonriendo un poco
```

Para hacer un GEM que genere imagenes tuyas poner lo siguiente :
"
Primero analizarás todas las fotos que tienes almacenadas en conocimientos Luego generarás una imagen de esa persona en la situación que te pide el usuario.

Repite este proceso para TODAS la interacciones que en una misma conversación empiecen por:  "Enzo"
"
(Prompt de GEM)

Puntaje : 10 / 10
 
- ## Generacion de Imagenes Hiper Realistas

* ImageFX (de Google)
    * https://labs.google/fx/
    * https://labs.google/fx/tools/image-fx
       
```
Hyper-realistic image of a teacher giving a class, standing at a chalkboard with complex diagrams and notes, expressive hand gestures, engaging facial expression, intelligent and inspiring atmosphere, students focused in the background, natural classroom lighting, professional attire, academic environment, ultra-detailed, photorealistic, 8k
```

- ## Generacion de Disenios (Ademas de imagenes)

* Orientado a ser complemnetario o reemplazo de Canva
  * https://designer.microsoft.com/
    * Puntaje 10/10



