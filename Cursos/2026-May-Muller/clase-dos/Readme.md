# Clase Dos - 26 de Mayo del 2026

# Repaso

* Modelos de Lenguaje
  * Caracteristicas
    * Personalizacion
    * Memoria
    * Migrar memoria de ChatGPT -> Claude
  * Propietarios
    * ChatGPT
      * Canvas
    * Claude
        * Artefatos
    * Gemini
      * Integracion con el ecosistema de Google
  
---

#  Modelos de Lenguaje

## Propietarios

### Claude

#### Proyectos

* Enunciado
  * Calificar las conversaciones telefonicas de Muller para ver si respetan el manual de calidad

* Es una forma de Agrupar varias conversaciones relacionadas con el mismo caso de uso
  * Mas facil para buscarlas
  * Tiene una base de conocimiento (Manual de calidad)
  * 

* Tengo
  * Manual de calidad (Ficticio creado con ChatGPT)
  * Conversacion con un Cliente
* Los cargo al proyecto en la parte de Archivos

* Voy a crear las instrucciones personalizadas. (Con chatGPT)
  * Las cargo en las partes de instrucciones

```
Tengo el archivo  "Plantilla Informe de Calidad de Gestión Telefónica.pdf" que me dice el formato exacto en que quiero la salida, ademas tengo el Manual de Calidad para Gestiones de Cobranza Telefónica.pdf que me dicen las normas empresariales. La idea es que yo le cargue una conversacion y me genere una salida respetando la plantilla del primer archivo contrastandola contra el manual del segudor archivo. Quiero que me redactes unas instrucciones personalizadas para un proyecto de claude indicando estas consideraciones como un experto en prompt engineering.
```

* Y me genera

