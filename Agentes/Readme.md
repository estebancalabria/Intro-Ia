# 🤖 Agentes de Inteligencia Artificial

Hasta ahora gran parte de nuestra interacción con la Inteligencia Artificial estuvo basada en una idea muy simple:

**Usuario → Prompt → Modelo → Respuesta**

Le hacemos una pregunta a un modelo como GPT, Claude o Gemini y obtenemos una respuesta.

Pero ¿qué pasa si además de responder permitimos que la IA pueda **hacer cosas**?

Por ejemplo:

- buscar información en Internet;
- consultar nuestros correos;
- revisar nuestro calendario;
- buscar información en documentos;
- consultar una base de datos;
- crear una tarea;
- generar un archivo;
- ejecutar código;
- interactuar con una API;
- modificar un proyecto de software.

Ahí empezamos a entrar en el mundo de los **agentes de Inteligencia Artificial**.

---

## 🧠 De un LLM a un agente

Un **Large Language Model (LLM)** recibe información y genera una respuesta.

Por ejemplo:

> Explicame qué es Machine Learning.

El modelo procesa nuestra solicitud y genera una respuesta.

Pero supongamos que preguntamos:

> ¿Qué reuniones tengo mañana?

El modelo no puede conocer nuestro calendario simplemente por haber sido entrenado con grandes cantidades de información.

Necesita acceder a nuestro calendario.

Para hacerlo necesita una **herramienta**.

El flujo empieza a cambiar:

**Usuario → Modelo → Herramienta → Calendario → Modelo → Respuesta**

Ahora el modelo no solamente está generando texto.

Está utilizando una herramienta para **interactuar con un sistema externo**.

Esta capacidad es una de las bases de los sistemas agénticos.

---

# 🤖 ¿Qué es un agente de IA?

Un **agente de Inteligencia Artificial** es un sistema que utiliza un modelo de IA junto con instrucciones, contexto y herramientas para intentar alcanzar un determinado objetivo.

Podemos simplificarlo así:

**Modelo + Instrucciones + Contexto + Herramientas + Acciones = Sistema agéntico**

Un agente puede:

1. recibir un objetivo;
2. analizar qué necesita hacer;
3. seleccionar una herramienta;
4. realizar una acción;
5. observar el resultado;
6. utilizar ese resultado para decidir qué hacer después.

No todos los agentes necesitan realizar todos estos pasos ni tener un alto grado de autonomía.

Existen agentes muy simples y agentes capaces de ejecutar procesos mucho más complejos.

---

# 🧩 Componentes de un agente

Aunque existen muchas arquitecturas diferentes, podemos identificar algunos componentes habituales.

## 🧠 Modelo

Es el modelo que permite interpretar lenguaje, analizar información, generar contenido y tomar decisiones.

Por ejemplo:

- GPT;
- Claude;
- Gemini;
- modelos open source.

El modelo es el componente que aporta las capacidades de razonamiento y generación, pero **el modelo por sí solo no constituye necesariamente un agente**.

---

## 📋 Instrucciones

Las instrucciones establecen cómo debe comportarse el agente.

Pueden definir:

- su objetivo;
- su función;
- reglas de comportamiento;
- restricciones;
- procedimientos que debe seguir;
- acciones que puede o no puede realizar.

Por ejemplo, podríamos crear un agente especializado en soporte técnico y darle instrucciones como:

> Ayudá al usuario a diagnosticar problemas técnicos. Antes de proponer una solución, consultá la documentación disponible y solicitá confirmación antes de realizar cualquier cambio.

---

## 🌐 Contexto

El agente necesita información para poder trabajar correctamente.

El contexto puede provenir de:

- la conversación actual;
- conversaciones anteriores;
- documentos;
- bases de conocimiento;
- información del usuario;
- aplicaciones empresariales;
- resultados obtenidos mediante herramientas.

Un buen agente no depende solamente de un buen prompt.

También depende de tener disponible el **contexto correcto en el momento correcto**.

---

# 🛠️ Tools

Uno de los componentes más importantes son las **Tools o herramientas**.

Las herramientas permiten que el agente interactúe con sistemas que se encuentran fuera del modelo.

Por ejemplo, podemos darle herramientas para:

- buscar en Internet;
- consultar Outlook;
- acceder a un calendario;
- buscar documentos;
- consultar SharePoint;
- consultar una base de datos SQL;
- ejecutar Python;
- utilizar GitHub;
- interactuar con un CRM;
- utilizar una API.

El modelo interpreta lo que quiere conseguir el usuario y puede determinar qué herramienta necesita utilizar.

---

# 🔎 Un ejemplo sencillo

Supongamos que preguntamos:

> ¿Tengo tiempo mañana a las 15:00 para una reunión?

Un modelo sin acceso a herramientas no puede conocer nuestro calendario.

Un agente con acceso al calendario podría:

1. interpretar nuestra solicitud;
2. seleccionar la herramienta de calendario;
3. consultar los eventos de mañana;
4. analizar el resultado;
5. responder si estamos disponibles.

La herramienta amplía lo que el modelo puede hacer.

