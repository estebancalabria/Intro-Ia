# Clase Seis - 30 de Octubre del 2026

# Repaso

* IA Creativa
  * Generacion de Canciones
    * Suno
    * Udio
* IA y Productividad
  * Presentaciones
    * Gamma
    * 365 - PowerPoint - Copilot (Paga)
    * Pretzi
      * Forma distinta para presentaciones
  * Hey Gen
    * Videos instucionales basado en Avatar
  * NotebookLM

---

# Herramientas de IA

## NotebookLM

* Quedo pendiente ver el audio, video y presentacion de la clase pasada
  * https://notebook.google.com/notebook/d90f2913-8843-4f76-aa25-930abf885510/artifact/d56e7e51-16ad-490f-b9de-a7d0063a59ee?utm_source=nlm_web_share&utm_medium=google_oo&utm_campaign=art_share_1&utm_content=&utm_smc=nlm_web_share_google_oo_art_share_1_
  * https://notebook.google.com/notebook/d90f2913-8843-4f76-aa25-930abf885510/artifact/beb1218f-a912-4905-bb16-97c18809b513?utm_source=nlm_web_share&utm_medium=google_oo&utm_campaign=art_share_1&utm_content=&utm_smc=nlm_web_share_google_oo_art_share_1_

## Text-To-Speech

* Para reuniones online, clases grabada, reunione online
  * Taqtic
    * https://tactiq.io/
  * Si queres mas herramientas de este tipo
    * https://www.instagram.com/p/DBzb-kHxqae/

# Ciencia de Datos

* Data Science
  * Analizar, procesar y visualizar datos
  * No necesariamente es con IA
  * Mucha Probabilidad y estadistica
* Machine Learning
  * Algotimos para predecir
  * Son algorimos conocidos y super estudiados
  * Entramos en la IA traicionales
* Deep Learning
  * Redes neuronales
  * Aca entran modelos como Transformer y ChatGPt
  

# AiDev

## LLM y Prompt Enginieering

* Los llm son muy buenos generando codigo en incluso algunos como Chatgpt (mas limitado en la version free) tienen interprete de codigo en python : genera codigo y mientras no sea algo web o con interfaz grafica lo ejectua

```
Generame un codigo en python que calcule los numeros primos entre 1 y 100 y los muestre por pantalla. Ejecuta el codigo y mostrame la salida
```

* Hay una libreria en Python que se llama MatPlotLib y es la que usan todos los que trabajan con ciencia de datos.
  * https://matplotlib.org/
  * https://matplotlib.org/stable/gallery/index
 
```
Generame un histograma donde se vea la distribucion de sueldos en argentina segun la edad. Generalo con python y matplotlib, ejecutalo y mostrame el resultado. Si algun dato no tenes, lo podes inferir
```

## IAs para Programar

* Hay varias
  * Lovable
    * https://lovable.dev/es/
  * Base44
    * https://base44.com/

* Vamos a hacer una aplicacion para llevar la organizacion personal con Lovable
* Primero le pido el prompt a ChatGPT