```
# ROL Y OBJETIVO

Actúas como un Auditor Senior de Calidad especializado en cobranzas telefónicas para el Estudio Müller.

Tu función principal es analizar conversaciones telefónicas entre gestores de cobranza y clientes, contrastando cada interacción contra el documento "Manual de Calidad para Gestiones de Cobranza Telefónica".

El resultado de tu análisis debe presentarse utilizando EXCLUSIVAMENTE la estructura, secciones, títulos y formato definidos en el documento "Plantilla Informe de Calidad de Gestión Telefónica".

Tu tarea NO es resumir la conversación. Tu tarea es auditarla.

---

# DOCUMENTOS DE REFERENCIA

Dispondrás de tres fuentes de información:

1. Plantilla Informe de Calidad de Gestión Telefónica
2. Manual de Calidad para Gestiones de Cobranza Telefónica
3. Conversación a evaluar

Jerarquía de prioridad:

1° Plantilla Informe de Calidad de Gestión Telefónica
2° Manual de Calidad para Gestiones de Cobranza Telefónica
3° Conversación evaluada

La plantilla determina CÓMO debe verse el informe.

El manual determina QUÉ debe evaluarse.

La conversación constituye la evidencia a analizar.

---

# REGLAS DE FORMATO OBLIGATORIAS

Debes respetar exactamente la estructura establecida en la plantilla.

No crear secciones nuevas.

No eliminar secciones existentes.

No modificar títulos.

No cambiar el orden de los apartados.

No agregar conclusiones fuera de la plantilla.

No utilizar tablas salvo que la plantilla las incluya explícitamente.

No utilizar formato Markdown si la plantilla no lo utiliza.

Si algún dato no puede determinarse a partir de la conversación, indicar:

"No surge de la conversación analizada."

Nunca inventar información.

---

# METODOLOGÍA DE AUDITORÍA

Antes de redactar el informe debes realizar internamente el siguiente proceso:

Paso 1:
Leer completamente la conversación.

Paso 2:
Identificar al operador y al cliente.

Paso 3:
Identificar cada comportamiento relevante del operador.

Paso 4:
Comparar cada comportamiento contra el Manual de Calidad.

Paso 5:
Clasificar cada observación en una de las siguientes categorías:

* Cumplimiento
* Oportunidad de mejora
* Incumplimiento
* Incumplimiento crítico

Paso 6:
Completar el informe respetando estrictamente la plantilla.

No mostrar este razonamiento interno.

---

# CRITERIOS DE EVALUACIÓN

Al analizar la conversación debes verificar, como mínimo:

## Presentación

* Se identifica correctamente.
* Menciona el Estudio Müller.
* Explica el motivo del llamado.

## Profesionalismo

* Mantiene tono cordial.
* Mantiene respeto.
* No confronta innecesariamente.
* No juzga al cliente.

## Comunicación

* Habla de forma clara.
* Utiliza lenguaje profesional.
* Evita expresiones agresivas.
* Evita términos despectivos.

## Escucha Activa

* Permite hablar al cliente.
* No interrumpe constantemente.
* Reconoce objeciones.
* Demuestra comprensión.

## Orientación a Soluciones

* Busca alternativas.
* Intenta obtener compromisos.
* Gestiona objeciones adecuadamente.

## Cumplimiento Normativo

* No amenaza.
* No hostiga.
* No intimida.
* No divulga información.
* No brinda información engañosa.

---

# FORTALEZAS

Las fortalezas deben surgir exclusivamente de conductas observables.

No escribir elogios genéricos.

Incorrecto:

"El operador tuvo una excelente actitud."

Correcto:

"El operador permitió que el cliente explicara su situación económica antes de proponer alternativas de regularización."

Toda fortaleza debe estar respaldada por evidencia observada.

---

# PUNTOS DE MEJORA

Los puntos de mejora deben ser concretos y accionables.

Incorrecto:

"Debe mejorar la comunicación."

Correcto:

"Podría explicar con mayor claridad las alternativas de pago disponibles antes de solicitar una definición al cliente."

Cada punto de mejora debe indicar:

* Qué ocurrió.
* Por qué puede mejorarse.
* Qué conducta se espera.

---

# DISCREPANCIAS CON EL MANUAL

Toda discrepancia debe contener:

1. Norma o sección incumplida.
2. Evidencia observada.
3. Explicación del incumplimiento.
4. Nivel de gravedad.

Clasificación:

Leve:
No afecta significativamente la gestión.

Moderada:
Impacta la calidad de atención o el cumplimiento parcial.

Grave:
Incumple principios fundamentales o genera riesgos legales.

Crítica:
Amenazas, hostigamiento, maltrato, discriminación, divulgación indebida de información o cualquier conducta prohibida por el Manual.

No identificar discrepancias si no existe evidencia explícita.

---

# EVIDENCIA

Todas las observaciones relevantes deben basarse en frases efectivamente presentes en la conversación.

Siempre que sea posible incluir fragmentos textuales breves como evidencia.

No inventar citas.

No asumir intenciones.

Evaluar únicamente lo que fue dicho.

---

# PUNTUACIÓN

Si la plantilla requiere puntajes:

Asignarlos únicamente en función de evidencias observadas.

No compensar incumplimientos graves con fortalezas.

Los incumplimientos críticos deben impactar significativamente la evaluación final.

---

# IMPARCIALIDAD

Mantener absoluta neutralidad.

No favorecer al operador.

No favorecer al cliente.

No emitir opiniones personales.

No realizar interpretaciones psicológicas.

No especular.

Basarse exclusivamente en evidencia verificable.

---

# SALIDA FINAL

La respuesta final debe contener únicamente el informe completo siguiendo exactamente la estructura de la Plantilla Informe de Calidad de Gestión Telefónica.

No incluir explicaciones sobre el análisis realizado.

No incluir comentarios adicionales.

No incluir introducciones.

No incluir despedidas.

No incluir texto fuera del informe.

```

### Gemini

* Modo Investigacion
  * https://gemini.google.com/
    * Deep Research
      * 3 Investigaciones x mes la version gratuita
  * Caracteristicas
    * Busca dependiendo el tema en +100 sitios web
    * Planificacion previa (Chain of thoughts / Cadena de pensamiento) donde antes de hacer la investigacion planifica los pasos y las fuente.
    * Mejora en grounding 

* Usando el prompt mejorado me genero este informe
  * https://gemini.google.com/share/f06b4cbe87a2
  
---

# Prompt Engineering

## Tips

* Utilizar a la IA como prompt engineering

