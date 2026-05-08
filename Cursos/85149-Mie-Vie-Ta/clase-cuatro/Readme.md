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

## Tip de contexto

* Usar el modo dictado para dar mas conexto en nuestros prompts

* No es lo mismo poner

```
Escribime un mail para decir que no voy a ir atrabaja hoy
```

* Que usando el modo dictado decir

```
Hola, me gustaría escribir un mail diciendo que no voy a ir a trabajar, dando una excusa muy verosímil. Te dejo en tus manos que invente la excusa y aplicando a la emotividad, ¿no?, sabiendo que mi jefe es hincha de Racing y que es una persona que no se toma muy bien los faltazos. Entonces me gustaría tratar este tema con mucho, mucho tacto, encontrarle la vuelta para que no se enoje, tratar de justificarlo muy bien. Mi jefe responde mucho mejor a los mails que son muy emotivos y muy persuasivos, así que espero que me hagas un mail que cumpla esas características.
```

## Tecnica de Prompting : Interaccion

# Glosario

* FOMO : Fear of Missing Out
* Systen Prompt
* JailBreak : Hackear a la IA para que responda cosas que no tiene permitido
