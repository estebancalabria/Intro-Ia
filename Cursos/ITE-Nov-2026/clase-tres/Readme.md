# Clase Tres - 16 de Noviembre del 2026

# Repaso

* LLM
  * Propietarios
    * ChatGPT
      * Redaccion con Lenguaje Natural
    * Claude
      * Tareas Tecnicas y Programacion
    * Gemini
      * Integracion con Ecosistema Google
      * Busqueda e investigacion Web
    * Copilot
      * Paredido a Gemini pero con el ecosistema 365
      * Apunta a corporaciones y proteccion de datos empresariales
    * Perplexity
      * Investigacioes Academicas
    * Grok
      * Tendendencias / Grounding en Redes
      * Baja censura
  * OS
    * Qwen
      * El ChatGPT OS (copia)
      * El estandar si queres instalar un modelo os local
    * Kimi
      * Similar a Claude con Enfoque Tecnico
    * Mistral
      * Enfoque a la legislacion Europea
* Comparar modelos
  * Arena.AI
    * Para estar actualizado en los modelos que salen
* Open Souce
  * Ejecucion Local
    * LMStudio (muy facil de de usar)
    * Ollama
  * Hugging Face (HF)
    * Listado de modelos
    * Codigo para usarlos en python
    * Spaces

---

# Prompt Engineerig

## Antomia de un prompt

Prompt = Tarea + Contexto + Rol + Ejemplo +  Formato + Tono

## Tips

* Usar la IA como experto en prompt engineerig
 * Le pongo el prompt como me sale y deje que la IA mejor

## Rol / Persona

* Objectivo
 * Decirle desde que lugar queremos que la IA nos de una resputesta

* Abrimos 4 solapas de ChatGPY
  * Prompt solo con la tarea (sin sol)
    * Promponeme un alrmuerzo para hoy. Dame una propuesta sin preguntar nada.
  * Con un rol especifico
    * Actua como una nutricionista especializado en salud y bienestar. Quiero que me propongas un almuerzo para hoy sin preguntar nada.
  * Desde la perspectiva de una persona conocida
   * Quiero que seas el Chef José Andrés y me propongas una comida para mi almuerzo.,
  * Citar un panel de expertos
   * Quero que me armes un panel de experto con distintos roles y que cada uno (maximo dos parrafos) me proponga una comida para hoy para mi almuerzo.

### Ejemplos

* Podemos ver algunos ejemplos en:
  * https://github.com/estebancalabria/Intro-Ia/tree/main/Prompt%20Engineering/Patrones%20de%20Prompting/Persona
* Por ejemplo

```
Quiero que actúes como una hoja de cálculo basada en texto. Solo responderás con una tabla de 10 filas, con los números de fila a la izquierda y las columnas de la A a la L. La primera celda de cada fila estará vacía para referenciar el número de fila. Te diré qué escribir en cada celda y tú solo me responderás con el resultado de la tabla, sin explicaciones. También te escribiré fórmulas, y tú me responderás solo con la tabla actualizada. Primero, respóndeme con una hoja vacía.
```

---

## Contexto 

* Contexto = Lo que escribis en el prompt + Toda la conversacion + Instrucciones Personaliadas + System Prompt + Memoria + Busqueda con Herramientas o busqueda web
* Muchas veces la IA me da mejores respuesta cuanta mas informacion tiene y es ahi donde resulta util aplicar el modo dictado y en vez de escribir prompts cortitos darle a la Ia todo el contexto para que trabaje

### Interaccion o Prompt Chainning (encadenamiento de prompts)

* Idea
  * Encadenar prompts generando una convesacion que tenga el contexto necesario antes de de pedirle la respuesta concreta de lo que quiero
 
* Interaccion
 * Le voy a pedir a la IA que me haga pregutnas "DE A UNA" para responder de forma mas precisa
 * Utlimamente los LLM a veces lo implementan sin que se lo ida

* Ejemplo

```
Dame una propuesta para comer hoy para mi almuerzo. Haceme pregutnas DE A UNA para obtener el contexto suficiente para encontrar la mejor propuesta de comida personalizada para mi."
```

 
---
# Break
HAsta y 15
---