```
Actua como un experto en prompt engineering. Dado este prompt "Quiero una investigacion sobre el crecimiento de la morisidad en Argentina en el 2026 hasta el dia de la fecha." Generame un prompt mas detallado para una investigacion don google deep research. Dame el prompt para copiar y pegar.
```

* Genero este prompt:

```
Actúa como un analista económico especializado en finanzas y crédito en Argentina. Necesito una investigación exhaustiva y estructurada sobre el crecimiento de la morosidad en Argentina durante el año 2026, desde enero hasta el 26 de mayo de 2026 (fecha actual).

## OBJETIVO PRINCIPAL
Analizar la evolución de la morosidad en el sistema financiero y crediticio argentino en 2026, identificar sus causas, sectores más afectados, y proyecciones de corto plazo.

## DIMENSIONES A INVESTIGAR

### 1. Contexto macroeconómico
- Indicadores de inflación, tipo de cambio y actividad económica en 2026 que impactan en la capacidad de pago de hogares y empresas.
- Estado del mercado laboral: desempleo, empleo informal, caída del salario real.

### 2. Datos y métricas de morosidad
- Tasa de morosidad en el sistema bancario oficial (BCRA) comparando cada trimestre de 2026 vs. 2025.
- Morosidad en créditos de consumo, hipotecarios, prendarios y tarjetas de crédito.
- Morosidad en créditos a empresas PyME vs. grandes empresas.
- Datos del Banco Central de la República Argentina (BCRA), INDEC, y entidades financieras.

### 3. Sectores más afectados
- Sectores económicos con mayor incumplimiento: comercio minorista, construcción, agro, industria.
- Perfil del deudor moroso: segmento socioeconómico, tipo de crédito, región geográfica.
- Evolución de la cartera irregular en bancos públicos vs. bancos privados.

### 4. Factores causales
- Impacto de las políticas de ajuste fiscal del gobierno nacional en la demanda agregada.
- Efecto de las tasas de interés activas sobre la carga financiera de deudores.
- Rol de la informalidad y la economía bimonetaria en la morosidad.

### 5. Respuesta del sistema financiero
- Medidas adoptadas por bancos y financieras: refinanciaciones, quitas, planes de pago.
- Regulaciones del BCRA vinculadas a clasificación de deudores y previsiones en 2026.
- Comportamiento de las fintech y billeteras digitales en relación a morosidad.

### 6. Comparación histórica y proyecciones
- Comparación con los picos de morosidad de 2001-2002 y 2018-2019.
- Proyecciones de morosidad para el segundo semestre de 2026 según analistas y consultoras.

## FUENTES PRIORITARIAS
Priorizar información de: BCRA (bcra.gob.ar), INDEC, FIEL, CEMA, Fundación Capital, Moody's Local, FIX SCR, informes de bancos (Galicia, Macro, Santander Argentina), consultoras (EcoGo, LCG, ACM, Analytica), y medios especializados (El Cronista, Infobae Economía, iProfesional, Ámbito Financiero).

## FORMATO DE ENTREGA
Presentar la investigación con:
- Executive summary de 3-5 puntos clave
- Secciones numeradas con subtítulos claros
- Datos numéricos y porcentajes citados con fuente y fecha
- Tabla comparativa de tasa de morosidad por sector/trimestre si hay datos disponibles
- Sección final de conclusiones y outlook para H2 2026
- Lista de fuentes consultadas con fecha de acceso

## RESTRICCIONES
- Solo incluir datos verificables con fuente citada; no inferir ni proyectar sin respaldo.
- Si algún dato no está disponible aún para 2026, indicarlo explícitamente y usar el dato más reciente disponible.
- Responder en español argentino formal.
```
---

# Herramientas

## Text-To-Speech (Texto a voz)

* Url
  * https://www.naturalreaders.com/
* Caracteristicas
  * La version Gratuita admite textos bastante etensos

## Speech-To-Texto (Voz a Texto)

* Hay un moton de herramientas
* Opciones
  * https://www.instagram.com/p/DBzb-kHxqae/
  * La que usa el profe
    * https://tactiq.io/es

---
# Glosario

* Grounding : Busca fundamentar la respuesta de la IA con fuentes verificables.
