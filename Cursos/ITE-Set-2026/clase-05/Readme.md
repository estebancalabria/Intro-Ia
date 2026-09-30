# Clase 05 - 30 de Septiembre del 2026

# Repaso

* Prompt Engineering
  * Tecnicas de prompting
      * Rol / Persona
      * Interaccion / Prompt Chaining
      * Formatos de Salida
        * Simples
          * Tabla
          * Bullets y sub bullets
        * Tecnicos
          * xml
          * json
          * csv (interactuar con y desde excel)
          * codigo de programacion
        * Presenteacion
          * pdf
          * 365 -> Powerpoint. word
          * HTML -> mayor personalizacion
        * Markdown
          * Generacion de plantillas de salida
          * Es el lenguaje con la que la IA responde por defecto
        * Diagramas
            * Mermaind
            * SVG
            * Matplotlib

---

# Prompt Engineering

* Tip: Usar la ia como experto experto en prompt engineerings

# Herrmientas de Productividad (Modulo 4)

## Presetnaciones

### Powerpoint en 365

* Con el agente de 365 podemos generar una presentacion facilmente

### Gamma

* Me parece que genera incluso mejores presentaciones que PowerPoint para algunos
* URL
  * https://gamma.app/signup?r=cjucljp9heegmkv
* Caracteristicas
  * Presentacion
  * Graficos
  * Paginas web
  * Publicas para redes Socials

* Con la IA genere este prompt para Gamma

