# Clase Seis - 1 de Octubre 2026

# Respaso

* Prompt Engineering
  * Utilizar a la IA como experto en prompt engineering
* Herramientas de Productividad (Modulo 4)
  * Gamma
    * Generar Presentaciones
    * Webs / Landings
    * Publicaciones para redes sociales
  * PowerPoint
    * Copilot para Powerpoint
  * HeyGen
    * Generacion de videos instucionales
    * Videos basados en Avatar
    * Utilizar nuestra voz y nuestra imagen
  * Lovable (Modulo 4 y 7)
    * Geenerar aplicaciones
    * Generar proptotipos con comportamiento
    * Permite hacer "vibe coding" -> Programar pero con lenguaje natural
    * Conectores : Con Excel, con google Sheets
  * Taqtic
    * Sppech-To-Text
    * HErramienta de transcripcion de audio/video
    * Es una de varias herramientas

---

# IA Generativa Creativa

## Generacion de Imagenes

### Prompt Engineering

* Recomendacion es que para generar imagenes utilicemos los prompts en ingles.

```
Dame el prompt para generar en gemini una imagen futurista de star wars en ingles
```

* Me genera este prompt

```
Generate a futuristic cinematic sci-fi image inspired by the visual aesthetic of epic space operas: a massive galactic city in the distant future, with monumental architecture, towering skyscrapers illuminated by neon lights, spacecraft flying between the buildings, enormous orbital stations visible in the sky, futuristic armored soldiers, and a mysterious warrior wielding a glowing red energy sword.

The scene should feel epic, technologically advanced, dark, and dramatic. Cinematic lighting, volumetric fog, reflections on metallic surfaces, neon lights, atmospheric particles, dramatic depth of field, panoramic composition, ultra-detailed, photorealistic, 8K, high contrast, realistic materials, epic sci-fi movie concept art.

Make it feel like a frame from a massive, high-budget futuristic space-opera movie rather than generic sci-fi artwork, with coherent world-building, sophisticated visual design, and an immense sense of scale.
```

### Modelos de Generacion

*  Modelos Propietarios
  *  NannoBannana (Google)
  *  Gpt-Image (ChatGPT)
  *  SeedDream
*  Modelos OpenSource
 *  Qwen-Image
 *  Flux

> [!NOTE]
> Se pueden consultar en Arena.AI

* Pueden ver una explicacion interesante del profe de como funcionan estos videos en el siguien enlace:
  * https://www.instagram.com/p/DRSGNZFgafh/

### Casos de uso

#### Generacion de Imagen desde texto

* Podemos generar imagenes desde Gemini o ChatGPT
* Tambien desde Qwen (OS)

* Gemini (NannoBannana)

```
Genera una imagen cinematográfica de ciencia ficción futurista inspirada en la estética de las grandes space operas: una enorme ciudad galáctica en el futuro, con arquitectura monumental, rascacielos iluminados con neón, naves espaciales volando entre los edificios, enormes estaciones orbitales visibles en el cielo, soldados con armaduras futuristas y un misterioso guerrero con una espada de energía roja. 

La escena debe transmitir una escala épica, tecnología avanzada y una atmósfera oscura y dramática. Iluminación cinematográfica, volumetric fog, reflejos en superficies metálicas, luces de neón, partículas en el aire, gran profundidad de campo, composición panorámica, ultra detailed, photorealistic, 8K, high contrast, realistic materials, epic sci-fi movie concept art.

Evita que parezca una ilustración genérica: debe sentirse como un fotograma de una superproducción cinematográfica futurista, con diseño visual coherente y gran nivel de detalle.
```

* Genero esta imagen

<img width="1024" height="559" alt="image" src="https://github.com/user-attachments/assets/53b8bcf2-63f3-4544-b970-821ce5c1b889" />

---

#### Generacion / modificacion de imagenes

* Basados en una imagen suya le pueden pedir a Gemini o cualquier chatbot una modificacion

<img width="1024" height="1024" alt="image" src="https://github.com/user-attachments/assets/3f5a79d9-63db-4a73-9757-12f940a29ea7" />

---

#### Generacion de imagen eligiendo el modelo

* Podemos generar imagenes con herramientas como
  * Leonardo
    * https://leonardo.ai/

> [!NOTE]
> Vale la pena explorarla
      
<img width="2560" height="1440" alt="image" src="https://github.com/user-attachments/assets/6664b286-7b8e-46f2-b31a-10f101df847e" />

---

#### Generacion de Imagenes con modelos Open Source

* Puedo usar Hugging Face
  * https://huggingface.co/spaces/black-forest-labs/FLUX.1-dev

<img width="1024" height="1024" alt="image" src="https://github.com/user-attachments/assets/6d396ad0-0d02-4402-8371-b690404ab9cd" />

---

#### Generacion de Imagenes con Texto

* Hoy en dia casi todos los modelos generan imagens con texto
* Pero el primero que lo hizo y es un modelo propietario se llama Ideogram
* Al profe le gustan mucho tambien las imagenes generadas con este modelo
 * Tiene su propia herramienta
   * https://ideogram.ai/

* Prompt Generado con IA
```
Generate a futuristic cinematic sci-fi image inspired by the iconic visual aesthetic of Star Wars: a massive galactic city in the distant future, with monumental architecture, towering skyscrapers illuminated by neon lights, spacecraft flying between the buildings, enormous orbital stations visible in the sky, futuristic armored soldiers, and a mysterious warrior wielding a glowing red energy sword.

**Integrate the exact text "STAR WARS" prominently into the composition**, using the franchise's classic, instantly recognizable logo typography: bold, geometric, uppercase golden-yellow lettering with the characteristic connected letterforms and proportions of the original Star Wars logo. The logo must be spelled correctly, clearly legible, and visually faithful to the classic franchise branding.

Make the logo feel like a natural, harmonious part of the cinematic composition rather than an element pasted on top. Position it prominently in the upper portion of the image, with subtle atmospheric integration, cinematic lighting, realistic glow, and carefully balanced contrast against the galactic background. Preserve the distinctive shape and proportions of the classic logo while ensuring excellent readability.

The scene should feel epic, technologically advanced, dark, and dramatic. Cinematic lighting, volumetric fog, reflections on metallic surfaces, neon lights, atmospheric particles, dramatic depth of field, panoramic composition, ultra-detailed, photorealistic, 8K, high contrast, realistic materials, epic sci-fi movie poster.

Create the visual impression of an authentic, high-budget space-opera movie poster, with sophisticated world-building, immense scale, dramatic visual hierarchy, and professional theatrical-poster composition.

**Important:** The words "STAR WARS" must be the only prominent text in the image. Do not add subtitles, taglines, credits, extra lettering, watermarks, or misspelled text. Prioritize accurate logo typography, visual harmony, and cinematic impact.
```

* Genero esta imagen

<img width="268" height="398" alt="image" src="https://github.com/user-attachments/assets/454df878-c65e-4ac6-910b-66694d6ca1f5" />

---

#### Generacion de Folleteria y 

* PAra este caso (como competencia de Canva) recomiendo
  * https://designer.microsoft.com/
 
* Generacion de Imagen comun

 <img width="1254" height="1254" alt="image" src="https://github.com/user-attachments/assets/43054205-51e3-411a-8c92-5a1f088917d5" />


* Generacion de una invitacion

> [!NOTE]
> Quedo pendiente porque no funciono la herramienta

----
# BREAK
# HAsta y 20
----

## Generacion de Vieos

## Generacion de Canciones
