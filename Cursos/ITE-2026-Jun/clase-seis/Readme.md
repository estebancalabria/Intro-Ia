# Clase Seis - 6 de Julio del 2026

## Repaso

* Large Language Models
  * Propietarios
    * Claude
      * Buena para tareas tecnicas como programar
* Prompt Engineering
  * Formato de Salida
    * Mermaid
      * Organigrama del Pais
      * Un diagrama de PIE
    * Codigo / Python
      * Libreria MatPlotLib
      * Tambien habiamos hecho el pong claude
* Agente
  * Tipos De Agente
    * Agentes Conversacionales
    * Agentes Autnomos
  * Partes de Un agente
    * LLM
    * Instruccion (System Prompt)
    * Funetes de Conocimiento (RAG)
    * Llamadas a herramientas
    * Orquestador
  * Contruimos un agente con Google Gems
    * Hicimos el ejemplod e La Panera Rosa
* Vibe Coding
   * https://replit.com/
* Herramientas
  * Para hacer Presentaciones, Webs, Publicaciones
    * Gamma
     
---

## Herramientas

### Generacion de Videos Instucionales

#### HeyGen

* URL
  * https://heygen.com/
* Caracteristicas
  * 3 videos de 1 minuto por mes
  * Puedo utilizar los avatars que vienen con la herramienta o puedo crear mi propio avatar
* Algunos Ejemplos
  * https://app.heygen.com/videos/llegada-a-la-luna-4fe57c7ee05c4340be90f26fa94d7f24
  * https://app.heygen.com/videos/cambio-climatico-1c6c4d3398ce4de0b06d707d99d87e30
  * https://app.heygen.com/videos/promocion-real-state-da89b82988ba4c0da266c61abac08896
  * https://app.heygen.com/videos/presentacion-0b8d0aa4a25449689be104e72a219cb0
 
* Vamos a hacer primero el script con ChatGPT

```
Quiero un script promocional para una empresa LC Paper que vende papel tisu. Es para generar un video basado en avatar de 1M. Devolverme el script sin emojis ni acotaciones directamente.
```

* ME genero esto:

```
En LC Paper creemos que un gran producto comienza mucho antes de llegar a las manos de nuestros clientes.

Somos una empresa especializada en la fabricación y comercialización de papel tissue, comprometida con ofrecer productos que combinan calidad, suavidad, resistencia y eficiencia para satisfacer las necesidades del mercado.

Trabajamos con tecnología moderna y procesos optimizados que nos permiten garantizar una producción confiable y altos estándares de calidad en cada etapa.

Nuestro compromiso también incluye la mejora continua, la innovación y el desarrollo de soluciones que aporten valor tanto a empresas como a consumidores.

Cada rollo de papel que producimos refleja el esfuerzo de un equipo que entiende la importancia de la excelencia, la responsabilidad y el servicio.

En LC Paper construimos relaciones de largo plazo basadas en la confianza, el cumplimiento y la calidad de nuestros productos.

Seguimos creciendo con una visión clara: desarrollar soluciones de papel tissue que acompañen a nuestros clientes hoy y en el futuro.

LC Paper. Calidad que se siente. Confianza que perdura.

```

* Copiamos el script en el chat de Hey Gen y elegimos al avatar "Ruben"

* Generamos este video
  * https://app.heygen.com/videos/publicidad-papel-tissue-6f96359cf8ff456bb6896dfebbc562e2

---

# IA Generativa Multimedia (IA Creativa)

## Imagenes

### Fundamentos

* Modelos
  * Propietarios
    * Nanno Bannana
    * GPT-Image (openAI)
  * Open Source
    * Wan

* Comparativa
 * https://arena.ai/leaderboard/text-to-image

* Tips
 * Los prompts para generar imagenes siempre son mejores en ingles. Usar chatgpt para generar el prompt

### Casos de Usos

#### Generacion Rapida de Imagenes

* Gemini y ChatGPT permite generar imagenes rapdamente

