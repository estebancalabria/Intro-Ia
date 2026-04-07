# Clase Tres - 7 de Abril del 2026

# Repaso

* Large Language Models
  * Propietarios
    * ChatGPT
    * Claude
    * Gemini
    * Grok
    * Perplexity
  * Open Source
    * Huggig Face
* Herramientas
  * Text-To-Speech
      * NaturalReaders
      * ElevenLabs

# LLM

* Propietarios
* Open Source
  * Chinos
    * Los desafio a que ponga el cartel de pagar para seguir usando
    * DeepSeek
    * Qween
  * Americanos
    * Familia Llama (lo tenemos en Wsap)
  * Europeos
    * Mistral
        * FRANCIA SEGUNDO!

## Propietarios

> Copitot

* Microsoft apunta al nicho coorporativo
* Hace mucho enfasis en seguridad

## Open Source

* Los modelos Open Source si tengo una buena computadora (GPU) lo puedo descargar localmente (25 GB o  lo que ocupe)
* Utilizar un programa local para hablar con ese modelo
    * Suele ser mucho mas lento
* Podemos utilizarlo con informacion sensible sin que ninguna empresa nos espie
    * No necesitan conexion a internet
* Seguridad
    * https://www.instagram.com/p/DOqu-k8Dvfb/?img_index=1

### DeepSeek

* Fue el primero en incorporar el modo razonamiento profundo o "pensado"
* Optimizado a mas no poder para lograr una performance en su momento igual o mejor a ChatGPT
  
> https://chat.deepseek.com/

* Ejemplo de prompt

```
En una habitacion hay tres personas. Una de ellas es un asesino. Entra un cuarto y mata al asesino. Cuantos asesinos vivos quedan en la habitacion
```

### Qwen

* El modelo favorito del profe
* Es el clon Chino de ChatGPT
* Desarrado por AliBaba
* La calidad es comparable a ChatGPT pero el uso gratuito es mas amplio...

> https://chat.qwen.ai/


### Uso de LLM Localmente

* Ideal para
    * Trabajar con datos sensibles
    * Para entornos corporativos donde la info no debe salir de la empresa
* Alternativas para uso
    * Ollama (MEdiante linea de comando) : https://ollama.com/
    * LMStudio (Aplicacion de Escritorio) : https://lmstudio.ai/
    * OpenWebUI : https://openwebui.com/
        * No recuerdo si te permite descargar el modelo local como las otras
* Todos los modelos Open Source que usamos los descarga de HuggingFace

* Como entra en juego JAN con todo esto
  * https://www.jan.ai/
  * Lo veo para la proxima

## Comparativa de Modelos de Lenguaje

* Como nos mantenemos actualizados en modelo de lenguaje y evitamos el
  * FOMO : Fear of Missing Out

> https://arena.ai/

* Ranking de Modelos de IA armado con la votacion de la gente

---

# Prompt Engieenring

## Funcdamentos de Prompt Engineering

> https://www.instagram.com/p/C5MDsQiR5cG/?img_index=1

* Buen Prompt
  * Tarea
  * Contexto
     * Toda la informacion que la IA usa para responder = Prompt + Conversacion + System Prompt (Intrucciones Personalizadas) + Memoria + Conversaciones pasadas
     * Esta bueno usar el microfono y hablarle largo y tendido para no escatimar contexto
     * OJO : El modo voz de chatgpt en celular es malo esta pensado para que sea mas fluido al hablar y no responde tan bien
  * Ejemplos
  * Rol/Persona  <<<<
  * Formato   <<<
  * Tono

* Van a encontrar formulas parecidas como RAFA = Rol + Acccion + Formato + Antecedentes/Audiencia

## Patron Rol/Persona

* Abrimos 4 solapas de ChatGPT
  * Prompt Simple
      * "Ya son casi las 13:00 decime que comer."
      * https://chatgpt.com/share/69d52903-1104-83e9-80c1-ebf2f3b5cc9d
  * Mismo Prompt dirigido a una persona
      * "Actua como un nutricionista vegano de comida macrobiotica que optimiza todos los aspectos de la nutricion de una persona. Ya son casi las 13:00 decime que comer."
      * https://chatgpt.com/share/69d52917-f28c-83e9-b70d-dbc87ab2c598
  * Mismo prompt a un personaje especifico
      * "Actua como Jaime Oliver. Ya son casi las 13:00 decime que comer."
      * Es la opcion divertida
      * https://chatgpt.com/share/69d52963-0f40-83e9-a46a-bde3bfdbc888
  * Citar un panel de expertos de distintas areas
     * "Quiero que me armes un panel de experto donde cada uno me conteste una propuesta.. Ya son casi las 13:00 decime que comer."
     * Muy util para analizar algo desde distintas perspectivas
     * <<< MUY BUENO
     * https://chatgpt.com/share/69d529a7-f084-83e9-8d60-244e32b5eab9

## Cadena de Razonamiento (Chain of toughts)

> Modo pensado ya no se hace

## Patron interaccion (Contexto)

* PROXIMA CLASE
* Propuesta "Como llegar a fin de mes"


---

# Speech 

# Text-A-Voz

# Voz-A-Texto

* Uso herramientas como 

> https://tactiq.io/es

* Workflow
  * Grabo la charla con Wsap
  * La transcribo con Tactic
  * La paso por un llm y la uso como contexto
    * Si tiene datos sencibles ---> Uso LLM local
    * Si no hay nada comprometedor ----> Uso chatgpt o el que me guste mas segun lo que necesito

# Glosario

* Alucinar : Cuando el LLM responde cualquiera
* 
