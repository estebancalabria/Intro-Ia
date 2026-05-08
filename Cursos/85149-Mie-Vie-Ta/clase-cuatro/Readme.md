# Clase Cuatro - 8 de Mayo del 2026

# Repaso

* Large Language Models
  * Propietarios
    * Grok
    * Perplexity
      * Integracion con herramientas
      * En cotextos academico y de investigacion por seleccion de fuentes
  * Open Source
    * Qwen
    * Mistral
    * DeepSeek
      * Introdujeron el modo pensado
* Herramienta
  * Napkin

# Herramientas

* Herrmienta que incoporta IA en Excel y Sheets (Gracias Roberto)
  * https://numerous.ai/

# Large Language Models

## Open Source

* Se pueden ejecutar localmente y los datos de las conversaciones no quedan almacenados en el servidor de una empresa
  * Esto muy importante para organizacione que manejan datos sensibles
  * https://www.instagram.com/p/DOqu-k8Dvfb/?img_index=1

### Repositorio de Modelos Open Source

* Peeden ir entrando y creandose una cuenta
    * https://huggingface.co/
* En esta pagina van a encontrar
  * Modelo Open Source de Gneracion de texto y todo tipo (Imagenes)
   * Ejecutar un modelo de IA tiene sus vercuetos
  * Datasets : Conjuto de datos que se usaron para entrenar los modelos
  * Spaces
    * Espacios de trabajo limitados por dia donde podes probar algunos modelos sin tener que descargarlos

### Ejecucion de Modelo Open Soure Localmente

* Herramientas para ejecutar un LLM local
  * https://ollama.com/
     * Mas complejo y se utiliza por linea de comando
  * https://lmstudio.ai/
     * Aplicacion de escritorio facil de usar
* Ambas descargan los modelos de HF

## Evaluacion de Modelos de IA

* Comparar modelos de IA
 * https://arena.ai/

* Hoy : Competencia de chistes

```
Contame un chiste
```

* En el Leatherboard

---

# Prompt Engineering

* Teoria
   * https://www.instagram.com/p/C5MDsQiR5cG/?img_index=1
* Componententes de un buen prompt
  * Tarea
  * Contexto
  * Ejemplo
  * Rol
  * Formato
  * Tono

# Contexto

* Prompt
* Conversacion
* System Prompt
  * Intrucciones del fabricante que definen como se debe comportar el modelo
  * Instrucciones Personalizadas
     * Actuabamos sobre el system prompt
* Herramientas
  * Busqueda Web
* Conversaciones pasadas
* Memoria

## Tips 

### Tip de contexto com el modo dictado

* Usar el modo dictado para dar mas conexto en nuestros prompts

* No es lo mismo poner

```
Escribime un mail para decir que no voy a ir atrabaja hoy
```

* Me Genero

```
Asunto: Ausencia hoy

Hola [Nombre],

Quería avisarte que hoy no voy a poder asistir al trabajo por un tema personal. Voy a estar atento al mail y a cualquier cosa urgente que necesiten.

Disculpá las molestias.

Saludos,
Esteban
```

* Que usando el modo dictado decir

```
Hola, me gustaría escribir un mail diciendo que no voy a ir a trabajar, dando una excusa muy verosímil. Te dejo en tus manos que invente la excusa y aplicando a la emotividad, ¿no?, sabiendo que mi jefe es hincha de Racing y que es una persona que no se toma muy bien los faltazos. Entonces me gustaría tratar este tema con mucho, mucho tacto, encontrarle la vuelta para que no se enoje, tratar de justificarlo muy bien. Mi jefe responde mucho mejor a los mails que son muy emotivos y muy persuasivos, así que espero que me hagas un mail que cumpla esas características.
```

* Me genero

```
Hola [Nombre],

Quería avisarte con tiempo que hoy no voy a poder asistir.

La verdad me costó bastante tomar la decisión porque sé que no es un buen momento para faltar y no me gusta dejar colgado al equipo, pero desde anoche estoy con un cuadro bastante fuerte de malestar y casi no pude descansar. Intenté levantarme para ir igual, pero sinceramente no estoy en condiciones de rendir bien ni de estar al 100%.

Te pido disculpas porque sé que estas cosas generan complicaciones y justamente por eso preferí avisarte de entrada y ser honesto antes que ir en malas condiciones y terminar empeorando durante el día.

Voy a intentar descansar y recomponerme un poco, porque siento que el cuerpo a veces nos obliga a frenar cuando el alma ya viene agotada hace rato. Mañana espero poder volver, no solo físicamente, sino también con la cabeza y el corazón en su lugar, para retomar todo lo pendiente con la energía y el compromiso que el trabajo y el equipo merecen.

Gracias por entender.

Abrazo,
[Tu nombre]
```

