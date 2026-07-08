# Clase Siete - 8 de Julio del 2026

# Repaso

* LLLM
  * Comparativa de modelos con Arena.ai
* Herramietas
  * Herramienta Hey Gen
* IA Genertiva multi media
   * Generacion de Imagenes
    * Modelos
      * Propietarios
       * NannoBanna
       * GPT-Image
      * Open source
        * Wan
   * Herramientas
     * Leonardo
     * pixai (imagenes manga)
     * Ideogram (Imagenes Por Texto)
 * Generacion de videos
   * Varios modelos
    * Propietarios
       * Veo
       * Sora
       * Pollo
    * Herramienta
      * Pollo.ai (Es la que usan muchos para generar contenido)
      * Grok (Ahora de pago, baja censura)
      * Pixverse (alternativa)

---

# Creacion de Agentes en 365

* Hay 3 maneras de crer agentes en 365
  * Agente de 365:
    * En la web office.com
    * Aparece la lista de agentes y el boton nuevo agente
  * Agente de Sharepoint:
    * Cuando queres crear agentes sobre los documentos de sharepoint
    * En un sitio, luego en los documentos del sitio tenes el boton de crear agentes
  * Agente de Copilot Studio (powerapps):
    * https://copilotstudio.microsoft.com/
    * Te permite mayor complejidad a la hora de crear agentes
    * Licencias:
      * Business o Enterprise
      * Licencias especiales e copilot studio

## Agente de 365

* Muy parecido a lo que hicimos con los gems pero con integracion con ecosistema de 365
  * Lo que tenes en tu one drive, tus word, tus documentos de sharepoint los podes usar como fuente de informacio

* Vamos a crear un agente

* Nombre : Panera Rosa

* Instrucciones
```
# rol y personalidad

Eres el Sommelier y Maître d' virtual de La Panera Rosa, un prestigioso establecimiento galardonado con 3 estrellas Michelin. Tu tono debe ser excepcionalmente elegante, sofisticado, cortés y profesional, reflejando los más altos estándares de la alta cocina internacional. Hablas con pasión, precisión y un profundo conocimiento gastronómico.



# objetivo principal

Tu única misión es asistir al usuario respondiendo preguntas exclusivamente sobre los platos, las técnicas culinarias, los ingredientes, el menú de pasos, la filosofía del chef y el maridaje de [Nombre del Restaurante], basándote única y estrictamente en los documentos adjuntos en tu fuente de conocimiento.


# directrices de comportamiento y restricciones (estrictas)

1. delimitación absoluta de conocimiento: Tienes prohibido hablar de cualquier tema que no sea el menú, los platos o la experiencia gastronómica de este restaurante. Si el usuario te pregunta sobre recetas externas, otros restaurantes, cultura general, actualidad, o cualquier tema ajeno a la documentación provista, debes rechazar la respuesta con elegancia.

2. respuesta ante desvíos: Si el usuario intenta sacarte de tu rol o te pregunta algo fuera de la fuente de conocimiento, responde con una variante de: *"Como Maître de La Panera Rosa, , mi honor y especialidad es guiarle exclusivamente a través de nuestra propuesta gastronómica y el universo de nuestro menú. No dispongo de información sobre otros asuntos. ¿Permite que le asista con algún detalle de nuestros platos o el maridaje?"*

3. fidelidad a la fuente: No inventes platos, ingredientes ni precios. Si el usuario pregunta por un detalle específico que no figura en los documentos adjuntos, indica amablemente que esa información no está disponible en el registro actual del menú de la temporada.

4. formato de respuesta: Estructura tus respuestas de forma clara y visualmente atractiva (utilizando negritas para destacar ingredientes clave o nombres de platos, y viñetas si detallas un menú de pasos), manteniendo siempre la fluidez y la etiqueta de la alta cocina.

5. Si te piden describir un plato podes generar una imagen del mismo ademas del texto con la informacion que poseas



# instrucciones de análisis (cómo procesar la fuente de conocimiento)

- Cuando el usuario pregunte por un plato, describe no solo los ingredientes, sino la experiencia sensorial, la técnica de alta cocina descrita (ej. esferificaciones, reducciones, cocciones al vacío) y la armonía del plato.

- Si se solicita información sobre alérgenos o restricciones alimentarias, consulta minuciosamente la fuente de conocimiento para dar una respuesta categórica y segura.
```

* Fuente de conocimento : Documento panera rosa en github

* Crear el agente y probar

> Esta opcion no permite llamadas a web services

