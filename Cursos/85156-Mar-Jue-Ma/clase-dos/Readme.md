# Clase Dos - 31 de Marzo del 2026

# Repaso

* Large Language Models
  * Propietiarias
    * ChatGPT
        * Emular la conversacion humana
        * Personalizacion (Recordar Preferencias_
        * Memoria
    * Gemini
        * Imagenes con Nano-Banana
        * Modo investigacion
            * Investiga en muchisimos sitios a la vez y te hace un informe
        * Integracion con el ecosistema de Google
        * Se centra mas en conocimiento factico (facts) que en la conversacion humana
            * Eventualmente la IA replazara al buscador
* Agente
    * Mencionamos el concepto

# IMPORTANTE: Requerimiento para aprobar el curso

> https://www.instagram.com/mct.esteban.calabria/ 

# Large Language Models

## Modelos Propietarios

### Claude 

* https://claude.ai/
* Es mas un profesional tecnico que amigable
    * Mas orientados a tareas tecnicas
        * Programacion
        * Analisis de datos
        * Analisis
  * Tiene una version de escritorio que configurandola puede acceder a tus tus archivos
        * https://claude.com/download
  * Claude tiene una funcionalidad PArticular
        * Artefactos
            * Sepeta el entregable de toda la respuesta y razonamiento del modelo
  * Fue el primero en ser MultiModal
  * Cotra : Pocos tokens en su capa gratuita y ultimamente un poco sobrecargado debido a un pico de demanda en su uso
  * Hagamos un ejemplo

```
Quiero que desarrolles conmigo el juego pong en un unico artefacto en  html y javascript. Que el jugador de la derecia se mueva con las teclas de cursor y el de la izquierda con la a y la z. Quiero una pantalla de bienvenida donde se empieza el juego con la barra espaciadora y que en cualquier momento se pueda pausar el juego tambien con la barra. Quiero que el juego tenga efectos de particulas y efectos de sonido que sea moderno y este a la altura de un juego del 2026.
```

* Lo hice con el modelo Haiku porque el Sonnet se trababa (es algo que ocurrio ultimamente, antes no era asi)

> https://claude.ai/share/d3a19a1c-fb53-4774-a14c-bff9ee35b639

### Grok 

* El modelo de Elon Musk
* El mas irreverente de todos
  * El modelo de lenguaje de los propietarios el que tiene mejor grado de censura
      * Le podes pedir que te cuente un chiste subido de tono
      * Menos politicamente correcto
* Muy buen generador de imagenes y videos sencillos (Modulo 4)
  * Parece que ahora no deja porque es pago

### Perplexity 

* https://www.perplexity.ai/
* Es ideal para citas y fuentes
* El entenamiento de modelo es especial porque mantiene las fuentes de donde saca la informacion
* Ideal para trabajos de investigacion, universidad, secundario
* Ejemplo

```
Quisiera una investigacion con fuentes academicas sobre la "Dama blanca"
```

* Voy a habilitar solo fuentes academicas

> https://www.perplexity.ai/search/hazme-un-informe-sobre-la-dama-PgLz6GrLQTC1ICf8uZJ6gg

## Modelos Open Source

### Aspectos Eticos y de Seguridad

* Ya es sabido que el Departamento de Defensa de USA puede consultar las conversaciones de ChatGPT.
* La privacidad SI IMPORTA cuando hablamos de IA
* Ver : https://www.instagram.com/p/DOqu-k8Dvfb/?img_index=1
* Existen herramientas para anonimzar documentos que contienen datos de terceros : https://www.k2view.com/blog/data-anonymization-tools/

### Que son los modelos Open Source

* Son modelos que alguien entreno y puso el modelo disponible para la comunidad
* Son modelos que se pueden modificar "libremente"
* Son modelos que se puedem descargar y utilizar en mi computadora maneniendo el control de mis datos
    * Ejecutar un LLM localmente suele requerir de un buen hardwaee y en particular de una buena placa de video (NVidia mejor)

### Donde se suben los modelos Open Source?

* Los modelos Open Source se suben a hugging Face
    * https://huggingface.co/
    * Es como un github pero de modelos Open Source (no solo LLM sino modelos de todo tipo_
    * **CTA: Se animan a crearse una cuenta en hugging face (para ahora o para clase que viene)
    * Sin ser tecnico tengo la posibilida de probar modelos en la seccion de Spaces (una vez que me cree la cuenta)
        * https://huggingface.co/spaces
        * Por ejemplo puedo probar el modelo Flux para generar imagen
            * https://huggingface.co/spaces/black-forest-labs/FLUX.1-dev
        * Con la imagen generada puedo usar el modelo WAN para crear un video
            * https://huggingface.co/spaces/r3gm/wan2-2-fp8da-aoti-preview

<img width="1024" height="1024" alt="image" src="https://github.com/user-attachments/assets/f379b4b5-f2d5-46ae-80a4-679a067488f2" />

### Moodelos Open Source

#### Americanos

* Familia Llama
  * Son modelos entrenados por Meta (Mark Zuckemberg)
  * El de Wsap
      * Tenes un contacto que se llama Meta
      * Podes citarlo y preguntarle cosass en tus conversaciones con el @Meta
          * El arbitro entre discusioen de amigos en Wsap!
  * Porque Open Source >>>>> https://www.youtube.com/shorts/wrdmUhx6f8o

#### Chinos

>>>> **PROXIMAMENTE**

---

# Herramienta (Modulo 3)

## Text to Speech (Texto a Voz)

### NaturalReaders

> https://www.naturalreaders.com/

* Les hace un OnBoarding....
* Es una muy buena opcion para soluciones rapida
* La capa gratuita es muy generosa.
* Puntuacion : 8/10
  * Las voces son mejorables pero para ser una herramietna con un margen gratuito amplio viene bastante bien 

### ElevenLabs

* https://elevenlabs.io/

* Es la que usan los youtubers y profesionales
* Muchas opciones para controlar el tono, el acento, la intencion
* El mas completa de todas hoy en dia en el mercado
* Cristian la estuvo probando y le gusto mucho, se asombra. 10/10

## Speech to Text (Voz a Texto)

* Mas adelante vamos a ver herramientas especificas (para transcribir reuniones) pero te adelanto que cualqueir llm puede utilizar su capacidad  multimodal para transcribir textos

# Comparativa

* Gracias Sofia

# Resumen rápido de elección según uso:

| Uso principal | Mejor modelo |
|---|---|
| Coding / Programación | Claude |
| Información actual / Noticias | Grok |
| Multimodal (imágenes/video) | Gemini |
| Uso general / Productividad | GPT-5 |
| Precio bajo + rendimiento | Grok o DeepSeek/Qwen |
| Proyectos largos / Análisis | Claude o Gemini |
| Privacidad / Local | Llama 4 |

# Glosario

* Multimodal : Modelos que entienden imagenes y archivos ademas de texto
* LA IA es no deterministica : Ante el mismo prompt no da siempre el mismo resultado

# Para la proxima clase....

* Vamos a terminar de ver otros Modelos Open source
* Vamos a expicar como utilizar un modelo Open Source Localmente
* Vamos a explicar como saber en un momento dado cual es el mejor LLM para una tarea dada (ya que esto cambia con el tiempo muy velozmente)
* Prompt Engineering
