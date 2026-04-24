# Clase dos - 24 de Abril 2026

# Repaso

* Large Laguage Models
  * Elegir el modelo adecuado segun la tarea
  * Propietarios
    * ChatGPT
      * Memoria
      * Emula conversaciones humanas
      * Personalizar la forma que queremos que responda (se educa)
    * Gemini
      * Mencionamos nada mas
    * Copilot
      * Mencionamos nada mas
* Propmpt Engineering
  * Como dar buenos prompts

# Large Language Models

## Modelos Propietarios

### ChatGPT

* OJO. ChatGPT en el celular tiene un modo voz...

  <img width="134" height="132" alt="image" src="https://github.com/user-attachments/assets/1c7d2742-3255-4669-b113-43edadb793de" / >
  
* Ese modo voz esta optimizado para que parezca que habla una persona, pero la calidad de respuesta es MALISIMA


---

### Gemini

* URl
    * https://gemini.google.com/app
* Empresa
    * Google
* Para que destaca
    * Gemini traza la IA con busquedas especialozandose en conomimiento Factico (en hechos)
    * Mejor integracion con busquedas en internet
    * Integracion con el ecosistema de google
    * Creador del modo investigacion: chequea dependiendo el tena en +100 paginas y te hace un informe (3 por mes gratis)
    * Excelente para editar y crear imagenes con Nanno Bannana

#### Integracion con el ecosistema de google

1. Integracion con Google Calendar

```
Generame un evento de una hora h oy a las 17:00 que sea hacerme millonario
```

```
Generame todos los martes y jueves a las 17 horas ir a pilate menos los dias feriadso
```

2. Integracion con Google Flights y Google hotels

```
Quiero viajar a la polinesia la semana que viene. Quiero que me busques opciones de vuelo por google flihgts y opciones de alojamiento por google hotels. Me voy a quedar una semana
```

#### Modo Investigacion (Lo mejor que tiene)

* Dado un tema te hace una investigacion profunda en internet con integrado como la de busqueda de goog
* Elegir dentro de las herramientas el Deep Research

```
Quiero una investigacion sobre los viaje a la Luna
```

* Este prompt me genero esta investigacion
  * https://gemini.google.com/share/9bee314be50c
* Se puede exportar a google docs directamente
---

### ChatGPT y Gemini

* Ambos incorporan el concepto de Canvas.
* Un canvas esta inspirado en los artefactos de Claude
* Te permite generar un espacio de trabajo sobre un documento que es editable
* En vez de generar todo el contenido nuevamente con las correcciones vas cambiando el mismo documento
   * Problema : Le pedis que cambie algo, te lo cambia y ademas te cambia otra cosa que no le pediste
   * Solucion : Usar un canvas para poder cambiar solamente algo especifico sin tocar el resto
* Al regenerar un documento entero una y otra vez se gasta muchos tokens y rapidamente llegamos al limite de uso de la capa gratuita
   * En cambio, usando canvas como solo cambia una seccion gastamos menos tokens y nos dura mas
* Puedo seleccioar un parrafo, boton derecho y hay un menu desplegable que dice "Preguntar a ChatGPT"

```
Quiero mandarle un mail a mi jefe para pedirle un aumento. Dame una version inicial y geneame un canvas para trabajar sobre el. 
```
* Me genera un canvas....

---

### Claude

* URL
  * https://claude.ai/
* Empresa
  * Anthorpic
* En que destaca
  * Tiene un enfoque muy fuerte hacia la Etica y la privacidad
  * Tiene un enfoque mas tecnico
    * Especial para tareas tecnicas, de programacion, de ingenieria, etc...
    * Respuestas mas profesionales
  * Invento el concepto de artefacto para previsualizar la respuesta (copiado como Canvas en otros modelos)
* Contras
  * Mas desde lo de trump esta saturado
  * Te deja hacer mucho menos que ChatGPT

#### Precision en tareas Tecnicas

```
Tengo que hacer un edificio en Madrid y quiero evaluar que materiales me conviene utilizar y quiero informacion tecnica relevante de dichos materiales como durabilidad, resitetencia y todos los datos tecnicos que un ingeniero indutrial maneja en el tema. Podes habilitar la busqeuda en itnernet.
```

* Respuestas
  * ChatGPT
    * https://chatgpt.com/share/69ea4d1b-310c-83e9-a1d2-94bbab7bdb7c
  * Claude
    * https://claude.ai/share/5897ffff-1db6-4894-a831-81008f445e83
* La de Claude es mucho más específico y técnico en su respuesta

#### Previsualizacion con artefactos

* Para Claude la palabra "artefacto" tiene un significado especial.
  * Es una palbra reservada o magica
  * Hace referencia a un espacio de previsualizacion
* Ademas Claude es ideal para programar, topisimo
* Orientado tambien al analisis de datos

```
Programame un unico artefacto con el juego PONG. El jugador de la izquierda se mueve con la a y la z. El de la derecha con las teclas de cursor. La barra espacidoa se usa para iniciar y pausar el juego. Una vez pausado el juego se puede reiniciar.  Quiero que tenga unos graficos modernos, con efectos de particulas, y que sea super profesional. Sorprendeme.
```

> [!NOTA]
> Miren lo que hizo Martin! Felicitaciones!
> https://achikigod.github.io/tenis-de-mesa/


# Actualidad

## Seguridad y privacidad

* Tema de Segudidad entre Claude y Trump
  * https://en.wikipedia.org/wiki/Anthropic%E2%80%93United_States_Department_of_Defense_dispute
* Esta noticia tiene que hacernos pensar en tema de uso de la IA y privacidad de los datos

# Modulo 3 : Herramientas de Productividad

## Text-to-Speech (Texto-a-voz)

### LLM

* Notar que ChatGPT y los llm suelen tener una opcion para leer la respuesta

<img width="606" height="389" alt="image" src="https://github.com/user-attachments/assets/00284c91-3833-4245-b0c2-b15bd72b180f" />

### Herramientas

#### Natural Readers

* Herramienta para leer un texto
  * https://www.naturalreaders.com/
* Idea
  * Está bueno para practicar pronunciación al estudiar algún idioma
  * Ideal para escuchar mientras manejo

> [!NOTE]
> Puntaje : 9 / 10

#### Eleven Labs

* Otras de este tipo:
  * https://elevenlabs.io/
      * Era una herramienta exclusivamente paga y ahora tiene capa gratuita
      * Para clonar voces
        

# Para la proxima clase

* Vamos a seguir viendo LLM Propietarios... y tambien Open Source
* De Claude (y en general de todos) me falto mencioar el concepto de la multimodalidad
  