### Tip : Usar a la ia como experto en prompt engineeing

* Se me ocurre este prompt

```
Quiero redactar un informe sobre analisis de inversiones inmobiiliarias en capital federal para ver que me conviene, en donde invertir, que barrios, que me conviene hacer en cada barrio, etc.
```

* Le digo a la IA que me lo mejore

```
Actua como un experto en prompt engineering y quiero que me vuelvas a redactar este prompt de manera profesional "Quiero redactar un informe sobre analisis de inversiones inmobiiliarias en capital federal para ver que me conviene, en donde invertir, que barrios, que me conviene hacer en cada barrio, etc." Dame directamente el contenido para compiar y pegar sin acotar nada mas.
``

> [!NOTE]
> OTRO TIP Decirel a la "Dame directamente el contenido para compiar y pegar sin acotar nada mas." me ahorro el inicio ylas consclusiones o preguntas de follow-up
--

* Me genero este prompt

```
Quiero que actúes como un analista senior especializado en inversiones inmobiliarias en la Ciudad Autónoma de Buenos Aires (Capital Federal), con enfoque financiero, estratégico y urbano. Necesito que redactes un informe profesional, profundo y basado en datos actuales del mercado inmobiliario argentino.

El objetivo del informe es ayudarme a identificar las mejores oportunidades de inversión inmobiliaria en CABA, analizando qué barrios ofrecen mayor potencial según distintos perfiles de inversión y estrategias posibles.

El informe debe incluir:

* Análisis general del mercado inmobiliario actual en Capital Federal.
* Contexto económico argentino y su impacto en el real estate.
* Evolución de precios por m² en distintos barrios.
* Comparación entre barrios consolidados, emergentes y en crecimiento.
* Identificación de barrios con mayor potencial de valorización futura.
* Rentabilidad estimada por alquiler tradicional y alquiler temporario.
* Análisis de oferta y demanda.
* Tipos de propiedades más convenientes según el barrio (monoambientes, 2 ambientes, PH, oficinas, locales, etc.).
* Estrategias recomendadas según presupuesto:

  * bajo
  * medio
  * alto
* Qué conviene hacer en cada barrio:

  * comprar para alquilar
  * comprar para refaccionar y vender
  * desarrollo inmobiliario
  * alquiler temporario
  * renta en dólares
  * compra especulativa
* Riesgos y oportunidades de cada zona.
* Impacto de factores urbanos:

  * transporte
  * seguridad
  * turismo
  * universidades
  * polos gastronómicos
  * oficinas
  * desarrollo urbano
* Comparación entre inversión inmobiliaria y otras alternativas financieras en Argentina.
* Recomendaciones concretas y accionables.
* Escenarios posibles a corto, mediano y largo plazo.
* Conclusión final indicando dónde invertiría un inversor inteligente hoy y por qué.

Quiero un enfoque extremadamente analítico, estratégico y realista. Utilizá tablas comparativas, rankings, ejemplos concretos y conclusiones claras. El informe debe tener tono profesional, como si hubiera sido elaborado por una consultora inmobiliaria y financiera de primer nivel.

```

## Tecnica de Prompting : Interaccion

* AKA : Prompt Chainning , metodo socratico
* Encadenar Prompts en la conversacion para ir generando un contexto con informacion necesaria para que la ia pueda confeccionar una respuesta efectica

* Ejemplo quiero organizar la finanzas de la casa

* Prompt Generico

```
Dame consejos para organizar las finanzas de la casa
```

* Prompt con interaccion
```
Dame consejos para organizar las finanzas de la casa. Quiero que me hagas preguntas de a una hasta obtener el contexto necesario para darme consejos personalizados a mi persona.
```

> [!NOTE]
>  IMPORTANTE pedirle las pregutnas de a una sino te hace un cuestanario todo junto

* Claude te lo arma multiple choice
  * Dame consejos para organizar las finanzas de la casa. Quiero que me hagas preguntas de a una hasta obtener el contexto necesario para darme consejos personalizados a mi persona. Que las preguntas sean multiple choice y pueda elegir con el mouse

# Glosario

* FOMO : Fear of Missing Out
* Systen Prompt
* JailBreak : Hackear a la IA para que responda cosas que no tiene permitido

# PRoxima clase...

* Tecnica de prompting Rol / Persona
* Tecnica de promting PErsonalizacion de salida
