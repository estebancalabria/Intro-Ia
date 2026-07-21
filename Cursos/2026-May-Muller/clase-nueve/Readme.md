# Clase Nueve - 21 de Julio 2026

# Repaso

* Labs Google
  * https://labs.google/
  * Google Flow
      * Generacios de Videos
      * Gemeracio ilimita de imagenes con NannoBanna
      * Generacion de personajes o disenios consistentes 
* Agentes
  * Que es un agente
      * Componentes
          * LLM = Prompt  -> Genera Salida
          * Uso de Herramientas -> (ej busqueda web, interactuar con un sistema mio) -> Info de exterior
          * Base de conocimiento (RAG)
              * Permite responder no solamente basado en el conocimito durante su entrenamiento
              * Groundig : Anclar la respuesta en conocimiento especifico
          * Orquestador
  * NotebookLM
    * Un agente especializado en una base de conocimiento generado por nosotros

---

# Comparacion de Modelos

* URL
  * https://arena.ai/
* Caracteristica
  * Web abierta que mantiene actualizada la comparativa de LLM (tanto os como propietarios)

---

# NotebookLM

* URL
  * https://notebooklm.google.com/
  * https://notebooklm.google.com/notebook/b598f9e6-518a-4c11-a36b-06e597cc7ef9  << De este curso

---
 
# Privacidad de Datos

* Las preguntas que uno le pasa al chat quedan registrada en el propietario que a su vez puede llegar a usar esa Info para entrenar modelo
    * Cuando uno hace preguntas en lugar de decir
        * "Quiero recuperar la deuda de Juan Perez dni 234343443 como hago"
        * Tanto Juan Perez, con DNI son datos sensibles
        * Es facil de solucionar
          * "Quiero recuperar la deuda de <PERSONA_1> dni <DOCUMENTO_1> como hago"
    * El problema muchas veces es cuando adjuntas archivos donde no tenemos tanto control de que informacion hay ahi

* En general no pasa nada, es dificil demostrar que se usaron datos sensible
    * Pero si una persona se entera que se usaron sus datos sensibles para consultar la IA sin su consentimiento, puede iniciar acciones

* Altermativas/Consideraciones para uso de datos sensibles
  * Anonimizar los datos
  * Utiizar modelos Open Source Localmente
  * Leer y resguardar los contratos con los proveedores de IA
  

## Animizacion

* La posibilidad de anonimizar datos antes de usarlo
* Se puede anonimizar con modelos Open Source
* Tener version de los doscumentos original / anomizada para usar con IA

* Herramientas anonimizadoras
  * Open Source
    * https://huggingface.co/spaces/rgsouza2024/anonimizador_sinergia
  * Microsoft
    * https://language.cognitive.azure.com/home
  * ARX Anonixer (gratuita)
    * https://arx.deidentifier.org/
  * Librerias de Anomizacion (codigo)
    * Microsoft Presidio

* Ejemplo texto anonimizar
```
El día 15/07/2026, Juan Carlos Pérez (DNI 32.456.789) se comunicó con el área de soporte de ACME S.A.

Datos del cliente:
- Nombre: Juan Carlos Pérez
- Fecha de nacimiento: 22/09/1985
- DNI: 32.456.789
- CUIL: 20-32456789-4
- Pasaporte: AR1234567
- Email: juan.perez@gmail.com
- Email laboral: jperez@acme.com
- Teléfono móvil: +54 9 11 4567-8910
- Teléfono fijo: (011) 4321-9876

Dirección:
Av. Corrientes 1234, Piso 8, Depto. B
Ciudad Autónoma de Buenos Aires
Código Postal: C1043AAX
```

### Ejemplo con libreria de anonimizacion

```
from presidio_analyzer import AnalyzerEngine
from presidio_anonymizer import AnonymizerEngine
from presidio_anonymizer.entities import OperatorConfig

# Crear motores
analyzer = AnalyzerEngine()
anonymizer = AnonymizerEngine()

texto = """
John Smith lives in New York.

His email is john.smith@gmail.com.

His phone number is (212) 555-1234.

His credit card is 4111-1111-1111-1111.
"""

# Detectar entidades
results = analyzer.analyze(
    text=texto,
    language="en"
)

# Configurar el reemplazo por tipo de entidad
operators = {}

for entity in results:
    operators[entity.entity_type] = OperatorConfig(
        "replace",
        {
            "new_value": f"<{entity.entity_type}>"
        }
    )

# Anonimizar
resultado = anonymizer.anonymize(
    text=texto,
    analyzer_results=results,
    operators=operators
)

print(resultado.text)
```

## Modelos Open Source

* Uso de un LLM Local
  * LMStudio
  * Ollama
  * ...
* Repositorio de Modelo Open Source
  * Hugging Face
    * https://huggingface.co/
    * Organizacion sin fines de lucro que nuclea un repositorio de todos los modelos Open Source
    * Cualquier modelo OS que utilicemos se baja de aca
    * Tiene los SPACES donde puedo probar modelos OS sin descargarlos con un limite diario

## Contratos con los Proveedores de IA

* Los proveedores de IA (OpenAI, Microsoft, Anthropic)
  * Tienen distintos contratos
    * Para Particulares
    * Para Empresas
  * Claude
    * Pro : Uso personal / domestico (no apto para usar con datos sensibles)
    * Para Empresas : https://www.anthropic.com/news/claude-for-small-business
        * DPA (Data Processing Agreement) <<< Uno tiene que guardarse una copia y ante cualqueir reclamo tenerlo como resguardo para mostrar que la empresa tiene un tratamiento con datos sensibles
  * OpenAI
    * https://openai.com/es-ES/solutions/
  * Microsoft
    * Azure Foundry 
  
---

## Manejo de Datos Sensibles y Empresas

* Manuales de procedimiento que demuestren que la empresa sabe que es un dato sensible y que lo trata con responsabilidad
  * Procedimiento de DLP (Data Loss Prevention) : Como minmimiza la empresa que los datos se escapen y que no se usen para otra cosa que se espera de ellos
* Identificado y estandarizado los lugares donde almacena la infromacion
  * Catalogo de datos
* Clasificados que documentos tienen datos sensibles y cuales no
* Tiene que tener identificados para que de usa cada fuente de datos
* Indentificar los owners y resposables de cada datos
  * Identificar los canales de comnunicacion y permisos de quien tiene acceso a cada dato
* Plan de capacitacion

### Herramientas para gestion de datos a nivel corpotativo

* Microsoft Purview
  * https://purview.microsoft.com/
* Dataplex
* AWS Glue Data Catalog
* Colibra
  * https://www.collibra.com/

---

# Notiicias

* https://www.eluniversal.com.mx/mundo/anthropic-debera-pagar-mil-500-mdd-por-libros-pirateados-para-claude-la-mayor-recuperacion-por-derechos-de-autor-de-la-historia/
  
