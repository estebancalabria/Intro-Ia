# Clase Cinco - 13 de Mayo del 2026

# Repaso

* Modelos de Lenguaje
  * Open Source
    * Hugging Face
      * El lugar donde se subian los modelos Open Source
      * Tiene spaces donde probar miles de modelos de IA
    * Ejecutar un modelo localmente
      * LMStudio
      * Ollama
  * Comparacion entre modelos de lenguaje
    * Arena.ai
* Prompt Engineering
  * Prompt =  Tarea + Contexto + Rol + Ejemplo + Formato + Tono
  * Tips
      * Modo dictado
  * Conteto = Prompt + Conversacion + Memoria + Conversaciones Pasadas + Herramientas
  * Patron Interaccion
    * Metodo Socratico
    * Prompt Chainning


# Prompt Engineering

## Contexto

* Agrupar por proyectos
  * Las conversaciones dentro del mismo proyecto tienen un contexto compartido
  * Los proyectos se pueden compartir hasta y personas
  * Esta bueno para trabajo en equipo

## Patron persona

* Solapa sin Rol
    * "Me duele la panza. Dame consejos que hacer."
* Solapa Con Rol
    * Actua como un experto en alimentacion natural y resposable.  Me duele la panza. Dame consejos que hacer.
* Solapa con una persona Especifica
  * Actua como si fueras Alberto Cormillot.   Me duele la panza. Dame consejos que hacer.
* Solapa con un panel de expertos
  * Quiero que armes un panel de expertos donde cada uno me de su vision.   Me duele la panza. Dame consejos que hacer. (un par parrafos para cada experto)

> Conversaciones en el proyecto
> https://chatgpt.com/g/g-p-6a04b4fb70008191b7deeecd6ae4ba19-promting-rol/project

### TIP

* Usar a la IA como experto en prompt engineering

```
Actua como un experto en prompt engineering. Dado este prompt "Me duele la panza. Dame consejos que hacer." queiro una version mejorada del mismo siguiendo todas las buenas practicas del prompt engineering. Devolver el prompt mejorado sin acotar nada mas.
```

* Me devuelve

```
Actúa como un médico clínico y especialista en gastroenterología con experiencia en orientación inicial para molestias digestivas comunes. Tu objetivo es brindar una guía clara, segura, práctica y responsable para una persona que dice: “Me duele la panza”.

Antes de dar recomendaciones, haz una breve evaluación inicial haciendo preguntas clave para entender mejor el problema, incluyendo:

* Ubicación del dolor.
* Intensidad del dolor (1 a 10).
* Desde cuándo comenzó.
* Tipo de dolor (punzante, cólico, ardor, presión, etc.).
* Síntomas asociados (náuseas, vómitos, diarrea, fiebre, gases, constipación, sangre, mareos, etc.).
* Qué comió o tomó recientemente.
* Antecedentes relevantes o medicación actual.

Luego:

1. Explica posibles causas comunes de manera simple y no alarmista.
2. Recomienda medidas prácticas y seguras que puedan ayudar en casa (alimentación, hidratación, descanso, qué evitar, etc.).
3. Indica claramente señales de alarma que requieren atención médica urgente.
4. Sugiere cuándo consultar con un profesional aunque no sea una urgencia.
5. Usa lenguaje claro, humano y tranquilizador, evitando tecnicismos innecesarios.
6. No inventes diagnósticos definitivos ni reemplaces una consulta médica real.
7. Organiza la respuesta con títulos y viñetas para que sea fácil de leer.
```

> [!NOTA]
> Cuando a la IA le decis que actue como "Experto en prompt engineering" lo primero que hace es aplicar el patron rol/persona

---

## 
