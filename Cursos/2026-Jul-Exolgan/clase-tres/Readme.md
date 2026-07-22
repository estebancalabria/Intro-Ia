# Clase Tres - 22 de Julio del 2026

# Repaso

* Large Language Models
  * Caracteristicas
      * Cada modelo destaca en algo
          * Claude
            * Era bueno para tareas tecnicas y programacion
            * Hicimos el pong
      * Uso de la Memoria
          * ChatGPT
          * Copilot
      * Respuestas editables (Canvas / artefacto)
          * ChatGPT
          * Copilot
          * Claude
            * Previsualizacion: Artefacto con el pong
      * Integracion con su ecosistema
          * Gemini -> Integracion con el ecosistema de google
              * Generacion de eventos en el calendar
              * Reserva de vuelos y hoteles con google flights y google hotels
          * Copilot -> Integracion con ecosistema 365
  * Agentes (vista preliminar)
      * Agentes Preconstruidos
          * Agente Investigador
              * Gemini (Modo Investigacion)
              * Copilot (Agente Investigador)
              * Perplexity (Investigacion Academica)
      * Agentes Hechos por nosotros
* Herramientas
  * Napkin
      * Enriquecer un texto con graficos / diagramas

---

# Modelos de Lenguaje

## Modelos Propietarios

### Grok

* URL
  * https://grok.com/
* Caracteristicas
  * Es el que menor grado de censura tiene
  * Buena groundig, siempre busca en la web y en X antes de responder
  * Previamente se podian generar videos rapido y gratis con grok, ahora esa funcionidad es paga

## Modelos Open Source

* Chinos
  * Deepseek
  * Qwen
  * Kimi-K3
* Ameicanos
  * Familia llama (MetaAI que esta en wsap)
* Europeos
  * Mistral

### DeepSeek

* URL
  * https://chat.deepseek.com/
* Noticia
  * https://www.elfinanciero.com.mx/tech/2025/12/10/deepseek-usa-chips-nvidia-prohibidos-por-trump-para-su-modelo-de-ia/
* Caracteristicas
  * Intrujo el modo razonamiento
    * Ahora lo tienen todo:
        * Gemini -> Extended thinking segun el modelo
        * Copilot -> Razonamiento Producto

* Problema de los asesinos
```
En una habitacion hay tres personas. Uno de ellos es un asesino. Entra una cuarta persona a la habitacion y mata al asesino. Cuantos asesinos vivos hay en la habitacion luego.
```

### Qwen

* URL
* Caracteristica
  * Modelo entrenado por la gente de AliExpress
  * Es el modelo OS mas parecido en funcionalidades a ChatGPT
  * Fue el preferido del profe por mucho tiempo

* Probanos la multi modalidad
  
* Interprete de codigo
  * Muy util cuando quiero analizar un excel
  * Si yo adjunto en cualquier LLM un excel grande, el llm no lo va a leer todo
  * Capacidad de generar codigo en python y ejecutarlo para calculos complejos
  * Adjuntarle un archivo y pedirle que sobre el archivo haga algun calculo

```
Dado el archivo adjunto usar el interprete de codigo para calcular la sumatoria, el promedio, la media y la mediana de los valores en la segunda columna
```

---

# Glosario

* Censura / Guardriels/ Guardarieles : Protecciones de los modelos de lenguaje para no tratar temas que podrian daniar u ofender a alguna persona
* Grounding : Anclar la respuesta del modelo en fuentes verificable
* Multimodalidad : Capacidad que tiene los modelos de lenguaje para no solo trabajar con texto, sino tambien con imagenes y archivos
* OCR : (Optical Character Recognition) : La capacidad que da la IA de reconocer y entender el texto en una imagen