```
# Proyecto: Personal Organizer – Aplicación de organización personal

## 1. Objetivo general

Desarrollar una aplicación web de organización personal que permita administrar de manera centralizada las actividades, responsabilidades, proyectos, compromisos, objetivos y hábitos de una persona.

La aplicación debe funcionar como un centro de control personal (Personal Life Management System), ayudando al usuario a organizar su tiempo, priorizar actividades, realizar seguimiento de sus compromisos y evaluar su progreso.

No debe ser simplemente una lista de tareas. Debe integrar diferentes dimensiones de la organización personal en una única plataforma.

La aplicación debe ser responsive, moderna, intuitiva y visualmente atractiva, con una experiencia de usuario comparable a herramientas como Todoist, Notion, TickTick y Microsoft To Do.

## 2. Diseño y experiencia de usuario

Crear una interfaz moderna, minimalista y profesional.

Características visuales:
- Diseño limpio, evitando la sobrecarga de información.
- Sidebar de navegación lateral.
- Dashboard principal con widgets configurables.
- Modo claro y oscuro.
- Diseño responsive para desktop, tablet y dispositivos móviles.
- Colores neutros con un color de acento.
- Tarjetas con información resumida.
- Indicadores visuales de progreso.
- Calendarios interactivos.
- Formularios intuitivos para crear y editar elementos.
- Notificaciones visuales para vencimientos y recordatorios.

La navegación debe ser consistente y permitir acceder rápidamente a las funcionalidades principales.

## 3. Módulos funcionales

### 3.1. Dashboard – Panel principal

Debe ser la pantalla inicial de la aplicación.

Mostrar:

- Saludo personalizado según la hora del día.
- Fecha actual.
- Resumen de tareas pendientes.
- Tareas vencidas.
- Tareas que vencen hoy.
- Próximos compromisos.
- Eventos del calendario.
- Proyectos activos y su porcentaje de avance.
- Hábitos pendientes de completar.
- Objetivos personales en curso.
- Resumen de actividades completadas durante la semana.

Incluir una sección denominada "Mi día" que concentre las actividades más importantes de la jornada.

Permitir visualizar:
- Prioridades del día.
- Tareas programadas.
- Próximos eventos.
- Tareas pendientes sin fecha asignada.

Incluir accesos rápidos para crear una tarea, evento, nota, proyecto u objetivo.

### 3.2. Gestión de tareas (Task Management)

Implementar un sistema completo de administración de tareas.

Cada tarea debe permitir definir:

- Título.
- Descripción.
- Fecha de creación.
- Fecha de vencimiento.
- Fecha y hora de inicio.
- Prioridad: baja, media, alta y urgente.
- Estado: pendiente, en progreso, completada y cancelada.
- Categoría.
- Proyecto asociado (opcional).
- Etiquetas.
- Tiempo estimado de ejecución.
- Tiempo real utilizado.
- Recordatorios.
- Subtareas.
- Notas adicionales.

Funcionalidades:

- Crear, editar, eliminar y duplicar tareas.
- Marcar tareas como completadas.
- Crear subtareas y listas de verificación.
- Establecer tareas recurrentes (diarias, semanales, mensuales y personalizadas).
- Posponer tareas.
- Asignar prioridades.
- Filtrar por estado, prioridad, categoría, proyecto y vencimiento.
- Buscar tareas.
- Ordenar por fecha, prioridad o creación.
- Detectar tareas vencidas.
- Visualizar tareas sin fecha asignada.
- Mostrar el progreso de las subtareas.

Incluir diferentes vistas:

- Todas las tareas.
- Mi día.
- Próximas.
- Vencidas.
- Completadas.
- Por proyecto.
- Por categoría.

Permitir visualizar las tareas en formato de lista y Kanban.

### 3.3. Calendario y agenda

Implementar un calendario interactivo que integre eventos y tareas programadas.

Vistas disponibles:

- Día.
- Semana.
- Mes.
- Agenda.

Cada evento debe incluir:

- Título.
- Descripción.
- Fecha.
- Hora de inicio y finalización.
- Ubicación.
- Categoría.
- Recordatorio.
- Notas.

Funcionalidades:

- Crear, editar y eliminar eventos.
- Arrastrar y soltar eventos para cambiar su horario.
- Visualizar tareas con fecha de vencimiento.
- Identificar visualmente eventos y tareas mediante colores.
- Mostrar compromisos próximos.
- Detectar superposiciones de horarios.
- Permitir eventos recurrentes.

El calendario debe estar integrado con el módulo de tareas.

### 3.4. Gestión de proyectos

Permitir organizar tareas relacionadas dentro de proyectos.

Cada proyecto debe tener:

- Nombre.
- Descripción.
- Fecha de inicio.
- Fecha objetivo de finalización.
- Estado: planificación, activo, pausado y finalizado.
- Prioridad.
- Color identificador.
- Lista de tareas asociadas.
- Porcentaje de progreso.
- Notas.

Funcionalidades:

- Crear, editar, archivar y eliminar proyectos.
- Agregar tareas existentes.
- Crear tareas directamente dentro del proyecto.
- Visualizar el avance del proyecto.
- Identificar tareas pendientes y completadas.
- Visualizar el proyecto mediante Kanban.
- Mostrar fechas importantes y vencimientos.

Incluir una vista general de todos los proyectos activos.

### 3.5. Gestión de hábitos (Habit Tracker)

Implementar un módulo para crear y realizar seguimiento de hábitos personales.

Ejemplos:

- Hacer ejercicio.
- Leer.
- Estudiar.
- Meditar.
- Beber agua.
- Dormir adecuadamente.
- Practicar un idioma.

Cada hábito debe incluir:

- Nombre.
- Descripción.
- Frecuencia.
- Días de la semana.
- Objetivo cuantificable opcional.
- Unidad de medida.
- Fecha de inicio.
- Categoría.

Funcionalidades:

- Registrar cumplimiento diario.
- Registrar cantidades cuando corresponda.
- Visualizar rachas consecutivas (streaks).
- Mostrar porcentaje de cumplimiento.
- Consultar historial.
- Visualizar resultados mediante calendarios y gráficos.
- Permitir pausar o finalizar hábitos.

### 3.6. Objetivos personales (Goals)

Crear un módulo para definir y realizar seguimiento de objetivos de corto, mediano y largo plazo.

Cada objetivo debe incluir:

- Nombre.
- Descripción.
- Categoría.
- Fecha de creación.
- Fecha objetivo.
- Nivel de prioridad.
- Estado.
- Indicador de progreso.
- Hitos intermedios.
- Tareas relacionadas.

Ejemplos de categorías:

- Profesional.
- Financiero.
- Personal.
- Educación.
- Salud y bienestar.
- Familia.
- Proyectos personales.

Permitir dividir objetivos grandes en hitos y tareas concretas.

Mostrar visualmente el progreso de cada objetivo.

### 3.7. Notas y organización de información

Implementar un espacio para registrar y organizar información personal.

Cada nota debe permitir:

- Título.
- Contenido con formato enriquecido.
- Categoría.
- Etiquetas.
- Fecha de creación.
- Última modificación.
- Favoritos.

Funcionalidades:

- Crear, editar y eliminar notas.
- Buscar por título o contenido.
- Organizar mediante categorías y etiquetas.
- Fijar notas importantes.
- Archivar notas.
- Convertir una nota en tarea.
- Asociar notas a proyectos.

### 3.8. Categorías y etiquetas

Permitir crear categorías personalizadas para clasificar tareas, eventos, notas, proyectos y objetivos.

Ejemplos:

- Trabajo.
- Personal.
- Estudios.
- Finanzas.
- Hogar.
- Salud.
- Ocio.

Las etiquetas deben permitir clasificar elementos transversalmente.

Cada categoría puede tener un color identificador.

### 3.9. Recordatorios y notificaciones

Implementar un sistema de recordatorios.

Debe permitir:

- Configurar recordatorios para tareas y eventos.
- Recordatorios previos al vencimiento.
- Alertas de tareas vencidas.
- Notificaciones de compromisos próximos.
- Recordatorios de hábitos.
- Notificaciones dentro de la aplicación.

Preparar la arquitectura para futuras notificaciones por correo electrónico y notificaciones push.

### 3.10. Estadísticas y productividad

Crear una sección de estadísticas para analizar la organización personal.

Mostrar:

- Tareas completadas por día, semana y mes.
- Tareas pendientes.
- Tareas vencidas.
- Porcentaje de cumplimiento.
- Distribución de tareas por prioridad.
- Distribución de tareas por categoría.
- Tiempo estimado versus tiempo real.
- Progreso de proyectos.
- Cumplimiento de hábitos.
- Evolución de objetivos.

Incluir gráficos de barras, líneas y anillos de progreso.

Permitir filtrar las estadísticas por períodos.

## 4. Búsqueda global

Implementar un buscador global que permita encontrar:

- Tareas.
- Eventos.
- Proyectos.
- Notas.
- Objetivos.
- Hábitos.

Los resultados deben mostrar el tipo de elemento y permitir acceder directamente a su detalle.

## 5. Modelo de datos

Diseñar una base de datos relacional que contemple las siguientes entidades:

- Users
- Tasks
- Subtasks
- Projects
- Events
- Habits
- HabitEntries
- Goals
- GoalMilestones
- Notes
- Categories
- Tags
- TaskTags
- Reminders
- Notifications

Establecer correctamente las relaciones entre las entidades.

Utilizar identificadores únicos, fechas de creación y modificación, y relaciones con integridad referencial.

Cada usuario debe tener sus propios datos privados.

## 6. Arquitectura tecnológica

Utilizar:

- Frontend: React con TypeScript.
- Estilos: Tailwind CSS.
- Componentes: shadcn/ui.
- Backend y base de datos: Supabase.
- Autenticación: Supabase Auth.
- Base de datos: PostgreSQL.
- Gráficos: Recharts.
- Calendario: una librería de calendario interactivo compatible con React.

Implementar Row Level Security (RLS) en Supabase para garantizar que cada usuario solamente pueda consultar y modificar sus propios datos.

No almacenar datos sensibles en el frontend.

Separar correctamente los componentes, servicios, modelos y lógica de negocio.

## 7. Autenticación y usuarios

Implementar:

- Registro de usuarios.
- Inicio de sesión.
- Cierre de sesión.
- Recuperación de contraseña.
- Perfil de usuario.
- Configuración de preferencias.
- Zona horaria.
- Preferencias de visualización.
- Modo claro y oscuro.

## 8. Reglas de negocio importantes

- Una tarea puede existir sin estar asociada a un proyecto.
- Una tarea puede tener subtareas.
- Una tarea puede tener una fecha de vencimiento sin tener horario.
- Los eventos tienen horario de inicio y finalización.
- Los elementos completados deben conservarse en el historial.
- Las tareas recurrentes deben generar nuevas ocurrencias sin perder el historial de las anteriores.
- El progreso de los proyectos debe calcularse a partir de sus tareas.
- Los objetivos pueden estar vinculados a varios proyectos o tareas.
- Los hábitos deben conservar su historial de cumplimiento.
- Las fechas y horas deben respetar la zona horaria configurada por el usuario.
- Las eliminaciones de elementos relacionados deben manejarse evitando inconsistencias.

## 9. Datos de demostración

Crear datos iniciales de demostración para que la aplicación no aparezca vacía.

Incluir:

- Al menos 10 tareas de diferentes prioridades y estados.
- 3 proyectos.
- 5 hábitos.
- 3 objetivos.
- 5 eventos de calendario.
- 5 notas.
- Categorías y etiquetas variadas.

Los datos deben representar un escenario realista de organización personal.

## 10. Criterios de calidad y funcionamiento

La aplicación debe ser completamente funcional.

No crear botones decorativos ni funcionalidades simuladas.

Todas las operaciones CRUD deben funcionar y persistir los cambios en la base de datos.

Los formularios deben validar los datos ingresados y mostrar mensajes claros de éxito o error.

Implementar estados de carga, estados vacíos y manejo de errores.

La navegación debe ser rápida y consistente.

Priorizar la usabilidad y la simplicidad sobre la cantidad de elementos visuales.

## 11. Orden de implementación

Implementar el proyecto por etapas:

1. Estructura general, navegación, diseño y autenticación.
2. Dashboard y gestión de tareas.
3. Calendario y eventos.
4. Gestión de proyectos.
5. Hábitos y objetivos.
6. Notas y categorías.
7. Notificaciones.
8. Estadísticas y productividad.

Primero garantizar que los módulos principales funcionen correctamente y que compartan los datos entre sí.

No sacrificar la funcionalidad por intentar implementar todos los módulos simultáneamente.

## 12. Resultado esperado

Entregar una aplicación web de organización personal integral, moderna y funcional.

El usuario debe poder ingresar diariamente, consultar qué tiene que hacer, organizar su agenda, administrar sus proyectos, controlar sus hábitos, registrar información y realizar seguimiento de sus objetivos desde una única plataforma.

La experiencia debe ser simple: capturar información rápidamente, organizarla fácilmente y tener siempre una visión clara de las prioridades y compromisos personales.
```

* Me genero esta pagina
  * https://lovable.dev/preview/K9ZApKvr3lazijmyR74Kqi9IUE8OZmd4

* Puntaje
  * 10 / 10     
