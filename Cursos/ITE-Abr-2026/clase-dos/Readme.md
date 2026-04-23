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

### Caracteristicas comunes

* Multimodalidad
* Artefactos / Canvas (Gemini/ChatGPT)
* Llamadas a herramientas
   * Busqueda Web

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


### Prueba Tecnica

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


### Prueba Multimodalidad : Landing a partir de CV

* Voy a adjuntar mi CV (pdf) y pedir que me genere una Landing
* Al poder trabajar con Archivos, imagenes, ademas de texto estoy diciendo que el modelo es "multimoadal"

```
A partir de Mi CV adjunto. Me podes generar una landing profesional en un unico artefacto  para darme a conocer y promocion.
```

* Me Genero
  * A partir de Mi CV adjunto. Me podes generar una landing profesional en un unico artefacto  para darme a conocer y promocion.




## Open Source

# Glosario

* Gronding : Vincular la respuesta de la IA con fuentes verificables