* Gemini  
<img width="1024" height="1024" alt="image" src="https://github.com/user-attachments/assets/d781ee95-cbb5-4bf7-9391-30f6ad26241a" />

* ChatGPT
<img width="1536" height="1024" alt="image" src="https://github.com/user-attachments/assets/419dd564-5dd2-4b8d-914e-800035a2b7c6" />


#### Generacion con Herramienta : Leonardo

* URL
  * https://leonardo.ai/
* Caracteristicas
   * Tiene muchas mas funcionalidades que las que vamos a ver en clase

* Prompt en ingles hecho con ChatGPT
```
A breathtaking, cinematic football showdown between Spain and Portugal moments before kickoff. In the center of the scene, **Lamine Yamal** and **Cristiano Ronaldo** stand face to face, locking eyes with absolute intensity, embodying the clash between the future and a living legend. Yamal wears Spain's iconic red jersey, while Cristiano wears Portugal's deep red kit, both illuminated by dramatic stadium floodlights. The packed stadium roars in the background, with thousands of fans waving Spanish and Portuguese flags, creating an electrifying atmosphere. Sparks, subtle smoke, and floating embers fill the air, enhancing the tension. The expressions are determined, emotional, and fearless. The image should convey destiny, rivalry, respect, and the magnitude of a historic international battle. Ultra-realistic sports photography, cinematic lighting, dramatic contrast, shallow depth of field, dynamic composition, emotional storytelling, premium FIFA World Cup promotional poster aesthetic, no text, no logos, no watermarks.
```

#### Generacion de Imagenes tipo Anime

* URL
  * https://pixai.art/

<img width="768" height="1280" alt="image" src="https://github.com/user-attachments/assets/bfb1c187-e98f-4d05-8f2c-d59272e713c6" /> 

#### Generacion de imagenes con Texto

* URL
  * https://ideogram.ai/
* Caracteristicas
  * Muy utilizada en publicidad por su buenos resultados en afiches publicitarios

```
A monumental, cinematic football poster capturing the ultimate clash between **Spain and Portugal**. Both national teams emerge from opposite ends of a legendary stadium tunnel under dramatic floodlights, surrounded by smoke, sparks, floating embers, and thunderous crowds waving Spanish and Portuguese flags. At the front of Spain, **Lamine Yamal** leads his teammates with fearless determination. At the front of Portugal, **Cristiano Ronaldo** marches with the confidence of a legendary captain. The atmosphere radiates destiny, pride, rivalry, and the weight of football history. The players are illuminated with dramatic rim lighting, while the stadium glows beneath a stormy evening sky. In the center of the composition, seamlessly integrated into the environment as if carved from glowing steel and illuminated by the stadium lights, appears the title: **"ESPAÑA VS PORTUGAL"** in massive cinematic lettering, bold, elegant, and perfectly blended into the scene—not floating or pasted, but part of the artwork itself. Hyper-realistic sports photography, blockbuster movie poster aesthetic, ultra-detailed faces, dynamic composition, dramatic contrast, volumetric lighting, emotional storytelling, premium World Cup atmosphere, no logos, no watermarks.
```

<img width="1024" height="576" alt="image" src="https://github.com/user-attachments/assets/809762c1-a502-4266-ba85-b34bd597ffe2" />

---

## Videos

### Fundamentos

* Modelos
 * Propietarios
   * Veo 3 (Google(
   * Sora (OpenAI)
   * Pollo
 * Open Source

* Comparativa
  * https://arena.ai/leaderboard/text-to-video

### Casos de Uso

#### Generacion Rapida de Videos

* Previamnete el mejor era Grok (pero ahora es pago)
  * https://grok.com/

#### Herramienta para elegir modelo

* URL
  * https://pollo.ai/invitation-landing?invite_code=dIOOD7
* Caracteristicas
  * Una de las mas utilizadas por los que  generan de contenido para redes 

* Otra herramienta

* URL

---

## Musica
