# Guía Avanzada de Prompting: Del Enfoque Zero-Shot al Aprendizaje en Contexto con Few-Shot

## 1. El Comportamiento del Modelo ante Solicitudes Directas (Zero-Shot)

Cuando un modelo de lenguaje amplio (LLM) procesa una instrucción en modalidad **Zero-Shot**, la generación de la respuesta depende de los pesos paramétricos acumulados durante su fase de preentrenamiento y su posterior alineación mediante aprendizaje por refuerzo con retroalimentación humana (RLHF).

En este enfoque, el usuario provee una consigna o un contexto operativo directo sin incluir ejemplos explícitos de la salida esperada.

```
[Prompt Zero-Shot]
┌────────────────────────────────────────────────────────┐
│ - Rol y Contexto                                       │
│ - Instrucción de la tarea                              │
│ - Datos de entrada (Input)                             │
└────────────────────────────────────────────────────────┘
                           │
                           ▼
              ┌────────────────────────┐
              │  Distribución general  │
              │  de probabilidades     │
              └────────────────────────┘
                           │
                           ▼
              ┌────────────────────────┐
              │ Output con alta        │
              │ variabilidad potencial │
              └────────────────────────┘

```

### Límites del Enfoque Zero-Shot en Entornos Corporativos

El comportamiento del modelo en Zero-Shot presenta dos limitaciones operativas principales:

* **Incertidumbre en el Formato de Salida:** Aunque la instrucción incluya restricciones de estilo o estructura, el modelo calcula la probabilidad del siguiente token basándose en patrones generales de internet. Esto provoca que ante entradas similares el formato final varíe entre ejecuciones (por ejemplo, omitiendo encabezados, cambiando la nomenclatura o alterando la jerarquía de la información).
* **Interpretación de Criterios Subjetivos:** Conceptos como "resumen ejecutivo", "criticidad alta" o "análisis detallado" carecen de una definición única. En Zero-Shot, el modelo asigna una interpretación promediada de lo que esos términos significan en su corpus de entrenamiento, lo cual suele diferir de los estándares, normativas o estilos de redacción específicos de una organización.

---

## 2. In-Context Learning y la Dinámica del Few-Shot

El paradigma **Few-Shot** modifica la forma en que el modelo procesa la instrucción mediante el concepto de *In-Context Learning* (aprendizaje en contexto). En lugar de modificar los pesos internos de la red neuronal mediante un reentrenamiento (Fine-Tuning), se condiciona la atención del Transformer incorporando dentro de la misma ventana de contexto una serie de pares ordenados de entrada y salida (`Input` $\rightarrow$ `Output`).

```
[Prompt Few-Shot]
┌────────────────────────────────────────────────────────┐
│ - Rol y Contexto                                       │
│ - Reglas y Taxonomía                                   │
│                                                        │
│  [Ejemplo 1] Input A  ──>  Output A (Ideal)            │
│  [Ejemplo 2] Input B  ──>  Output B (Ideal)            │
│                                                        │
│ - Datos de entrada reales (Input C)                    │
└────────────────────────────────────────────────────────┘
                           │
                           ▼
              ┌────────────────────────┐
              │ Reducción del espacio  │
              │ de búsqueda (Atención) │
              └────────────────────────┘
                           │
                           ▼
              ┌────────────────────────┐
              │ Output estructurado,   │
              │ consistente y alineado │
              └────────────────────────┘

```

### Mecanismos Internos del Few-Shot Prompting

Al incluir ejemplos representativos en la secuencia de entrada, se activan los siguientes mecanismos de resolución:

1. **Alineación por Atención Cruzada:** Las capas de atención del modelo comparan los tokens de los datos de entrada reales con los tokens de los ejemplos provistos. Esto permite replicar de forma explícita la estructura sintáctica, la longitud y la profundidad conceptual demostradas en las salidas de referencia.
2. **Restricción del Espacio de Búsqueda:** Los ejemplos actúan como un filtro que reduce la entropía en la selección de tokens. Al limitar las opciones probabilísticas del modelo a aquellas que concuerdan con el patrón presentado, se mitiga el riesgo de variaciones imprevistas y se minimizan las desviaciones en el formato.
3. **Calibración de Estándares Internos:** El modelo utiliza las demostraciones para deducir las reglas de negocio implícitas. Por ejemplo, al observar qué tipo de problemas fueron clasificados como "Críticos" en los ejemplos previos, ajusta la evaluación del nuevo caso según ese mismo rasgo sin necesidad de detallar cada regla en la instrucción.

---

## 3. Matriz de Análisis Técnico y Criterios de Selección

La elección entre utilizar un enfoque Zero-Shot o estructurar un prompt Few-Shot depende de los requerimientos de la tarea, la estabilidad requerida en la salida y las restricciones del sistema.

| Dimensión de Análisis | Enfoque Zero-Shot | Enfoque Few-Shot |
| --- | --- | --- |
| **Mecanismo de Inferencia** | Invocación directa del conocimiento paramétrico base del modelo. | Anclaje dinámico de la atención a través de demostraciones en contexto. |
| **Previsibilidad de la Estructura** | Variable. El formato final puede alterarse ante cambios menores en el texto de entrada. | Alta. El modelo imita la sintaxis, el orden de las variables y el estilo del bloque de ejemplo. |
| **Consumo de Ventana de Contexto** | Bajo. Solo requiere el texto de la consigna y la información a procesar. | Elevado. Los pares de ejemplo consumen una porción considerable de la cuota de tokens. |
| **Sensibilidad a la Redacción** | Alta. Pequeñas modificaciones en la adjetivación del prompt pueden alterar significativamente el resultado. | Baja. El peso compositivo de los ejemplos predomina sobre las variaciones léxicas de la directiva. |
| **Aplicación Recomendada** | Redacción abierta, ideación, resúmenes no estructurados, traducción general y consultas exploratorias. | Procesamiento estructurado de datos, integración con APIs (JSON/CSV), auditorías normativas y tareas corporativas estandarizadas. |
