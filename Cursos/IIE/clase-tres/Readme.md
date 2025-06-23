# Prompt Engineering

## Conceptos de Prompt Engineering (Repaso)
* System Prompt
* Contexto
* Formula de Prompt Efectivo = Tarea + Contexto + Ejemplo + Persona + Fomato + Tono
* Memoria
* Personalizacion ChatGPT

## Patrones de Prompting (Repaso)
* Persona
* Audicence Persona
* Interaccion
* Personalizacion de Salidas (Formatos)
   *  bullets
   *  Json
   *  XML
   *  html
   *  CSV -->  Integracion con Excel)

### Patron Personalizacion de Salida : Markdown

Prompt Inicia
> Dame una lista de 10 paises que debo visitar antes de morir

Prompt Mejorado
> Dame la lista respetando la siguiente plantilla markdown
Plantilla
```markdown
# [Nombre Del Pais]
## Datos
* **Capital** : [CAPITAL]
* **Poblacion** : [POBLACION DEL PAIS]
* **Idioma** : [Idioma del pais]
* **Moneda** : [Moneda del pais]
## 5 Lugares de Interes
1. [Lugat de Interes 1]
2. [Lugat de Interes 2]
...
## Descripcion
[ Descripcion porque debo de conocerlo ]
---
```