```
# Presentación ejecutiva trimestral — Assurance Seguros

Crea una presentación corporativa ejecutiva para **Assurance Seguros**, una compañía multinacional ficticia de seguros que opera en América Latina, Europa y Norteamérica, ofreciendo seguros de automóviles, hogar, vida y empresas.

## Objetivo

Presentar los resultados del tercer trimestre de 2026 (Q3: julio, agosto y septiembre) ante el comité ejecutivo y los directores regionales. Mostrar resultados financieros y operativos, comparar el desempeño con el trimestre anterior y los objetivos, identificar oportunidades de mejora y establecer prioridades para el cuarto trimestre.

**Importante:** todos los datos, cifras, regiones y resultados son ficticios y se utilizan exclusivamente para una demostración.

## Estructura de la presentación

Crea 10 diapositivas con contenido ejecutivo, análisis cuantitativo y conclusiones respaldadas por los datos.

### 1. Portada

* Assurance Seguros.
* Resultados ejecutivos del tercer trimestre de 2026.
* Período: julio–septiembre de 2026.
* Presentación para el comité ejecutivo.

### 2. Resumen ejecutivo

Presenta los principales indicadores del trimestre:

* Primas emitidas: USD 1.280 millones.
* Crecimiento trimestral: +8,5 %.
* Ratio combinado: 94,8 %.
* Resultado operativo: USD 124 millones.
* Satisfacción del cliente: 84/100.
* Siniestros resueltos dentro del SLA: 91 %.

Incluye tres logros principales y dos desafíos identificados a partir de los datos.

### 3. Resultados financieros

Utiliza los siguientes datos:

| Indicador               |     Q2 2026 |     Q3 2026 | Objetivo Q3 |
| ----------------------- | ----------: | ----------: | ----------: |
| Primas emitidas         | USD 1.180 M | USD 1.280 M | USD 1.250 M |
| Ingresos reconocidos    | USD 1.105 M | USD 1.195 M | USD 1.180 M |
| Resultado operativo     |   USD 105 M |   USD 124 M |   USD 120 M |
| Ratio combinado         |      96,0 % |      94,8 % |      95,0 % |
| Ratio de siniestralidad |      65,0 % |      63,8 % |      64,0 % |
| Ratio de gastos         |      31,0 % |      31,0 % |      31,0 % |

Compara los resultados con Q2 y con los objetivos de Q3. Utiliza tarjetas KPI y gráficos de barras. Expresa las variaciones en porcentajes o puntos porcentuales según corresponda.

### 4. Rentabilidad y eficiencia

Explica la relación entre:

* Ratio de siniestralidad.
* Ratio de gastos.
* Ratio combinado.
* Resultado operativo.

Destaca que el ratio combinado resulta de sumar el ratio de siniestralidad y el ratio de gastos. Identifica las variaciones observadas sin atribuir causas que no estén demostradas por los datos.

### 5. Resultados por región

| Región         |   Primas Q3 | Variación vs. Q2 | Ratio combinado |
| -------------- | ----------: | ---------------: | --------------: |
| América Latina |   USD 420 M |          +11,0 % |          96,2 % |
| Europa         |   USD 510 M |           +6,0 % |          92,5 % |
| Norteamérica   |   USD 350 M |           +8,5 % |          95,4 % |
| Total          | USD 1.280 M |    +8,5 % aprox. |   94,8 % aprox. |

Compara crecimiento, volumen de negocio y rentabilidad técnica por región. Incluye un gráfico comparativo y un mapa estilizado. Señala diferencias regionales que merezcan análisis adicional.

### 6. Desempeño por línea de negocio

| Línea de negocio     |   Primas Q3 | Crecimiento trimestral |           Ratio combinado |
| -------------------- | ----------: | ---------------------: | ------------------------: |
| Automóviles          |   USD 480 M |                 +7,0 % |                    98,5 % |
| Hogar                |   USD 210 M |                 +5,0 % |                    91,0 % |
| Vida                 |   USD 310 M |                +10,0 % | No aplica en este ejemplo |
| Seguros corporativos |   USD 280 M |                +12,0 % |                    91,5 % |
| Total                | USD 1.280 M |                        |                           |

Compara el crecimiento y la contribución de cada línea. Explica que el ratio combinado consolidado debe calcularse sobre las líneas comparables, sin mezclar indicadores de seguros de vida que utilicen métricas de rentabilidad diferentes.

### 7. Operaciones y gestión de siniestros

| Indicador                  |  Q2 2026 |  Q3 2026 | Objetivo Q3 |
| -------------------------- | -------: | -------: | ----------: |
| Siniestros recibidos       |  185.000 |  198.000 |     195.000 |
| Siniestros resueltos       |  176.000 |  193.000 |     190.000 |
| Tiempo medio de resolución | 8,2 días | 6,9 días |    7,0 días |
| Resolución dentro del SLA  |     87 % |     91 % |        90 % |
| Procesamiento automatizado |     42 % |     55 % |        50 % |

Analiza el volumen de trabajo, la velocidad de resolución, el cumplimiento de los SLA y la automatización. Identifica oportunidades para mejorar la eficiencia operativa.

### 8. Experiencia del cliente y transformación digital

| Indicador                         | Q2 2026 | Q3 2026 | Objetivo Q3 |
| --------------------------------- | ------: | ------: | ----------: |
| Satisfacción del cliente          |  81/100 |  84/100 |      83/100 |
| NPS                               |     +32 |     +37 |         +35 |
| Retención de clientes             |  87,5 % |  89,0 % |      88,0 % |
| Operaciones por canales digitales |    61 % |    68 % |        65 % |

Muestra la evolución de los indicadores mediante gráficos sencillos. Distingue entre resultados observados y posibles explicaciones. No afirmes que la digitalización causó mejoras en satisfacción o retención si los datos no permiten establecer esa relación.

### 9. Riesgos, desafíos y oportunidades

Identifica y explica:

* Crecimiento del volumen de siniestros.
* Diferencias de rentabilidad entre regiones y líneas de negocio.
* Costos operativos y de siniestralidad.
* Retención y adquisición de clientes.
* Automatización de procesos.
* Oportunidades de mejora en la experiencia digital.

Separa los hechos medidos de las hipótesis que requieren validación adicional.

### 10. Prioridades para Q4 2026

Utiliza los siguientes objetivos ficticios:

* Primas emitidas: USD 1.350 millones.
* Ratio combinado: inferior al 95 % en las líneas comparables.
* Procesamiento automatizado de siniestros: 62 %.
* Satisfacción del cliente: 86/100.
* Retención de clientes: 90 %.

Presenta tres prioridades estratégicas, los indicadores para realizar su seguimiento y los próximos pasos propuestos.

## Diseño visual

* Formato panorámico 16:9.
* Estética de consultoría estratégica y presentación para comité ejecutivo.
* Paleta corporativa: azul marino, blanco, gris claro y verde azulado.
* Tipografía moderna, profesional y legible.
* Gráficos de barras, líneas de tendencia, tarjetas KPI y tablas compactas.
* Una idea principal por diapositiva.
* Títulos que comuniquen conclusiones, no solamente categorías.
* Uso moderado de iconos y elementos visuales.
* Evitar párrafos extensos, imágenes de stock genéricas y gráficos tridimensionales.
* Mantener consistencia entre cifras, porcentajes, unidades y períodos.
* Indicar siempre si una variación se expresa en porcentaje o en puntos porcentuales.

## Criterios de calidad

La presentación debe tener apariencia de informe interno de una multinacional aseguradora. Utiliza lenguaje ejecutivo, conclusiones concretas y visualizaciones que faciliten la toma de decisiones.

No inventes causas, acontecimientos ni resultados adicionales como si fueran hechos comprobados. Si detectas inconsistencias entre los datos, señálalas o aclara los supuestos antes de elaborar una conclusión. No presentes los datos simulados como resultados reales de una empresa.

Incluye una nota discreta en la portada o al pie de las diapositivas que indique: **“Datos ficticios elaborados exclusivamente para fines demostrativos”.**

```

---