---

# 🔄 Un agente también puede trabajar en varios pasos

Algunas tareas necesitan una única acción.

Otras pueden requerir varias.

Por ejemplo:

> Preparame para las reuniones que tengo mañana.

Un agente podría necesitar:

1. consultar nuestro calendario;
2. identificar las reuniones;
3. buscar correos relacionados;
4. buscar documentos relacionados;
5. consultar reuniones anteriores;
6. organizar la información;
7. generar un resumen para cada reunión.

En este caso el agente está combinando diferentes fuentes y herramientas para alcanzar un objetivo más amplio.

---

# 🔁 El ciclo de un agente

En tareas más complejas puede aparecer un ciclo similar al siguiente:

**Objetivo → Analizar → Actuar → Observar → Decidir → Continuar**

Por ejemplo:

> Investigá este tema y preparame un informe.

El proceso podría ser:

### 1. Objetivo

El usuario define qué necesita.

### 2. Análisis

El agente determina qué información necesita obtener.

### 3. Acción

Utiliza una herramienta de búsqueda.

### 4. Observación

Recibe y analiza los resultados.

### 5. Decisión

Determina que necesita información adicional.

### 6. Nueva acción

Consulta otra fuente.

### 7. Resultado

Integra la información obtenida y genera el informe.

Este ciclo puede repetirse hasta alcanzar el objetivo o hasta necesitar intervención del usuario.

---

# 🌎 ¿Para qué podemos utilizar agentes?

Los agentes no pertenecen exclusivamente al desarrollo de software.

Pueden utilizarse prácticamente en cualquier escenario donde una IA necesite interactuar con información, herramientas o sistemas.

---

## 📅 Productividad

Un agente podría:

- consultar nuestro calendario;
- encontrar horarios disponibles;
- organizar reuniones;
- consultar documentos;
- recuperar información de reuniones anteriores;
- identificar tareas pendientes.

---

## 📧 Comunicación

Un agente podría:

- buscar correos;
- resumir conversaciones;
- generar respuestas;
- clasificar mensajes;
- buscar información relacionada antes de responder;
- enviar mensajes cuando tenga los permisos necesarios.

---

## 🔎 Investigación

Un agente podría:

- realizar búsquedas;
- consultar diferentes fuentes;
- comparar información;
- profundizar en determinados resultados;
- sintetizar información;
- preparar un informe.

---

## 📊 Análisis de datos

Un agente podría:

- consultar una base de datos;
- ejecutar consultas;
- analizar datasets;
- utilizar Python;
- calcular estadísticas;
- detectar patrones;
- generar visualizaciones;
- elaborar reportes.

---

## 🏢 Procesos empresariales

Un agente podría interactuar con:

- CRM;
- ERP;
- bases de datos;
- sistemas de tickets;
- herramientas de gestión de proyectos;
- bases de conocimiento;
- plataformas empresariales.

Por ejemplo:

> Buscá los clientes que tienen oportunidades abiertas, identificá cuáles no tuvieron actividad durante los últimos 30 días y preparame un resumen.

Para resolverlo podría consultar diferentes sistemas y combinar sus resultados.

---

## 💻 Desarrollo de software

Otro escenario posible es utilizar agentes para trabajar con proyectos de software.

Estos agentes pueden:

- explorar un repositorio;
- leer archivos;
- crear archivos;
- modificar código;
- ejecutar comandos;
- ejecutar tests;
- analizar errores;
- utilizar Git;
- interactuar con GitHub.

Este tipo particular de agente suele denominarse **Coding Agent**.

---

# 💻 Coding Agents

Los **Coding Agents** son agentes especializados en tareas relacionadas con el desarrollo de software.

Algunos ejemplos son:

| Ecosistema | Coding Agent |
|---|---|
| OpenAI | Codex |
| Anthropic | Claude Code |
| Google | Gemini CLI |
| GitHub | GitHub Copilot CLI |

Estos agentes suelen tener acceso a herramientas relacionadas con el entorno de desarrollo:

- sistema de archivos;
- terminal;
- Git;
- GitHub;
- compiladores;
- intérpretes;
- package managers;
- frameworks de testing;
- linters.

Por ejemplo, podemos pedir:

> Analizá este proyecto y explicame cómo está organizado.

Pero también podemos establecer un objetivo:

> Agregá validación al formulario de registro y verificá que los tests sigan funcionando.

El agente podría explorar el proyecto, modificar los archivos necesarios, ejecutar los tests, observar un error, corregirlo y volver a ejecutar los tests.

Es un ejemplo muy claro de comportamiento agéntico.

Pero los **Coding Agents son solamente un tipo de agente**.

---

# 🎯 Agentes especializados

Podemos crear agentes especializados en diferentes funciones.

Por ejemplo:

### 🔎 Agente de investigación

Herramientas:

- búsqueda web;
- documentación;
- bases de conocimiento.

### 📊 Agente de datos

Herramientas:

- SQL;
- Python;
- bases de datos;
- herramientas de visualización.

### 📧 Agente de productividad

Herramientas:

- correo;
- calendario;
- documentos;
- tareas.

