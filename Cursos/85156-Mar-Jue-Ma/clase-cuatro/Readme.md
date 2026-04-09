# Clase Cuatro - 9 de Abril de 2026

# Repaso

* Open Source
    * LLM
      * DeepSeek
      * Qween
      * Mistral : Siempre segundo
    * Hugging Face (HF)
        * El lugar/repositorio donde se suben los modelos Open Source
            * Por Ejemplo el modelo flux  de generacion de imagenes esta en HF
        * Tiene "Spaces" para probar online modelos Open Source (no solo de texto sino de todo tipo
    * LM Studio
        * Un aplicacion de escritorio que se DESGARGA los LLM de HF localmente y te permite ejecutarlos
        * Ideal para trabajar localmente con Datos Sesibles
* Prompt Engineering
    * Formula de Microsot (Alternativa al RAFA) :  Tarea + Contexto + Ejemplo + Rol + Formato + Tono
          * Contexto = Prompt + Conversacion + System Prompt (Instrucciones Personalizadas) + Memoria + Conversaciones Pasadas + (Tools como Busqueda Internet)
    * Patrones de Prompting
        * Rol/Persona
* Herramienta
    * Tactiq

# Aspectos de LLM

* La IA tiene SESGOS (Prejuicios) y comete ERRORES
  * La ia no es su valor agregado no cometere Errores
  * Poreso es IMPORTANTISISMO validar y controlar lo que dicen
  * Lo que tenemos que aportarle como personas a la IA es el Criterio

# Prompt Engineering

## Patrones de Prompting : Interaccion

* Objetivo : Armar el contexto de forma mas efectiva
* Patron Relacionado : Prompt-Chaining (Ir encadenado prompts para armar el contexto de la conversacion)
* Idea : Pedrile a la IA que me pregunte a mi la informacion que necesita para darme una respuesta mas efectiva

* Ejercicio
    * Prompt Sin Interaccion
        * Armame una dieta general de la semana
    * Prompt con unteraccion
        * Armame una deita de la semana personalizada especialmete para mi. Quiero que me hagas preguntas de A UNA hasta que tengas todo el contexto necesiario para armarme la dieta optima. Hace todas las pregustas que necesites y recienc uando tengas toda la informacion necesaria armame la dieta.

> [!NOTE]
> Este patron de prompting es un viaje de IDA!

## Patrones de Prompting : Personalizacion de salida

* Los LLM generan texto. Es importante conocer los formatos con los que se llevan bien
* Vamos a pedirle a la IA una lista y la vamos a mostrar en distintos formatos y ver para que me sirve cada uno
    * Quiero una lista de 10 razas de perros. Su peso, tamanio, color, personalidad, edad, utilidad, alguno famoso
* Formatos
    * XML / JSON : Formatos mas tecnicos
        * Dame la lista como JSON
        * Dame la lista como XML
    * HTML
        * Original: Dame la lista en HTML
        * Mejorado : Dame la lista en un html que se vea profesional, elegante, que es para compartir a mis clientes. Luego lo voya  imprimir como pdf.
        * Ideal para generar PDFs (para mandar a clientes, para darle formatos especificos)
            * ACLARACION: A algumos LLM ya le podes pedir directamente el pdf
    * CSV (en espania Ce - Se - Uve)
        * Texto Separados por comas
        * Es un formato que Excel entiende de forma nativa (Aunque nosotros vamos a trabajar con Google Sheets)
        * Si trabajo con Gemini es mucho mas facil generar la planilla y necesito este formato le pido directamente una tabla

# Citas de Alumnos

* Juan Ignacio : Yo cuando lo uso en mi trabajo termino aprendiendo más y mucho más rápido. Ya busca por mi las fuentes y me plantea posibles errores que jamás hubiese tenido en cuenta. Estoy como soporte técnico. Lógicamente tenes que tener un conocimiento previo, pero como herramienta profesional a mi me ayuda a ser super eficiente. El tema es saber ponerle un freno, no me siento seguro que toda mi vida la organice una maquina
* Lorena : La IA potencia si sabemos como usarla

# Glosario

* AGI : La Inteligencia Artificial General (AGI) es un tipo de IA hipotética capaz de entender, aprender y aplicar conocimientos en múltiples dominios de manera flexible, igualando o superando las capacidades cognitivas humanas. A diferencia de la IA estrecha actual, la AGI busca resolver cualquier tarea intelectual, razonar, planificar y crear autónomamente. 
