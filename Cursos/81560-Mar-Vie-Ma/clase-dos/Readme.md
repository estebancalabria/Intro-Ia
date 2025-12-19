# Clase Dos - 19 de Diciembre del 2025

# Repaso

* Large Largunage Models (Modulo 1)
  * Modelos Propietarios
    * ChatGPT
        * Trata de simular conversacion humana
        * Tiene personalizacion y memoria
    * Gemini
        * Facts / Hechos
        * Integracion completa con el entorno de Google
        * Modo Investigacion
    * Claude
        * Creacion de Artefacto
        * Bueno para programacion y cosas tecnicas
* Herramientas (Modulo 3)
    * NaturalReaders
    * Napkin

# Large Language Models

- ## Modelos Propietarios

* Grok
    * https://grok.com/
    * El modelo de Elon Musk
    * Suele tener visiones ma creativas / distintas
    * Su modelo es el que menos censura tiene
    * LA generacion de videos en groq es una locura, super facil
    * Dicen que destaca en busquedas web
    * Puntaje : 9 / 10
* Perpeplexity
    * https://www.perplexity.ai/
    * Ideal para investigaciones cientificas
    * El mejor en el tema de citar fuentes de donde saca la informacion
        * Ejemplos "Quiero hacer una investigacion actualizada sobre la calvicien en estados unidos, su evolucion, si aumenta con el tiempo, disminuye, los factores ambientales." (Elegir solo fuentes academicas)
* Copilot
   * https://copilot.microsoft.com/
   * Microsoft no tiene su propio LLM
   * Es una version custimazada de ChatGPT pero muy etica
   * Ideal para que lo usen los ninios, lo mas eticos, censurado y policamente correcto

### Riesgos de modelos propietarios

* Dependencia de la conectividad
* Privacidad de los datos
   * No ingresar nunca informacion sensible en los modelos de lenguaje
   *https://www.instagram.com/p/DOqu-k8Dvfb/?img_index=1
* Si las empresas se ponen de acuerdo y te cobran 10000 millones de dolares por usar sus modelos no podes haer nada 

- ## Modelos Open Source

* Familia LLama
  * Los de Meta, los de Mark Zuckemberf
  * Se pueden usar directamente en Wsap con @Meta o lo tienen como contacto
* Los Chinos
  * Deepseek
     * https://chat.deepseek.com/
     * Fue el primero en introducir el modo razonamiento
        * El modo razonamiento es la implementacion interna directamente dentro del modelo de un patron de prompting Chain of thoughts que se usaba para resolver problemas complejos y de logica
     * Fueron los pioneros en modo razonamiento
        * Ejemplo : "Hay una habitacion con tres personas. Uno de ellos es un asesino. Entra una cuarta persona a la habitacion y mata al asesino. Cuantos asesinos vivos quedan en la habitacion."
        * Ejemplo : "Una mesa tiene 4 patas de 100cm salvo una con 101cm. Etiqueta las 4 patas y dime qué probabilidad tiene cada pata de estar apoyada en un suelo perfectamente..."
  * Qwen
     * https://chat.qwen.ai/
     * **El modelo preferido del profe**
     * Copia todo lo que tiene ChatGPT (Memoria, Personalizacion)
     * No le encontre el limite de uso...
     * No tiene la amabilidad forzada que ChatGPT tiene por defecto
  * Kimi-K2
     * Es un Mixture of Experts
* Hay muchos lugares donde ejecutar Modelos OS, pero la mejor online es Groq
     * Es groq con q (No confundir con el Grok de Elon Musk)
       * Es moto de inferencia (Hostea modelos Open Source Existentes)
       * Tiene una arquitectura especial para ejecutar los LLm que se llama LPU (Language Processsing unit), logran la velocidad de ejecucion mas rapida del mercado
       * Tiene una API KET Gratuita.

# Novedades

* Tesis de Leo ente repo : Cursos/81560-Mar-Vie-Ma/clase-dos/montesano 2014.pdf
* Sobre la deuda cognitiva : https://www.researchgate.net/publication/392560878_Your_Brain_on_ChatGPT_Accumulation_of_Cognitive_Debt_when_Using_an_AI_Assistant_for_Essay_Writing_Task
 
 # Glosario

* Jailbreak : Encontrar la manera mediante un prompt de burlar la censula del modelo de lenguaje
* Tokens : Una palabra, silaba que es la unidad de medida / prediccion del modelo de lenguaje
    * https://platform.openai.com/tokenizer
    * Descubriminto : No es lo mismo todo en MAYUSUCula que todo en todo en minuscula. La primera consume mas tokens
* Cantidad de Parametros : Nos habla del tamaño del modelo de lenguaje.  Relacionado con la cantidad de neuronas del modelo de lenguaje. Cada parametro es el peso de una conexion entre neuronas.
* Deuda Cognitiva: hablamos de eso... 

# Proxima Clase...

> Les explico como ejecutar un modelo de lenguaje (Open Source) en su computadora...
> Comparar llms