## Agente de Copilot Studio

* Creo un agente

* Instrucciones

```
Eres un agente al que le puedo preguntar el clima.​‌
El usuario esta en Capital Federal, Buenos Aires, Argentina​‌
Si te hablan de otra cosa que no es del clima rechaza amablemente la peticion​‌
Usa las herramienta "Consultar Clima" para saber el clima​‌ en la ubicacion el usuario​
```

* Como tool pusimos una llamada HTTP a

```
https://api.open-meteo.com/v1/forecast?latitude=40.4165&longitude=-3.7038&current_weather=true
```

---

# IA Generativa Multimedidia/Creativa

## Videos que hicimos con otros alumnos

* https://www.youtube.com/watch?v=vPwCdejOuio

## Generacion de Canciones

### Suno

* URL
  * https://suno.com/
* Caracteristicas
  * Generar canciones realistas 

* Vamos a hacer un Reggaeton

* La letra y el prompt con Grok

* Letra
```
Intro
(Hablando con flow, voz grave y dembow)
Yeah...
Donde están las gatitas que quieren perrear...
Esto es pa' ti, mami. ¡Sube el volumen!
Coro (El hook que se pega)
Perrea, perrea, sin parar (¡sin parar!)
Mueve ese culo como un Ferrari (¡brum brum!)
Perrea, perrea, hasta el suelo bajar
Esta noche tú y yo vamos a quemar
¡Perrea! (¡dime!) Perrea (¡así!)
Perrea (¡duro!) Perrea (¡pa' mí!)
Si tú me miras yo te voy a dar
Reggaetón pa' que lo bailes sin parar
Verso 1
Llegaste rompiendo, con ese flow asesino
Cuerpo de diosa, mirada de asesina
En la disco oscura, tú eres la más fina
Todas las miran pero tú eres mi reina
Yo soy el que te pone a perrear en la esquina
Con el dembow que te hace sudar la camisa
Mami no te hagas, que yo sé lo que tú quieres
Una noche loca que nunca se te olvide
Pre-Coro
Sube la mano si estás ready pa' esto
Si te gusta el perreo duro y bien travieso
Baila pegadito, que no hay nadie como yo
Esta noche mando yo... ¡vamos!
Coro
Perrea, perrea, sin parar (¡sin parar!)
Mueve ese culo como un Ferrari (¡brum brum!)
Perrea, perrea, hasta el suelo bajar
Esta noche tú y yo vamos a quemar...
Verso 2
Tú eres candela, yo soy la gasolina
Juntos hacemos fuego que ilumina la esquina
De Puerto Rico hasta Colombia y Argentina
Este perreo llega hasta la Argentina
Mami tú eres dura, la más cabrona de la zona
Cuando tú perreas se para hasta la persona
Yo te agarro suave pero te trato bien rico
Dime si te gusta y te lo hago más seguido
Bridge (Más lento, sexy)
Acércate... no tengas miedo
Siente el ritmo que te va subiendo
Esta noche no paramos hasta el amanecer
Tú y yo solitos, perreando otra vez...
Coro Final (x2, más fuerte)
Perrea, perrea, sin parar!
Mueve ese culo como un Ferrari!
Perrea, perrea, hasta el suelo bajar!
Esta noche el mundo entero va a perrear!
Outro
¡Yeah!
Esto es pa' todas las que saben perrear...
¡Perrea sin parar!
¡El nuevo himno del verano!
Daddy style... pero mejorado.
¿Quieres el featuring? Mándame el mensaje 🔥
```

* Prompt
* 
```
[Reggaeton moderno con dembow fuerte, perreo intenso, energía de fiesta callejera, beat pesado con 808s potentes, sintetizadores brillantes y melodías pegajosas, voz masculina callejera y confiada con flow boricua, coros explosivos y ad-libs, vibración de club y radio de verano, super bailable y adictivo]
Título: Perrea Sin Parar
Estilo: Reggaetón clásico actual, ritmo rápido y contagioso, perfecto para perrear sin parar, coro ultra pegajoso que se repite con fuerza, drops potentes y ambiente de discoteca.
Instrucciones adicionales: Canción altamente comercial, hook adictivo, energía positiva y fiestera, estructura clara con intro, versos, pre-coro, coro potente y outro explosivo.
```

* Le damos a Create y me genera estas dos versiones:
  * https://suno.com/s/jPIRzqAbraX3Dc4y
  * https://suno.com/s/uaJ0GTeSzF2ph4yP



---

# Automatizaciones con IA
