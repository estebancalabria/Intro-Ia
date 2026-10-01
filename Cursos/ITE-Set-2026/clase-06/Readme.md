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

> [!NOTE]
> PAra usar NanoBannana en forma ilimitada (cuando la interfaz de gemini no es suficiente) lo podemos hacer en google flow https://flow.google.com/?

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
# BREAK Hasta y 20
----

## Generacion de Videos

### Modelos de Generacion de Video

* Modelos Propietarios
 * Pollo
 * SeedDream
 * Sora
* Modelos Open Source
 *  Wan

### Proceso de Generacion de videos

* La IA genera video cortos, 5 o 10s.
  * Para generar con IA videos largos lo que se haces tomar todos los video cortos y compaginarlos con editor de videos
  * Como editor de video suelo usar https://www.capcut.com/
* Asi con esta forma hicimos un video (triste) con alumnos
  * https://www.youtube.com/watch?v=vPwCdejOuio
  * La cancion tambien esta integramente generada por IA

---

### Generacion de videos a Partir de Imagenes

* URL
  * https://redirect.inviteurl.app/invitation-landing?invite_code=dIOOD7
* Caracteristicas
 * Te permite elegir el video
 * Trae el modelo Pollo que es economico

* Generamos este viceo
 * https://pollo.ai/v/cmupti2ww5tiljd6picdldfnk?source=share

---

### Generacon de videos a partir de texto

* URL
  * https://pixverse.ai/es

> [!NOTE]
> Recomiendo de todas maneras siempre partir de una imagen. Te da mas control y te permite saber de ante manos que de va a generar. Tener en cuenta que la generacion de videos es muy exigente a nivel recursode GPU

* Prompt con IA:
```
Create an epic, cinematic sci-fi video inspired by the iconic visual universe of Star Wars, resembling a high-budget theatrical movie trailer.

SCENE AND ENVIRONMENT:
A vast futuristic galactic city stretches across the horizon, featuring monumental architecture, towering skyscrapers illuminated by neon lights, massive orbital stations, and enormous spacecraft moving between the buildings. Futuristic armored soldiers patrol elevated platforms while a mysterious warrior holding a glowing red energy sword stands on a rooftop overlooking the city. Multiple spacecraft fly through the atmosphere as distant explosions illuminate the skyline.

CAMERA MOVEMENT:
Begin with a breathtaking wide shot of the galactic city from above. Slowly descend between colossal skyscrapers as flying spacecraft pass close to the camera. Transition into a smooth cinematic tracking shot following a futuristic spacecraft through the city. The camera then moves toward the mysterious warrior standing on a rooftop, with the red energy sword gradually illuminating the surrounding fog. Finish with a dramatic pullback revealing the immense scale of the futuristic metropolis and the spacecraft filling the sky.

STAR WARS LOGO:
Integrate the exact text "STAR WARS" into the final composition using the franchise's classic, instantly recognizable logo typography. Preserve the distinctive bold, geometric, uppercase yellow lettering, characteristic connected letterforms, and original proportions. The logo should emerge harmoniously from the cinematic atmosphere, becoming clearly visible against the galactic background. Use subtle golden illumination, atmospheric depth, and carefully balanced contrast. The logo must remain stable, correctly spelled, and clearly legible, without warping, flickering, or morphing.

VISUAL STYLE:
Epic space opera, futuristic galactic civilization, monumental architecture, advanced spacecraft, dramatic red energy sword, cinematic volumetric lighting, atmospheric fog, realistic metallic reflections, glowing neon details, distant stars, subtle lens flares, immense sense of scale, photorealistic materials, sophisticated visual effects, high contrast, dramatic composition, premium Hollywood sci-fi cinematography.

MOTION AND QUALITY:
Fluid, natural camera movement, realistic spacecraft acceleration, convincing depth and parallax, atmospheric particles drifting through the scene, dynamic but controlled lighting, seamless transitions, consistent architectural details, and physically believable motion. Every element should feel like part of a coherent, living science-fiction universe.

ENDING:
Conclude with a powerful, cinematic hero shot of the galactic city at night. The camera slowly pulls back as spacecraft cross the illuminated skyline. The classic yellow "STAR WARS" logo appears prominently in the center of the frame, perfectly integrated into the scene. Hold the final composition long enough for the logo to be clearly read.

FORMAT:
Cinematic widescreen 16:9, 4K visual quality, 24 fps film aesthetic, rich blacks, dramatic highlights, smooth motion, professional movie-trailer production value.

IMPORTANT CONSTRAINTS:
Display only the exact words "STAR WARS" as prominent text. No subtitles, no taglines, no additional lettering, no credits, no watermarks. Avoid distorted typography, flickering logos, inconsistent objects, abrupt camera movements, artificial-looking CGI, and visual glitches. Prioritize cinematic coherence, smooth animation, and accurate, readable logo typography.
```

* Generamos estos videos :
  * https://app.pixverse.ai/video/427529235386837
  * https://app.pixverse.ai/video/427529200119173
  * https://app.pixverse.ai/video/427529002664406
  * https://app.pixverse.ai/video/427529233252848