### 💼 Agente de ventas

Herramientas:

- CRM;
- correo electrónico;
- información de clientes;
- sistemas empresariales.

### 🛠️ Agente de soporte

Herramientas:

- documentación;
- bases de conocimiento;
- sistemas de tickets;
- información de dispositivos.

### 💻 Agente de programación

Herramientas:

- archivos;
- terminal;
- Git;
- GitHub;
- testing.

Muchas veces la especialización de un agente no está determinada solamente por el modelo que utiliza.

Está determinada principalmente por la combinación de:

**Modelo + Instrucciones + Contexto + Herramientas**

---

# 👥 Sistemas Multiagente

No necesariamente tenemos que trabajar con un único agente.

También podemos construir sistemas que utilizan **varios agentes especializados**.

Por ejemplo, imaginemos que queremos generar un informe utilizando diferentes fuentes de información.

Podríamos tener:

### Agente de investigación

Busca y recupera información.

↓

### Agente de análisis

Analiza y compara los datos encontrados.

↓

### Agente de redacción

Genera el informe final.

Cada agente puede tener:

- instrucciones diferentes;
- herramientas diferentes;
- contexto diferente;
- responsabilidades diferentes.

También puede existir un agente encargado de **coordinar el trabajo de otros agentes**.

A esto se lo suele denominar **sistema multiagente o Multi-Agent System**.

---

# 👤 Human in the Loop

No todas las decisiones deberían ejecutarse automáticamente.

En muchos escenarios es importante que exista intervención humana.

Por ejemplo, un agente podría recibir:

> Analizá este correo y prepará una respuesta.

El agente puede:

1. leer el correo;
2. consultar información adicional;
3. generar una respuesta.

Pero antes de enviarla podría solicitar autorización:

> La respuesta está preparada. ¿Querés que la envíe?

Este enfoque se conoce como **Human in the Loop**.

El humano continúa participando en determinadas decisiones, especialmente cuando una acción puede tener consecuencias importantes.

---

# 🔐 Autonomía, herramientas y permisos

No todos los agentes necesitan el mismo nivel de autonomía.

Podemos tener un agente que solamente pueda:

**leer información**

Otro puede:

**leer + crear información**

Otro:

**leer + crear + modificar**

Y otro podría incluso:

**leer + crear + modificar + eliminar + ejecutar acciones**

Por eso existe una relación directa entre:

**Autonomía ↔ Herramientas ↔ Permisos ↔ Riesgo**

Cuanto mayores sean las capacidades del agente, más importante será controlar:

- qué herramientas puede utilizar;
- a qué información puede acceder;
- qué acciones puede realizar;
- cuáles requieren autorización humana.

Un principio importante es otorgar al agente **solamente las herramientas y permisos necesarios para realizar su función**.

---

# 🧠 ¿Un agente tiene que ser completamente autónomo?

No.

Este es un punto importante.

Un sistema no necesita trabajar durante horas, crear grandes planes o tomar todas las decisiones independientemente para utilizar conceptos agénticos.

Puede existir un agente muy simple que:

1. interpreta una solicitud;
2. selecciona una herramienta;
3. ejecuta una acción;
4. devuelve el resultado.

También podemos construir sistemas más sofisticados capaces de:

- crear planes;
- ejecutar múltiples pasos;
- revisar sus resultados;
- utilizar diferentes herramientas;
- delegar tareas;
- pedir aprobación;
- continuar trabajando según los resultados obtenidos.

Por lo tanto, **la capacidad agéntica puede existir en diferentes grados**.

---

# 🚀 Del chatbot al agente

Podemos observar una evolución interesante.

## Chatbot tradicional

**Usuario → Pregunta → Respuesta**

El sistema conversa.

---

## LLM

**Usuario → Prompt → Modelo → Respuesta generada**

El modelo comprende y genera lenguaje.

---

## LLM con herramientas

**Usuario → Modelo → Tool → Resultado → Modelo**

El modelo puede acceder a capacidades externas.

---

## Agente

**Usuario → Objetivo → Modelo → Herramientas → Acciones → Observaciones → Decisiones → Resultado**

La IA puede utilizar esas capacidades para avanzar hacia un objetivo.

---

# 🎯 Idea principal

La evolución hacia agentes representa un cambio importante en nuestra relación con la Inteligencia Artificial.

Pasamos de sistemas que principalmente:

> **generan respuestas**

a sistemas que además pueden:

> **utilizar herramientas y realizar acciones para intentar alcanzar un objetivo.**

Un agente puede buscar información, consultar documentos, trabajar con nuestros correos, analizar datos, interactuar con aplicaciones empresariales o modificar software.

Los **Coding Agents** como Codex, Claude Code, Gemini CLI o GitHub Copilot CLI son ejemplos muy visibles de este cambio, pero representan solamente un tipo de agente.

La idea fundamental es mucho más amplia:

> **Cuando conectamos un modelo de IA con contexto, instrucciones y herramientas, dejamos de pensar solamente en qué puede responder el modelo y empezamos a pensar en qué puede hacer.**
