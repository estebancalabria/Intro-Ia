# Clase Ocho - 30 de Abril de 2027

# Repaso

* IA Creativa
  * Generacion de Canciones
    * Udio
        * Bueno para generar fragmentos cada 5 segundos
          * https://www.youtube.com/watch?v=3sHdwQNJxDk&list=RD3sHdwQNJxDk&start_radio=1
    * Suno
        * Generar canciones enteras con estilo clasicos
    * Video institucional con HeyGen
        * Cancion de Udio/Suno de fondo
  * Generacion de Imagenes
    * Leonardo
    * Ideogram
        * Generar imagenes con texto

# Miscelaneas

* Entrevista de Moria a los Thereans
  * https://www.youtube.com/watch?v=Wh5Tif8LwYU

# Experiencia

* Criterio a la hora de usar la IA
* Validacion y grounding de lo que dice la IA
* Usar distintos modelos para tener visinones distitnas y un tercero que desempate

# Generacion de Imagenes

## Modificar una imagen

* Es dificil muchas veces dar en la tecla de la imagen exacta que quiero
* En lugar de volver a generar otra imagen distinta muchas veces es posible editar la imagen que ya tenemos con IA
* El modelo que mas destacaba en este aspecto
    * NannoBannana
* Pero ojo. OpenAI saco hace pocas semanas un modelo nuevo de imagenes que en edicion de imagenes parece que lo supera
    * GPT-image-2

<img width="1200" height="670" alt="image" src="https://github.com/user-attachments/assets/8d27bc73-ffa4-4a99-b7e5-329b97724d2a" />

```
Tengo esta imagen. Me podes generarla de nuevo tal cual esta pero la N arriba de Therean tiene un Ñ. Sacarle el apostrofe, Virgulilla, Circunflejo arriba de la Ñ para que sea una N. El resto de la iamgen esta perfecto
```

<img width="1024" height="571" alt="image" src="https://github.com/user-attachments/assets/71b7f426-0025-4d8c-9b1c-7cd4d993f252" />

> [!NOTE]
> Cuando quiero modificar una imagen de una persona es util incluir esto como parte del prompt
> "respetando los rangos y expresiones faciales"

# Generacion de Videos

* SeedDream
* Flux
* Sora
* Veo3
* Ejemplo de como la ia es correcta pero muchas veces pierde el criterio estrategico

* Casos de USO
  * Texto-a-Video
  * Imagen-A-Video
      * Este es el caso de uso deseable. Generar primero la imagen. Mayor control y el modelo trabaja mejor
  * Agregar efectos
  * Lip sync y sincronizacion de movimiento <<<
 
* La generacion de videos hoy se limita a videos de 5/10 segundos
* Para un video mas largo es neceseario compaginarcon una herramienta como Capcut


## Metodologia para la generacion de video

* Ejemplo de video
  * https://www.youtube.com/watch?v=Zxt-nqVWKZ4
* Como se hizo
  * Guion: Primero se escribe un script (con chatGPT) de framentos cortos de 5 segundos  
    * 70 fragmentos
    * Los dialogos
    * Al menos 3 horas te lleva
  * Para cada fragmento generas una imagen
    * Si son muchos fragmentos posiblemente tengas que pagar una herramienta y no te sirva solo las capas freemium (gratuitas)
  * Con cada imagen generas un video de 5 segundos
  * Si hay algo hablado un texto tranversal generas la voz
      * Generalmente para esto se usa eleven labs
      * O sino grabas las voces con microfono
  * Compaginas todo con CapCut (o el que te guste mas)


## Texto a video e Imagen a Video

* Existen muchas herramientas de generacion de video.
* Para no abrumarlos me gusta
    * Pollo.AI que tiene todos los modelos
          * https://pollo.ai/invitation-landing?invite_code=dIOOD7
      * PixVerse
          * https://share.pix.video/referral/JAEN6NA7
      * Buscar opciones en (https://theresanaiforthat.com/)
* Quiero hacer un video rapido a partir de una imagen
    * Grok (el mejor para videos rapidos pero Elon Musk se puso la goora y ahora te lo cobra)
        * Censura muy baja
        * Aspectos eticos a considerar

* PolloAI    
  * Generamos este video : https://pollo.ai/v/cmolmd1su00wqu95mcbzz933d?source=share
  * Puntaje : 10/10
    * Qwen : El reemplazo de Grok cuando se puso la gorra
* Pixverse
  * Puntaje : 10 / 10

## Generacion de Efectos

 * No esta en una sola herramienta
     * Las que vimos antes lo tienen
* La primera donde lo vi
      * https://pika.art/


## PRoxima Clase

* Mostrar Central de IAS
