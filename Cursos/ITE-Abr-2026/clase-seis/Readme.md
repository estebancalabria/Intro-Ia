# Clase Seis - 5 de Abril del 2026

# Repaso

* Prompt Engineering
  * Personalizacion de Salida
    * Generacion y analisis de Datos
      * Python y MatPlotLib
* Herramientas
  * Uso de Copilot en Excel (con subscripcion a 365)
  * Presetaciones
    * Gamma (Y landings, redes sociales)
    * Mencion Pretzi
  * Videos Instucionales
    * Hey Gen

---

# IA Generativa Cretiva

## Generacion de Imagenes

* Casos de Uso
  * Generar imagenes a partir de texto
  * Generar imagenes a partir de imagen de referencia
  * Modificar una imagen existente
  * Imagenes con Texto
  * Diseño Grafico

* Modelos para generar imagenes
  * Propietarios
    * NannoBannana (Gemini)
    * GPT image 2 (recien salido del horno)
    * SeedDream
    * ...
  * Open Source
    * Flux
      * Lo podemos probar desde HF spaces

> [!NOTE]
> Los modelos propietarios tienen bastantes restricciones a la hora de generar imagenes para no permitir generar imagenes que pueden ridiculizar o herir la suceciptibilidad de un tercero

* Funcionamiento de los modelos de difusion (tecnico)
  * https://www.instagram.com/p/DRSGNZFgafh/
     
* Prompt Engineering para imagen
  * TIP:  Los prompts para imagenes si son en ingles suelen dar mejores resultados

### Generacion de Imagenes desde texto/imagen

* URL
  * https://leonardo.ai/
* Caracteristicas
  * 150 creditos por dia (casi gratis)
  * TE permite utilizar la mayoria de los modelos populares

---

#### Texto a imagen

```
A modern urban building under construction, captured in a highly realistic professional commercial photography style for an advertising campaign. The scene shows a multi-story concrete and steel structure in progress, with scaffolding, cranes, safety netting, construction workers wearing helmets and reflective vests, stacks of materials, and machinery on site. Clean composition with strong perspective, golden hour natural lighting, blue sky with subtle clouds, polished cinematic look, ultra-detailed textures on concrete, metal, glass, and dirt. Emphasis on progress, innovation, trust, and architectural ambition. Shot with a full-frame DSLR, 35mm lens, shallow depth of field, HDR quality, crisp focus, photorealistic, premium branding aesthetic, high resolution, no text, no logos.
```

* Resultado
  
<img width="2048" height="1136" alt="gpt-image-2_A_modern_urban_building_under_construction_captured_in_a_highly_realistic_profes-0" src="https://github.com/user-attachments/assets/ec0f2723-d64d-4152-bb91-155fff68e421" />

---

#### Imagen a Imagen

* Patiendo de esta imagen (pixelada y baja calidad)

<img width="168" height="300" alt="PixeadaConDerechos" src="https://github.com/user-attachments/assets/ceea8be8-9ab6-4aef-9c93-ecb768a4c28c" />

* Generamos esta imagen

<img width="1696" height="2528" alt="nano-banana-2_Quiero_la_imagen_en_calidad_cinematrografica_y_en_un_entorno_mas_natural_y_verde-0" src="https://github.com/user-attachments/assets/12763889-c27f-4108-9aac-426bce9dcfe8" />

---

#### Modificar imagen

* El mejor para modificar imagenes era Nanno Bannana (ahora el GPT image 2 de openai le hace competencia)
  * https://gemini.google.com/a
  * Se usa directamente desde la interfaz de Gemini

* Generamos esta imagen de un colega

<img width="1366" height="768" alt="Gemini_Generated_Image_1cbefu1cbefu1cbe" src="https://github.com/user-attachments/assets/36619ab1-3885-4d78-91c4-ff8e078711f8" />

