# Chain of Thought: pensar antes de responder

## ¿Qué es este documento?

Esta es una guía conceptual sobre el patrón de prompting **Chain of Thought (CoT)** — de dónde viene, por qué funciona, cómo se relaciona con los modos de razonamiento que hoy traen incorporados varios modelos de IA, y cuándo realmente conviene usarlo.

## Objetivos

Al terminar de leer esta guía vas a poder:

- Explicar en tus propias palabras qué es Chain of Thought y en qué se diferencia de un prompt directo.
- Distinguir la técnica de prompting CoT del "modo de razonamiento" que ya traen incorporado algunos modelos (como el Razonamiento Profundo de Copilot).
- Identificar en qué tipo de tareas conviene aplicar CoT y en cuáles no aporta demasiado.
- Reconocer las limitaciones del patrón, para no confiar en él a ciegas.

---

## Un poco de historia

El término "Chain of Thought" aparece formalmente en enero de 2022, en un paper de investigadores de Google titulado *"Chain-of-Thought Prompting Elicits Reasoning in Large Language Models"* (Wei et al., 2022). La idea central era simple pero tuvo mucho impacto: en vez de pedirle al modelo una respuesta directa, se lo guiaba con ejemplos que mostraban el razonamiento intermedio paso a paso antes de llegar a la conclusión — algo parecido a cómo un profesor resuelve un problema en el pizarrón mostrando cada paso, en vez de escribir solo el resultado final.

Poco después, en el mismo año, otro grupo de investigadores (Kojima et al., 2022) descubrió algo todavía más práctico: no hacía falta dar ejemplos elaborados. Bastaba con agregar una frase simple al final del prompt — la famosa **"Let's think step by step"** ("pensemos paso a paso") — para que el modelo generara ese razonamiento intermedio por su cuenta. A esta variante se la conoce como **Zero-shot CoT**, y es la versión que más se usa hoy en el día a día, porque no requiere preparar ejemplos de antemano.

Desde entonces, CoT se convirtió en una de las técnicas de prompting más estudiadas y replicadas en la industria, y sentó las bases conceptuales de lo que después evolucionaría hacia los modelos de razonamiento que tenemos hoy.

---

## El patrón, explicado simple

La diferencia central es esta:

| | Prompt directo | Chain of Thought |
|---|---|---|
| Qué le pedís | La respuesta final | El razonamiento, y después la respuesta |
| Cómo procesa la tarea | Va directo a la conclusión más probable | Descompone el problema en pasos intermedios |
| Cuándo se nota más la diferencia | Preguntas simples y directas | Problemas con varias variables, cálculos, lógica o decisiones con trade-offs |

**Ejemplo mínimo:**

- *Prompt directo:* "¿Cuánto es 17% de 850?"
- *Prompt con CoT:* "¿Cuánto es 17% de 850? Pensá paso a paso antes de dar el resultado."

En preguntas tan simples como esta la diferencia puede ser mínima. Donde el patrón realmente se nota es en problemas con varios factores en juego — decisiones de negocio, comparaciones con trade-offs, o cualquier tarea donde el camino hacia la respuesta importa tanto como la respuesta misma.

**Una forma de pensarlo:** es similar a la distinción que popularizó el psicólogo Daniel Kahneman entre dos formas de pensar humano — el "pensamiento rápido" (intuitivo, automático, la primera respuesta que se te ocurre) y el "pensamiento lento" (deliberado, analítico, el que usás cuando te sentás a resolver algo con cuidado). Un prompt directo se parece más al pensamiento rápido; pedirle CoT al modelo lo empuja hacia el pensamiento lento.

---

## ¿Y el "modo de razonamiento" de los modelos actuales?

Acá es donde suele haber confusión, porque están relacionados pero **no son lo mismo**.

- **CoT como técnica de prompting** es algo que el usuario pide explícitamente, agregando una instrucción al prompt ("pensá paso a paso"). Funciona con cualquier modelo, incluso los más simples, porque es una instrucción externa.

- **Los modos de razonamiento incorporados** (como el "Razonamiento Profundo" de Copilot, o modelos entrenados específicamente para razonar) son otra cosa: son modelos que fueron **entrenados** para generar ese razonamiento paso a paso de manera automática, sin que nadie se lo pida. En vez de necesitar la frase mágica "pensá paso a paso", el comportamiento de "pensar antes de responder" ya viene incorporado en cómo el modelo procesa cualquier pregunta.

En otras palabras: los modelos de razonamiento son, en cierto sentido, la evolución natural de la idea de CoT — lo que antes había que pedir con una instrucción en el prompt, ahora algunos modelos lo hacen solos, como parte de su funcionamiento interno. Ese razonamiento interno a veces se muestra al usuario (como cuando ves el "pensamiento" del modelo antes de la respuesta final) y a veces queda oculto.

**Entonces, ¿sigue siendo útil pedir CoT explícitamente si ya existen estos modos?** Sí, por varias razones prácticas:

- No siempre vas a tener el modo de razonamiento activado o disponible (a veces por costo, por velocidad, o porque la herramienta que estás usando no lo ofrece).
- Pedirlo explícitamente te da más control sobre *qué* querés que el modelo analice paso a paso (por ejemplo, forzarlo a mirar costos, riesgos y tiempos por separado, en ese orden).
- Es una habilidad de prompting que funciona en cualquier escenario, con cualquier modelo, tengas o no acceso a un modo de razonamiento dedicado.

---

## Los límites del patrón (para no idealizarlo)

Vale la pena conocer esto para usar la técnica con criterio y no como una solución mágica:

- **El razonamiento que muestra el modelo no siempre refleja fielmente cómo "llegó" realmente a la respuesta.** Investigación reciente muestra que a veces el modelo genera una explicación paso a paso que suena coherente, pero que no necesariamente representa el proceso real detrás de la respuesta — puede ser una justificación posterior más que un registro fiel del razonamiento.
- **No siempre mejora el resultado.** Estudios recientes muestran que el beneficio de pedir CoT explícitamente varía mucho según la tarea y el modelo: en tareas simples, a veces no cambia nada, y en algunos casos incluso puede introducir más variabilidad en la respuesta.
- **Emerge mejor en modelos grandes.** La técnica funciona de forma más consistente en modelos con mucha capacidad; en modelos más chicos el efecto es menos confiable.

La conclusión práctica no es "no lo uses", sino: **tratalo como una herramienta que ayuda especialmente en tareas complejas y con varias variables, y seguí revisando la respuesta final con criterio propio — como con cualquier salida de la IA.**

---

## Para llevarte

- Chain of Thought = pedirle al modelo que razone paso a paso *dentro de una misma respuesta*, no confundir con la técnica de interacción/chaining (que es una conversación de varios turnos para juntar contexto).
- Es especialmente útil en decisiones con varias variables, cálculos y problemas de lógica — menos relevante en preguntas simples y directas.
- Los modos de razonamiento automático de los modelos actuales son, conceptualmente, una evolución entrenada de esta misma idea.
- No es una garantía de razonamiento perfecto: sigue siendo una herramienta a supervisar, no una caja negra infalible.

---

## Referencias

- Wei, J. et al. (2022). *Chain-of-Thought Prompting Elicits Reasoning in Large Language Models.* https://arxiv.org/abs/2201.11903
- Kojima, T. et al. (2022). *Large Language Models are Zero-Shot Reasoners.*
- Meincke, L. et al. (2025). *Prompting Science Report 2: The Decreasing Value of Chain of Thought in Prompting.* https://arxiv.org/abs/2506.07142
- Turpin, M. et al. (2023). *Language Models Don't Always Say What They Think.*
