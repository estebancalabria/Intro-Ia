# Clase Dos - 23 de Abril del 2026

# Repaso

* Roadmap del Curso
* LLM
  * Propietarios
    * ChatGPT
        * Emular Conversacion
        * Personalizacion
    * Gemini
        * Modo Investigacion ( 3 gratis por mes)
        * Integracion con Google
    * Copilot
        * Integracion con Microsoft
* Herramienta
    * NaturalReaders
      * TODO: Buscar alternativa

# Large Language Models

## Propietarios

* Distitintos modelos de OpenAi y comparacion
  * https://www.instagram.com/p/DKhQrTvuFcw/?img_index=1
  * De paso lo conocen a Sam Altman el creador de ChatGPT

### Caracteristicas comunes

* Multimodalidad
* Artefactos / Canvas (Gemini/ChatGPT)
* Llamadas a herramientas
   * Busqueda Web


### Ideas Generales de Trabajo

* Conociendo la ventaja de cada herramientas es posible
  * Configurar un flujo de trabajo donde utilizamos varias en simultanea
  * Ejemplo
     * Perplexity para la investigacion academica
     * ChatGPT para ir redactando y modificando el irforme con Cancas
     * Claude (y/o Gemini) para una verificacion factural de lo que vamos generando

---

### Canvas en ChatGPT o Gemini

* En claude vimos los artefactos para la previsualizacion
* CharGPT y Gemini tienen algo similar que se llama Canvas
* Te permite previsualizar un documento y editarlo parcialmente (sin tener que vovler a generar todo de nuevo)
* Canvas es como una palabra reservada (palabra magico o especial) que ChatGPT entiende

```
Quiero que  me redactes un correo para pedir un aumento a mi jefe. Generarme un canvas con la primer version.
```

* Me genera una primera version que puedo "editar"
* Al editar me divide la pantalla en dos
* La edicion no necesita generar todo el documento de nuevo
   * Ahorramos tokens
 * Solo se modifica lo que le pedimos concretamente
 * A veces pasa que al generar todo de vuelta cambia cosas que no queriamos

> [!NOTE]
> Ahorro de tokens en canvas : https://chatgpt.com/share/69ea58b9-b67c-83e9-bf3e-456966226a54

---

### Claude

* URL
   * https://claude.ai/
* Empresa
   * Anthropic
* Para que destaca
   * Cuestiones tecnicas desarrollo / ingenieria
   * Intrujo el concepto de artefacto (que otros modelos se conoce como Canvas)
      * Artefacto = previsualizacion
   * Fuerte enfoque en cuanto a lo Etico
   * Fue el primero en introducir el concepto de miltimodalidd (permite adjuntar archivos)
* Contra
   * En la version gratuita llego muy rapido al limite

* Noticias relacionadas
  * https://en.wikipedia.org/wiki/Anthropic%E2%80%93United_States_Department_of_Defense_dispute
 
* PAra probar su capacidad tecnica en desarrollo utilice el siguiente prompt

```
Quiero que desarrolles el juego pong en un unico artefacto en javascript y html donde se empiece a jugar y se pause el juego con la barra espaciadora. Puedo reiniciar el juego al pausar. El jugador de la derecha se mueve con las teclas de cursor y el de la izquierda con la a y la z. Quiero que sea un disenio moderno, con efectos de graficos que impacten, super profesional.
```

* A partir de ese prompt me genero

> https://claude.ai/share/e2178f1d-c6d7-4f14-8eed-92e65a95d281

#### Prueba Tecnica

* Prompt
```
Tengo que hacer un edificio en Madrid y quiero evaluar que materiales me conviene utilizar y quiero informacion tecnica relevante de dichos materiales como durabilidad, resitetencia y todos los datos tecnicos que un ingeniero indutrial maneja en el tema. Podes habilitar la busqeuda en itnernet.
```
* Respuestas
  * ChatGPT
    * https://chatgpt.com/share/69ea4d1b-310c-83e9-a1d2-94bbab7bdb7c
  * Claude
    * https://claude.ai/share/5897ffff-1db6-4894-a831-81008f445e83

