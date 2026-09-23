# Clase Dos - 23 de Septiembre del 2026

# Repaso

* Fundamentos de IA
  * Modelos Propietarion vs Open Source
  * Funcionamiento de la IA
    * Token
      * Tokenizacion
    * Contexto
      * (prompt) -> (system prompt) + (pesonalizacion) -> (memoria) -> (herramientas/ busqueda web) -> (conversaciones previa) ->(IA)
    * Entrenamiento costos
  * Uso
    * Instrucciones Personalizadas -> Personalizacion de las Respuestas
    * Uso de la Memoria
  * Conceptos
    * Grounding
    * Alunacion
      * Importancia de verificar lo que dice la IA
    * No deterministica : el mismo prompt no genera siemrpe el mismo resultado

# Historia

* Abogado hizo su alegato con chatgpt pero el modelo invento la jurisprudencio
    * https://litigio.com.ar/2025/08/27/un-abogado-cito-jurisprudencia-inventada-por-chatgpt-y-el-tribunal-advirtio-al-colegio-de-rosario/

# Modulo 2 : IA Generativa

* Modelos de Lenguaje (LLM)
  * Propietarios
      * ChatGTP (https://chatgpt.com/)
        * Empresa : OpenAI
        * Caracteristicas
          * Trata de emular conversacion humana
          * Bueno para escribir mails, redaccatar informes
      * Copilot
        * Emprese : Microsoft
        * Ojo hay dos copilot, el que se usa en 365 con subscripcion (https://m365.cloud.microsoft) y el domestico para uso general (https://copilot.microsoft.com/)
        * No es un modelo, sino que por detras usa otros modelos como chatgpt o claude
        * Su uso es espcial para empresas, porque no usa los datos para entrenar modelos
        * Preprocesa los prompts y aplica filtros de etica
        * Copilot 365 (pago)
          * Integracion con el ecosistema de 365 (Word, Outlook, Calendar)
      * Claude
        * Empresa : Antrhopic
        * Ahora se queda sin credito enseguida, cada vez te da menos la version gratuita
        * Especial para tareas tecnicas (IT, construccion, fisica, etica)
        * El modelo que mas se usa para programar
        * Tiene artefactos (previsualizacion del resultado final)
      * Gemini
        * Empresa : Google
        * Busca reemplazar/complementar al motor de busqueda
        * Optimizado para el grouning (buscqeuda web) y basar las respuestas en conocimientico factico (hechos)
        * Integracion de productos del ecosistema google
          * Google Calenndar
            * "Generar un evento en mi calendar a las 16:30 que sea ir al medico"
          * Google Flights y Google Hotels
            * "Quiero viajar a las Maldivas desde Madrid haciendo escala en Gran Canaria para 3 personas. Quiero irme 15 dias. Buscame opciones de alojamiento y hoteles en google flighs y google hotels."
        * Lo mejor que tiene es el modo investigacion
          <img width="527" height="245" alt="image" src="https://github.com/user-attachments/assets/ef26db82-25f6-4113-a00a-fe78301cbdff" />
        * Primero hace una planificacion de la investigacion  
      * Grok
        * Empresa : X (Elon Musk)
        * Caracteristicas
          * Muy buen Grounding actualizado (busca todo X, tendencias)
          * Perdismo, tendencias, analisis de mercado
            * "Cual es el actor que esta mas en tendencia esta ultima semana"
          * Es el mas irreverente de todos, menos filtros
          * El que menor grado de censura tiene (+18)
            * Contame un chiste subido de tono.
            * Palabrotas, mal hablado
      * Perplexity
        * https://www.perplexity.ai/
        * Caracteristica
            * El modelo utilizado en ambitos academicos para hacer investigaciones cientificas
        * "Quiero hacer una investgacion actulizada sobre las ultimas teorias e investigaciones sobre el origen del unverso"
  * Open Source
    * China
      * Qwen
        * El modelo chino de Alibaba / AliExpress
        * Trata de imitar en todo a ChatGPT
        * No te quedas sin limite tan rapido (no conozco el limite de uso)
        * Bueno para procesar mucho texto y no quedarte sin tokens
        * Beno para generar videos rapidamente
        * Muy bueno para hacer videos (ahora te los cobra)
      * DeepSeek
        * Fue el primer modelo chino en incorporar el modo pensado el cual obliga al modelo a exteriorizar su razonaminto lo que provoca respuestas mas correctas y precisisas para problemas de logica
        * Noticia : https://www.cnbc.com/2026/08/19/china-ai-nvidia-chips-us-export-controls.html
        * "Hay una habitacion con 3 personas. Uno de ellos es un asesino. Una cuarta persona entra a la habitacion y mata al asesino. Cuantos asesinos vivos hay luego en la habitacion."
      * Kimmi-K3
        * El open Source para lo tecnico
        * Competencia de Claude pero no se acaba tan rapido (No llegue nunca al limite)
        * https://www.kimi.ai/es-419
    * Europeos
      * Mistral
      * https://chat.mistral.ai/
      * Proteccion de datos y GPDR
        * https://chat.mistral.ai/work/1dba201b-2466-48c1-aaf7-3a9c1ae978e2

---

## Caracteristicas de los modelos
     * Son redes neuronales (neuronas conectadas entre si)
     * Cantidad de parametros
     * Se puden diferenciar en
       * https://www.instagram.com/p/DKhQrTvuFcw/?img_index=7
           * Modelos de Chat
           * Modelos de Razonamiento

---

## Como se el esta actual de los LLM


---

## Como instalo un modelo Open Source en Mi computadora

* Cuando necesito la maxima privacidad

---

# Modulo 3 : Prompt Engineering

> [!NOTE]
> Utilizar una IA como mejorador de prompts

* Ejemplo
```
Actue como un especialista en prompt engineering y quiero mejorar este prompt para una investigacion profunda con gemini. Dame el prompt mejorado "Quiero una investigacion produnda analizando las mejores opciones de inversion hoy en dia en Espania. "
```

* Me devuelve

```
Quiero que realices una **investigación profunda, rigurosa y actualizada sobre las mejores opciones de inversión disponibles para una persona física residente fiscal en España a fecha de hoy**.

No quiero una respuesta genérica ni una lista superficial de productos. Quiero un análisis comparable, basado en datos actuales y fuentes primarias siempre que sea posible.

### 1. Objetivo de la investigación

Analiza qué alternativas de inversión existen actualmente en España y cuáles presentan una combinación atractiva de:

* rentabilidad esperada;
* riesgo;
* liquidez;
* fiscalidad;
* costes;
* protección del capital;
* diversificación;
* horizonte temporal;
* facilidad de acceso para un inversor particular.

No asumas de antemano que una determinada categoría es mejor que otra.

### 2. Alternativas que debes analizar

Como mínimo, estudia:

* depósitos bancarios;
* cuentas remuneradas;
* Letras del Tesoro;
* bonos del Estado español;
* bonos corporativos;
* fondos monetarios;
* fondos de renta fija;
* fondos indexados;
* ETFs;
* fondos de inversión tradicionales;
* acciones españolas;
* acciones internacionales;
* REITs/SOCIMIs;
* inversión inmobiliaria directa;
* crowdfunding inmobiliario, si es relevante;
* oro;
* criptomonedas;
* otras alternativas que consideres relevantes para un inversor particular en España.

Si alguna alternativa tiene características que hacen que no sea comparable directamente con las demás, explícalo.

### 3. Análisis de cada alternativa

Para cada categoría proporciona:

1. Qué es y cómo funciona.
2. Rentabilidad histórica relevante.
3. Rentabilidad esperada razonable, diferenciando claramente entre datos históricos, estimaciones y escenarios.
4. Nivel de riesgo.
5. Volatilidad cuando sea aplicable.
6. Riesgo de pérdida permanente de capital.
7. Liquidez.
8. Horizonte temporal recomendado.
9. Costes y comisiones.
10. Fiscalidad en España para una persona física.
11. Tratamiento de dividendos, intereses y plusvalías.
12. Posibles ventajas fiscales.
13. Riesgos regulatorios, de mercado, de crédito, divisa o contraparte.
14. Inversión mínima aproximada.
15. Facilidad de acceso desde España.
16. Ejemplos concretos de vehículos o productos disponibles actualmente.
17. En qué circunstancias tendría sentido utilizar esa alternativa.
18. En qué circunstancias podría ser una mala elección.

### 4. Fiscalidad española

Dedica una sección específica a la fiscalidad.

Analiza el tratamiento fiscal vigente en España, incluyendo cuando corresponda:

* IRPF;
* rentas del ahorro;
* intereses;
* dividendos;
* ganancias de capital;
* fondos de inversión;
* ETFs;
* acciones;
* bonos;
* Letras del Tesoro;
* inversiones inmobiliarias;
* criptomonedas;
* mecanismos de diferimiento fiscal;
* diferencias entre fondos de inversión y ETFs;
* retenciones;
* tributación de inversiones extranjeras;
* obligaciones informativas relevantes.

Distingue entre fiscalidad estatal y posibles diferencias autonómicas cuando sean relevantes.

No inventes tipos impositivos. Verifica los tipos vigentes actualmente mediante fuentes oficiales.

### 5. Contexto macroeconómico

Analiza el contexto actual de España, Europa y los mercados internacionales que pueda afectar a las decisiones de inversión:

* inflación;
* tipos de interés del BCE;
* rentabilidad de la deuda pública;
* crecimiento económico;
* desempleo;
* mercado inmobiliario;
* valoración de las bolsas;
* evolución del euro;
* perspectivas monetarias;
* riesgos geopolíticos;
* situación fiscal de España;
* principales riesgos macroeconómicos.

Distingue claramente entre **datos actuales**, **previsiones de organismos oficiales** y **opiniones de analistas**.

### 6. Comparación cuantitativa

Construye una tabla comparativa con las principales alternativas y, cuando sea posible, utiliza métricas cuantitativas como:

* rentabilidad esperada;
* volatilidad;
* liquidez;
* costes;
* fiscalidad;
* riesgo;
* horizonte recomendado;
* correlación con otras clases de activos;
* protección frente a inflación.

Cuando no exista una métrica objetiva, indícalo en lugar de inventar una puntuación.

### 7. Escenarios

Analiza cómo podrían comportarse las distintas inversiones bajo al menos estos escenarios:

**Escenario A:** tipos de interés altos y crecimiento económico moderado.

**Escenario B:** caída de tipos y recuperación económica.

**Escenario C:** recesión.

**Escenario D:** inflación persistentemente elevada.

**Escenario E:** crisis financiera o fuerte caída de los mercados.

Explica qué activos podrían beneficiarse o verse perjudicados en cada escenario y por qué.

### 8. Construcción de carteras

Después del análisis individual, plantea ejemplos de carteras hipotéticas para distintos perfiles:

* conservador;
* moderado;
* equilibrado;
* crecimiento;
* agresivo.

No quiero que presentes ninguna como universalmente "mejor". Explica qué objetivos y supuestos hacen que cada cartera tenga sentido.

Incluye ejemplos para horizontes de:

* 1–3 años;
* 5 años;
* 10+ años.

### 9. Inversor residente en España pero con acceso internacional

Analiza también si tiene sentido utilizar productos de inversión extranjeros desde España.

Compara, cuando corresponda:

* productos españoles;
* productos europeos;
* ETFs domiciliados en Irlanda/Luxemburgo;
* brokers españoles;
* brokers internacionales.

Considera fiscalidad, regulación, costes, protección del inversor, divisa y facilidad administrativa.

### 10. Fuentes

Prioriza fuentes primarias y de alta calidad:

* Banco de España;
* BCE;
* CNMV;
* Agencia Tributaria;
* Ministerio de Hacienda;
* Tesoro Público;
* INE;
* Eurostat;
* organismos europeos;
* documentos oficiales de fondos y ETFs;
* informes financieros de las entidades correspondientes.

Puedes utilizar medios financieros y estudios de bancos o gestoras para complementar el análisis, pero identifica claramente cuándo una afirmación procede de una fuente comercial o de una opinión de mercado.

**No utilices blogs genéricos como fuente principal cuando exista una fuente oficial disponible.**

Para cada dato importante y especialmente para datos actuales, proporciona la fuente y la fecha.

### 11. Control de calidad

Antes de elaborar las conclusiones:

* verifica que los datos sean actuales;
* comprueba las fechas de publicación;
* contrasta información importante con más de una fuente cuando sea posible;
* distingue hechos de previsiones;
* distingue rentabilidad histórica de rentabilidad esperada;
* identifica incertidumbres;
* no presentes predicciones como hechos;
* no selecciones productos simplemente porque hayan tenido un buen rendimiento reciente;
* señala posibles conflictos de interés de las fuentes;
* indica cuando un dato no esté disponible o sea difícil de estimar.

### 12. Resultado final

Quiero un informe estructurado de forma profesional:

1. **Resumen ejecutivo**
2. **Situación actual de los mercados**
3. **Análisis de cada clase de activo**
4. **Fiscalidad en España**
5. **Comparación cuantitativa**
6. **Análisis por escenarios**
7. **Carteras hipotéticas según perfil y horizonte**
8. **Productos y vehículos concretos disponibles actualmente**
9. **Principales riesgos**
10. **Conclusiones**

En las conclusiones no quiero simplemente una lista de "ganadores". Explica **qué alternativas son adecuadas para qué objetivos, perfiles de riesgo y horizontes temporales**, y cuáles son las principales razones a favor y en contra de cada una.

Toda la información debe estar referida a la situación **actual a fecha de la investigación**. Si existen datos que no pueden verificarse con suficiente precisión, dilo explícitamente.

```

# Glosario

* Guardrails (Guardarieles, Quitamiedos)
    * Protecciones de los modelos que agrega el fabricante para temas sensibles e ilegales
* Jailbreak
    * Usar tecnicas de prompting para burlar los guardarieles de los LLM 