---

### Generacion de videos Gratis

* Recomendaciones
  * Usar el chat de Qwen con la opcion de video
     * https://chat.qwen.ai/
     * Tarda bastante en generar el video
     * Son videos de calidad moderada
     * Generamos este video
        * https://chat.qwen.ai/s/t_f92b37b9-902c-445e-b7e8-d8cd677ffe00
  * Usar el generador de videos en Arena.ai
    * https://arena.ai/
    * No te deja elegir el modelo
    * Tarda mucho en generar
    * No encontre el limte de uso

----
# BREAK Hasta y 15
----
 

## Generacion de Canciones

* Hay Dos Alternativas top del mercado hoy
  * https://www.udio.com/home
  * https://www.udio.com/

* Vamos a generar una cacion pop de amor

```
**DONDE ESTÁS VOS**

**Verso 1**
Te vi llegar sin avisar,
como una canción en la radio,
yo que juraba no volver
a enamorarme de nadie.

Y ahora la ciudad parece
un poco más linda al caminar,
porque entre tanta gente
solo te quiero encontrar.

**Pre-coro**
Y no sé cómo explicarlo,
pero pasa cuando estás,
el mundo baja el volumen
y mi corazón te escucha más.

**Coro**
Donde estás vos,
quiero estar yo,
aunque se apague el mundo alrededor.
Si me das tu mano,
no pregunto dónde vamos,
porque mi lugar
es donde estás vos.

Donde estás vos,
late mi voz,
se me olvida todo lo que fui antes de los dos.
Y si mañana cambia el cielo,
si se pierde la dirección,
yo voy a encontrarte
donde estás vos.

**Verso 2**
Tenemos noches para hablar
y mil secretos que inventar,
un par de sueños imposibles
que algún día van a pasar.

Y cuando me mirás así,
no necesito nada más,
porque hasta el miedo se hace pequeño
si te quedás.

**Pre-coro**
Y no sé cómo explicarlo,
pero pasa cuando estás,
el mundo baja el volumen
y mi corazón te escucha más.

**Coro**
Donde estás vos,
quiero estar yo,
aunque se apague el mundo alrededor.
Si me das tu mano,
no pregunto dónde vamos,
porque mi lugar
es donde estás vos.

**Puente**
Y si la vida nos cambia el plan,
si alguna vez nos hace dudar,
mirame a los ojos una vez más,
que yo te vuelvo a elegir igual.

**Último coro**
Donde estás vos,
quiero estar yo,
que nos encuentre juntos el amanecer.
Si me das tu mano,
yo me quedo a tu lado,
porque mi lugar
es donde estás vos.

Donde estás vos...
donde estás vos...
si estás conmigo,
todo puede ser mejor.

**Outro**
Y aunque se apague el mundo alrededor,
yo voy a encontrarte...
donde estás vos.

```

* Prompt para la musica

```
Modern emotional pop love song, catchy and radio-friendly, with a powerful romantic atmosphere. Male lead vocal, warm, expressive and intimate in the verses, building into a big, memorable and uplifting chorus.

Contemporary pop production with piano and soft atmospheric synths at the beginning, gradually adding deep bass, punchy drums, subtle electric guitar and cinematic layers. Strong dynamic build from the verses into an explosive chorus designed to be instantly singable.

Tempo around 105 BPM, 4/4. Major key with emotional chord progressions and a bittersweet touch. The chorus should feel euphoric, romantic and anthemic, with layered backing vocals and harmonies.

Structure: short atmospheric intro, verse, pre-chorus with increasing tension, huge chorus, second verse, pre-chorus, chorus, emotional bridge with reduced instrumentation, final chorus bigger than the previous ones, and a memorable outro.

Overall sound: polished 2020s mainstream pop, cinematic but not overly orchestral, emotionally sincere, energetic, romantic, catchy and suitable for a major radio hit. Avoid excessive vocal effects, EDM drops, reggaeton rhythms, or overly complex instrumentation.


```

* SUno genero
  * https://suno.com/s/jIeOfbMjEMgSHlqB
  * https://suno.com/song/56644c84-634a-4918-8180-0a5c0447ac65?sh=X3m8SdUoUJrx41M7
  * https://suno.com/song/9d212906-a877-4db4-903a-aa09bcc4960d?sh=qUWU9ShsZk8Oh5qS
  * https://suno.com/song/18a4e35d-bc6c-4556-b2a4-3f5b2fcfaf8c?sh=6JtqpbR3nlDvvHv3
* Udio
 * https://www.udio.com/songs/h5yXzRiXh4DRL4RSwqJbHu?utm_source=clipboard&utm_medium=text&utm_campaign=social_sharing
 * https://www.udio.com/songs/bcs1c6FHb7TxMssaqdxBUF?utm_source=clipboard&utm_medium=text&utm_campaign=social_sharing
* Otra herramienta (mureka) que el profe no conoce
  * https://www.mureka.ai/song-detail/164001619116033?source=switch

> [!NOTE]
> Nos quedamos con Suno
