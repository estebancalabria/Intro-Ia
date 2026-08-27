# Lab: Chain of Thought vs. Modo de Razonamiento Automático

**Curso:** MS Copilot para el desarrollo profesional — SMW Agro
**Duración estimada:** 15-20 minutos
**Objetivo:** Diferenciar la técnica de prompting Chain of Thought (CoT) del modo de razonamiento automático que ya traen algunos modelos, y entender cuándo conviene pedirlo explícitamente.

---

## Contexto para el participante

Ya vimos que cuando le pedimos algo a la IA en una sola instrucción, a veces salta directo a una conclusión sin sopesar bien todas las variables. En este lab vamos a comparar tres formas de hacer la misma pregunta y ver si cambia la calidad de la respuesta.

---

## Caso de uso

> Vamos a evaluar una decisión de negocio genérica: si conviene tercerizar un proceso operativo (por ejemplo, logística, soporte al cliente o administración) o mantenerlo interno.

---

## Paso 1 — Prompt directo, modelo normal

Abrí una conversación nueva en Copilot Chat (modo estándar, sin activar Razonamiento Profundo) y usá este prompt tal cual:

```
¿Nos conviene tercerizar el proceso de [elegí un proceso: logística / soporte al cliente / administración] o mantenerlo interno? Respondé directamente con tu recomendación.
```

**Consigna:** guardá la respuesta. Fijate si te da una recomendación clara pero con poca justificación, o si salta directo a una conclusión.

---

## Paso 2 — Prompt directo + Chain of Thought explícito

En una conversación **nueva** (para que no arrastre el contexto del paso anterior), usá este prompt:

```
¿Nos conviene tercerizar el proceso de [mismo proceso elegido] o mantenerlo interno?

Antes de responder, razoná paso a paso:
1. Compará costos actuales vs. costos tercerizados.
2. Analizá riesgos operativos de cada opción.
3. Evaluá el impacto en los tiempos de entrega o de respuesta.
4. Recién después de este análisis, dame la recomendación final con su justificación.
```

**Consigna:** compará esta respuesta con la del Paso 1. ¿Cambió la profundidad del análisis? ¿La recomendación final es la misma?

---

## Paso 3 — Mismo prompt directo, con Razonamiento Profundo activado

En una conversación nueva, activá el modo **Razonamiento Profundo** de Copilot y usá el mismo prompt simple del Paso 1 (sin pedir nada extra):

```
¿Nos conviene tercerizar el proceso de [mismo proceso elegido] o mantenerlo interno? Respondé directamente con tu recomendación.
```

**Consigna:** observá si el modelo igual desarrolla un razonamiento antes de la conclusión, aunque no se lo pediste explícitamente como en el Paso 2.

---

## Puesta en común

Completá esta tabla comparando las tres respuestas:

| | Paso 1 (directo) | Paso 2 (CoT explícito) | Paso 3 (Razonamiento Profundo) |
|---|---|---|---|
| ¿Explica el razonamiento antes de concluir? | | | |
| ¿Considera costos, riesgos y tiempos por separado? | | | |
| ¿La recomendación final es la misma en los tres casos? | | | |
| ¿Cuál te genera más confianza para tomar la decisión? | | | |

**Preguntas para discutir en grupo:**

1. ¿En qué escenarios de tu trabajo diario un prompt directo alcanza, y en cuáles conviene forzar el razonamiento paso a paso?
2. ¿Vale la pena pedir CoT explícito incluso cuando tenés el modo Razonamiento Profundo disponible? ¿Por qué?

---

## Ejercicio final (para llevarse)

Elegí una decisión real de tu trabajo (elegir proveedor, priorizar tareas, evaluar una inversión, etc.) y repetí el mismo ejercicio de tres pasos con tu propio caso. Traé la comparación a la próxima instancia de seguimiento del curso.
