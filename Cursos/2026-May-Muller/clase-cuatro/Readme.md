# Clase Cuatro - 9 de Junio del 2026

# Repaso

* Herramientas
  * There IS an AI For That
  * Natural Readers
* LLM
  * Open Source
    * HF : Hugging Face
      * Respositorio para subir modelos open source
      * Space de HF
    * Mistral
    * Groq
    * Ejecutar Modelo Localmente
      * LMStudio
      * Ollama
  * Propietarios
    * Grok
    * Gemini
      * Modo Investigacion
* Prompt Engineerings
  * Formula = Tarea + Contexto (Memoria + SystemPrompt + InstruccionesPersonalizadas + Herramientas) + Ejemplo + Rol + Formato + Tono
  * Tip : Usar Microfono para mas conxtexto
  * TIP : Usar la IA como prompt Engineering
  * Patrones/Tecnicas de Prompting
    * Contexto
      * Prompt Chainning / encadenamiento de Prompts / Metodos Socratico

---

# Herramientas

## Napkin

* URL
  * https://www.napkin.ai/
* Caracteristicas
  * Permite enriquecer un texto con imagenes/diagramas
* Puntaje
  * 9 / 10

---

# Prompt Engineering

## Rol

* Solapa 1 : Prompt Solo Tarea
  * "Dame estrategias para cobrar una deuda a un cliente moroso"
  * https://chatgpt.com/g/g-p-6a04b4fb70008191b7deeecd6ae4ba19-promting-rol/shared/c/6a28429b-4058-83e9-af78-9c032c22967d?owner_user_id=user-FiOaCNjhGgtJ4Aa4tiv8Ommy
* Solapa 2 : El mismo prompt especificando un rol
  * "Actua como un experto en persuacion nivel fbi especialista en morosidad y cobre de deudas. Dame estrategias para cobrar una deuda a un cliente moroso"
  * https://chatgpt.com/g/g-p-6a04b4fb70008191b7deeecd6ae4ba19-promting-rol/shared/c/6a28429d-4810-83e9-9e42-3ceb917324a3?owner_user_id=user-FiOaCNjhGgtJ4Aa4tiv8Ommy
* Solapa 3 : El mismo prompt especificando una persona especifica
  * "Actua como Ricardo Fort. Dame estrategias para cobrar una deuda a un cliente moroso"
  * https://chatgpt.com/g/g-p-6a04b4fb70008191b7deeecd6ae4ba19-promting-rol/shared/c/6a28429f-6a6c-83e9-ad46-d984a82b88c4?owner_user_id=user-FiOaCNjhGgtJ4Aa4tiv8Ommy
* Solapa 4 : Citar a una panel de experto (varios roles)
   * "Quiero que armes un panel de expertos donde cada uno daestrategias para cobrar una deuda a un cliente moroso. Quiero un parrador o pocos parrafos segun cada experto. "
   * https://chatgpt.com/g/g-p-6a04b4fb70008191b7deeecd6ae4ba19-promting-rol/shared/c/6a2841ee-4938-83e9-adc1-f2f599a30f64?owner_user_id=user-FiOaCNjhGgtJ4Aa4tiv8Ommy

## Formato

* Algunos formatos que debemos conocer para sacarle todo el jugo a la IA

* Lista sin formato
  * "Dame una lista de compras mensual para una oficina. Producto, cantidad, departamento,  precio, motivo. Los datos pueden ser aproximados. dame la lista de 10 elementos."
 * Formatos Tecnicos
   * JSON
    * Dame la lista en json
   * XML
    * Dame la lista un xml
* Formatos Pseudo Tecnicos
  * HTML (el de la web)
   * Sirve, por ejemplo para generar pds 
     * "Generame la lista en un unico html profesional y elegante que se pueda mandar a mi jefe"
     * Luego "Me generas el html para desgargar"
     * Click en achivo para descargar el html
     * Ctrl+P lo podes imprimir como pdf
* Formato para Interactuar con Excel
  * CSV (Comma Separated Values)
  * "Dame la lista como un csv"
   


---

# Glosario

* La Ia no es deterministica : El mismo prompt no siempre devuelve la misma respuesta