* Veredicto de los especialistas (No el profe)
   * Segun los expertos de este curso : Parece más concreto y técnico la opción de CLAUDE


#### Prueba Multimodalidad : Landing a partir de CV

* Voy a adjuntar mi CV (pdf) y pedir que me genere una Landing
* Al poder trabajar con Archivos, imagenes, ademas de texto estoy diciendo que el modelo es "multimoadal"

```
A partir de Mi CV adjunto. Me podes generar una landing profesional en un unico artefacto  para darme a conocer y promocion.
```

* Me Genero
  * A partir de Mi CV adjunto. Me podes generar una landing profesional en un unico artefacto  para darme a conocer y promocion.

---

### Perplexity

* Url
  * https://www.perplexity.ai/
* 
* Es un modelo especial que se usa prinpalmente para "Ivestigacion"
* Se encarga de mantener las fuentes de lo que hablamos para mejorar el grounding
* Podes dicrimnar las fuentes que queres que use (fuentes academicas)
  * Ideal para trabajos para la facultad

```
Quiero hacer una investigacion sobre las ultimas novedades en materiales para la construccion 
```
* ( El anterior lo hice citando solmente fuentes academicas)

* Me genero la siguiente investigacion con fuentes academicas

> https://www.perplexity.ai/search/quiero-hacer-una-investigacion-FaFvkheCT9.H_F9R2HGFqA#2

---

### Grok 

* Url
  * https://grok.com/
* Empresa
  * X (Elon Musk)
* Caracteristicas destabales
  * Muy buen grounding : Buqueda web por defecto, antes de contestar busca informacion en X y en itnernet
  * Muy buena integracion con la plataforma de X
  * Menor censura que otros modelos
  * ERA el mejor para generar videos rapidamente (pero ahora es pago)
* Desventaja
  * Utimamente ajusto mucho sus planes y cosas que eran gratis ahora solo en la version paga
  * En los picos de demada no lo podes usar
  * Muchas veces tiene un tono mas irrevente menos profesional ajustado a la ubicacion del usuario
  * Muchos temas legales por la baja censura
 

#### Menor censura

```
Haceme un chiste que le resulte gracioso a alguien de Madrid que tenga dobles sentidos, malas palabras y sea de mal gusto
```
* Probar distitos modelos
   * Gemini : Puede que no te deje
   * Grok : Te hace el chiste
 
* Videos controversiales
   * https://grok.com/imagine/post/b68b595d-12a2-4bae-a74b-0e5ad28818d2?source=post-page&platform=web
   * Mo pude generar un video asi con otro modelo


---

## Open Source

* Los modelos anteriores son modelos Propietarios
  * Pertenecen a una empresa que los administra
  * La empresa (como vimos con grok) restringe su uso a voluntad y ajusta limites de uso
  * No tenemos plena seguridad que pasa con los dats que le damos (las convesaciones de chat)
       * Aspectos importantes de Privacidad
  * El acceso a los modelos y la informacion no esta democratizada
* Los modelos Open Source
   * Son modelos que una organizacioacion entrena y pone a disposicion del publico general
   * Los podemos modificar libremente
   * Los podemos descargar y utilizar localmente (con una buena computadora)
* Los modelos propietarios suelen ser mas eficientes porque las empresas estan compitiendo todo el tiempo por mejores funcionalidades pero los modelos Open Source los podemos descargar, modificar y utilizar en entornos donde la privecidad y sensibilidad de los datos es critica
* Porque son importanes los modelos Open Source?

### Catalogo

* Americanos
  * Familia Llama
      * Por Meta (ex Facebook)
  * Gemma
      * Google
* Chinos
   * DeepSeek
      * https://chat.deepseek.com/
   * Qwen
      * De la empresa Alibaba
      * https://chat.qwen.ai/
   * Kimi
      * https://www.kimi.com/
* Euroepos
   * Frances
     * Mistral
        * https://chat.mistral.ai/chat

### Ejecutar un modelo localmente

* LMStudio
  * Aplicacion de escritorio muy facil
  * https://lmstudio.ai/
* Ollama
   * https://ollama.com/

# Glosario

* Gronding : Vincular la respuesta de la IA con fuentes verificables
