# Lab: Clasificación de mails con Few-Shot Prompting

**Curso:** MS Copilot para el desarrollo profesional
**Duración estimada:** 15-20 minutos
**Objetivo:** Usar la técnica de Few-Shot Prompting para clasificar mails reales con el conector de correo, y comparar el resultado contra un pedido de clasificación sin ejemplos (zero-shot).

---

## Contexto para el participante

Ya vimos cómo conectar Copilot a nuestro mail. En este lab vamos a usar esa conexión para algo muy práctico: pedirle a la IA que nos clasifique los mails según su prioridad. Vamos a comparar dos formas de pedirlo para ver si cambia la consistencia del resultado.

**Requisito:** tener el conector de mail (Gmail u Outlook) habilitado, como en el lab de conectores.

---

## Paso 1 — Clasificación sin ejemplos (Zero-Shot)

Abrí una conversación nueva en Copilot Chat con el conector de mail activo y usá este prompt:

```
Revisá mis últimos 10 mails sin leer. Clasificá cada uno en una de estas tres categorías: Urgente, Normal, Bajo.

Devolvé el resultado en una tabla con las columnas: Remitente, Asunto, Categoría.
```

**Consigna:** guardá el resultado. Fijate si podés explicar con claridad por qué la IA eligió cada categoría, o si el criterio te parece poco consistente entre mails parecidos.

---

## Paso 2 — Clasificación con ejemplos (Few-Shot)

En una conversación **nueva**, usá este prompt, que incluye ejemplos ya clasificados antes de pedirle la tarea:

```
Quiero que clasifiques mails según su prioridad, usando estas tres categorías: Urgente, Normal, Bajo.

Estos son ejemplos de cómo quiero que clasifiques:

Mail: "El sistema está caído y no podemos facturar" → Urgente
Mail: "¿Podrían mandarme el catálogo actualizado?" → Bajo
Mail: "Necesito el reporte del mes antes del viernes" → Normal
Mail: "Reclamo: el pedido llegó incompleto y el cliente está esperando respuesta" → Urgente
Mail: "Newsletter mensual de la industria" → Bajo

Ahora, siguiendo el mismo criterio de estos ejemplos, revisá mis últimos 10 mails sin leer y clasificalos.

Devolvé el resultado en una tabla con las columnas: Remitente, Asunto, Categoría.
```

**Consigna:** compará esta tabla con la del Paso 1. ¿Cambiaron algunas categorías? ¿El criterio te parece más alineado con cómo vos priorizarías esos mismos mails?

---

## Puesta en común

Completá esta comparación:

| | Paso 1 (Zero-Shot) | Paso 2 (Few-Shot) |
|---|---|---|
| ¿Coincide la clasificación con tu propio criterio? | | |
| ¿Hubo mails "ambiguos" que cambiaron de categoría entre los dos pasos? | | |
| ¿Cuál de las dos tablas usarías para priorizar tu día sin revisar cada mail manualmente? | | |

**Preguntas para discutir en grupo:**

1. ¿En qué otras tareas de tu trabajo diario tenés categorías con criterios "difíciles de explicar en una frase" (como distinguir un reclamo técnico de una simple consulta)? Esos son los casos donde más ayuda el few-shot.
2. Si tu criterio de prioridad cambiara con el tiempo (por ejemplo, un cliente nuevo que ahora es prioritario), ¿qué parte del prompt tendrías que actualizar?

---

## Variante avanzada (opcional)

Pedile a Copilot que, además de clasificar, te arme un resumen ejecutivo solo de los mails "Urgente", priorizados por orden sugerido de respuesta:

```
De los mails que clasificaste como Urgente, armame un resumen de una línea por cada uno y sugerime el orden en el que debería responderlos, explicando brevemente por qué.
```

---

## Ejercicio final (para llevarse)

Pensá otra tarea repetitiva de tu trabajo que hoy hacés "a criterio" (clasificar tickets, priorizar pedidos, ordenar solicitudes) y armá tu propia versión de este prompt con 3 a 5 ejemplos representativos de tu propio criterio. Probalo y traé el resultado a la próxima instancia de seguimiento del curso.
