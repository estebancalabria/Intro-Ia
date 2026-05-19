# Claude: Características para Productividad con IA

> Guía para el curso de IA y Productividad  
> Última actualización: Mayo 2026

---

## Los tres productos de Claude

| Producto | Para quién | Acceso |
|---|---|---|
| **Claude.ai** (web/móvil/desktop) | Todos los usuarios | claude.ai |
| **Claude Desktop** | Usuarios que quieren MCP | App descargable |
| **Claude Code** | Desarrolladores | CLI / terminal |

---

## Claude.ai — Lo que puedes mostrar en demo

### ✅ Artefactos
Genera código, documentos, SVGs y mini-apps React renderizadas en vivo dentro del chat. El usuario puede interactuar con ellas sin salir de Claude.

### ✅ Proyectos
Espacios de trabajo persistentes con archivos, PDFs y un system prompt fijo. Claude mantiene el contexto durante toda la conversación del proyecto. Es el equivalente más cercano a "instrucciones personalizadas por área".

### ✅ Memoria
Claude recuerda información entre conversaciones: nombre, rol, preferencias, contexto profesional. Se activa en Ajustes. Demo: preguntarle "¿qué sabes de mí?"

### ✅ Búsqueda web en tiempo real
Claude puede buscar en internet dentro de la conversación, sin salir del chat.

### ✅ Deep Research
Genera reportes largos y profundos consultando múltiples fuentes. Muy impactante para audiencias de productividad.

### ✅ Análisis de archivos
Sube un PDF, Excel, imagen o CSV y Claude lo analiza, extrae datos o responde preguntas sobre él.

### ✅ Ejecución de código
Claude corre Python internamente y muestra resultados, gráficas y cálculos reales — no solo genera el código.

### ✅ Estilos de escritura
Entrena el estilo de redacción propio para que Claude escriba como tú. Útil para newsletters, correos y posts.

### ✅ Sin publicidad
Claude.ai no tiene anuncios ni promociones pagadas. Lo que responde no está influenciado por anunciantes.

---

## ⚠️ Limitación honesta: Sin skills para usuarios

En Claude.ai **no existe un sistema de skills** que el usuario pueda cargar o modularizar. Lo más cercano:

- **Instrucciones personalizadas** en Ajustes → texto fijo que Claude lee siempre
- **System prompt en Proyectos** → contexto permanente por proyecto

La diferencia con Claude Code es que ahí las skills son **modulares y contextuales** — solo consumen contexto cuando se necesitan. En Claude.ai todo está siempre cargado, lo cual es menos eficiente.

---

## Claude Desktop + MCP — El gran diferenciador

**MCP (Model Context Protocol)** convierte a Claude de chatbot en agente que ejecuta tareas reales en tus herramientas.

> *"Es como darle a Claude manos para tocar tu computadora y tus apps."*

### Conexiones posibles
- Google Drive / Gmail
- Notion
- Sistema de archivos local
- Bases de datos
- GitHub
- Cualquier servicio con conector MCP

### Demo recomendada
Claude leyendo y escribiendo en Notion o Drive directamente desde la conversación — sin copiar y pegar.

---

## Claude Code — Para desarrolladores

Sistema completo de memoria y personalización por proyecto:

| Mecanismo | Qué hace |
|---|---|
| `CLAUDE.md` | Instrucciones permanentes que Claude lee al inicio de cada sesión |
| `.claude/rules/` | Reglas modulares por carpeta o tipo de archivo |
| `Skills (SKILL.md)` | Workflows reutilizables, se activan solo cuando son relevantes |
| **Auto memory** | Claude escribe sus propias notas sobre el proyecto entre sesiones |
| **MCP** | Conexión con herramientas externas vía `.mcp.json` |

### Skills en Claude Code
```
.claude/
  skills/
    mi-skill/
      SKILL.md   ← solo se carga cuando Claude la necesita

~/.claude/
  skills/         ← disponibles en todos tus proyectos
```

---

## Secuencia de demo sugerida para el curso

1. **Sube un PDF** → pídele que resuma y extraiga datos clave
2. **Crea un Artefacto** → dashboard o mini-app interactiva
3. **Activa búsqueda web** → pregunta algo de actualidad
4. **Muestra Proyectos** → cómo mantiene contexto entre sesiones
5. **Deep Research** → genera un reporte en minutos
6. **Claude Desktop + MCP** → Claude escribiendo en Notion en vivo ← 🔥 más impactante

---

## Comparativa rápida por perfil de audiencia

| Característica | Claude.ai | Claude Desktop | Claude Code |
|---|---|---|---|
| Artefactos | ✅ | ✅ | ✅ |
| Proyectos | ✅ | ✅ | — |
| Memoria | ✅ | ✅ | ✅ avanzada |
| Skills propias | ❌ | ❌ | ✅ |
| MCP | Parcial | ✅ pleno | ✅ |
| Búsqueda web | ✅ | ✅ | ✅ |
| Deep Research | ✅ | ✅ | — |
| Para quién | Todos | Todos | Devs |

---

*Recursos oficiales:*  
- [claude.ai](https://claude.ai)  
- [Documentación](https://docs.claude.com)  
- [Soporte](https://support.claude.com)
-