> [!NOTE]
> Cuando generamos una imagen y no es exactamente lo que buscamos pero se acerca. Podemos utilizar Nanno Bannana para modificarla sin tener que volver a generarla desde cero

---

#### Imagenes con Texto

* URL
  * https://ideogram.ai/
* Caracteristicas
  * Modelo especializado en generacion de imagenes con texto
  * Se usa muchisimo en todo lo que s publicidad
  * La capa gratuita es menos generosa que LeondadoAI

 ```
A modern urban building under construction, captured in a highly realistic professional commercial photography style for an advertising campaign. The scene shows a multi-story concrete and steel structure in progress, with scaffolding, cranes, safety netting, construction workers wearing helmets and reflective vests, stacks of materials, and machinery on site. Clean composition with strong perspective, golden hour natural lighting, blue sky with subtle clouds, polished cinematic look, ultra-detailed textures on concrete, metal, glass, and dirt. Emphasis on progress, innovation, trust, and architectural ambition. Prominently integrated into the scene, large and elegant typography reads "Ayres de Madrid" with "Proyecto de Construccion" placed below it, both texts seamlessly blended into the environment (e.g., on a billboard, construction banner, or building facade), matching perspective, lighting, and shadows for a natural and realistic appearance. Shot with a full-frame DSLR, 35mm lens, shallow depth of field, HDR quality, crisp focus, photorealistic, premium branding aesthetic, high resolution, no logos other than the specified text.
```

* Imagen generada

<img width="1312" height="736" alt="image" src="https://github.com/user-attachments/assets/1e235c5d-22e3-4d47-96a0-35948682edb9" />

---

#### Diseño Grafico

##### Microsoft Designer

* URL
  * https://designer.microsoft.com/
* Caracteristicas
  * Buen Modelo de generacion de Imagenes
  * Caracteristicas para diseño como Canva

* Genere una invitacion
 * Descripcion : ¡Veni a conocer nuestro piso piloto en nuestra obra casi finalizada en el centro de madrid!
 * Imagen : Un edificio en proceso de construccion casi terminado

<img width="412" height="576" alt="image" src="https://github.com/user-attachments/assets/86f9b9a8-84da-4b8d-8b36-6848aa74fff7" />

##### Lovart

* URL
  * https://www.lovart.ai/
* Caracteristicas
  * Entorno de experimentacion para probar diseños
  * Poco creditos capa gratuita

```
Quiero todo el diseño de marca de una empresa de construccion (brochure, pagina web, tarjetar personales, etc) que sea todo consistentente
```

----
## Generacion de Videos

* Tambien existen numerosos modelos
 * Propietarios
   * Sora
   * Veo3
   * Seeddream
 * Open Source

* Casos de uso
  * Videos rapidamente : Qwen
  * Videos a partir de Imagenes
  * Videos a partir de Textos
  * Genracion de efectos 

* Proceso
  * Hacer un script con ChatGPT dividido en escena
  * Para cada escena generar un prompt para una imagen
  * Generar la imagen a partir de ese prompt
  * A partir de cada imagen generas un video de (5-10 segundos)
  * Generas la musica con otro programa de IA
  * Generas la voz con otro programa de IA
  * Compaginas todo con un programa editor de video tipo capcut
 
* Ejemplo de video que hicimos con alumnos
  * https://www.youtube.com/watch?v=vPwCdejOuio

### Videos rapidamente 

* Previamente lo podiamos hacer con Grok pero la parte de generacion de videos ahora es paga exclusivamente
* Podemos reemplazarlo por Qwen
   * https://chat.qwen.ai/

### Videos desde Imagenes/Texto

* URL
   * https://pollo.ai/invitation-landing?invite_code=dIOOD7
* Caracteristicas
   * Permite elegir el modelo
   * Si ingresan a la herramienta a diario se van acumulando creditos

* Creamos este video
  * https://pollo.ai/v/cmorjqiz408xjy3l9ly60rm1q?source=share

---

## Proxima clase... Generacion de Canciones

