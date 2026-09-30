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
Presentación ejecutiva trimestral — Assurance Seguros

# Presentación ejecutiva trimestral — Assurance Seguros

Crea una presentación corporativa ejecutiva para **Assurance Seguros**, una compañía multinacional de seguros, con el objetivo de presentar los resultados del tercer trimestre de 2026 (Q3: julio, agosto y septiembre) ante el comité ejecutivo y los directores regionales.

## Contexto

Assurance Seguros opera en América Latina, Europa y Norteamérica, ofreciendo seguros de automóviles, hogar, vida y empresas. La compañía busca mejorar su rentabilidad, acelerar la transformación digital, aumentar la satisfacción de los clientes y optimizar la gestión de siniestros.

**Importante:** todos los datos, cifras, países, indicadores y resultados de esta presentación son ficticios y se utilizan exclusivamente para una demostración. No representan información real de una compañía.

## Objetivo

Mostrar los resultados financieros y operativos del trimestre, compararlos con el trimestre anterior y con los objetivos establecidos, identificar tendencias y presentar las prioridades para el cuarto trimestre.

## Estructura de la presentación

Crea 10 diapositivas:

1. **Portada**

   * Assurance Seguros.

   * Resultados ejecutivos del tercer trimestre de 2026.

   * Período: julio–septiembre de 2026.

   * Estilo corporativo multinacional.
2. **Resumen ejecutivo**

   * Ingresos por primas: USD 1.280 millones.

   * Crecimiento trimestral: +8,5 %.

   * Ratio combinado: 94,8 %.

   * Satisfacción del cliente: 84/100.

   * Siniestros resueltos dentro del SLA: 91 %.

   * Presentar tres logros y dos desafíos principales.
3. **Resultados financieros**

   * Primas emitidas, ingresos y resultado operativo.

   * Comparación entre Q2 y Q3 de 2026.

   * Comparación con los objetivos trimestrales.

   * Utilizar gráficos de barras y tarjetas KPI.
4. **Rentabilidad y eficiencia**

   * Ratio combinado.

   * Ratio de siniestralidad.

   * Ratio de gastos.

   * Explicar cómo se relacionan los indicadores y qué implican para la rentabilidad técnica.
5. **Resultados por región**

   * América Latina.

   * Europa.

   * Norteamérica.

   * Comparar ingresos, crecimiento y ratio combinado.

   * Utilizar un gráfico comparativo y un mapa estilizado.
6. **Desempeño por línea de negocio**

   * Automóviles.

   * Hogar.

   * Vida.

   * Seguros corporativos.

   * Comparar primas emitidas, crecimiento y rentabilidad técnica.
7. **Operaciones y gestión de siniestros**

   * Total de siniestros recibidos y resueltos.

   * Tiempo promedio de resolución.

   * Porcentaje resuelto dentro del SLA.

   * Nivel de automatización del procesamiento.

   * Identificar oportunidades de mejora.
8. **Experiencia del cliente y transformación digital**

   * Índice de satisfacción del cliente.

   * NPS.

   * Retención de clientes.

   * Porcentaje de operaciones realizadas por canales digitales.

   * Evolución de la adopción digital.
9. **Riesgos, desafíos y oportunidades**

   * Evolución de los costos de siniestros.

   * Diferencias de desempeño entre regiones.

   * Eficiencia operativa.

   * Retención y adquisición de clientes.

   * Automatización de procesos.

   * Separar claramente los hechos medidos de las hipótesis explicativas.
10. **Conclusiones y prioridades para Q4 2026**

```
*   Tres prioridades estratégicas.
```

```
*   Objetivos cuantificables para el próximo trimestre.
    
*   Indicadores para realizar el seguimiento.
    
*   Cierre ejecutivo con próximos pasos.
    
```

## Datos y consistencia

Utiliza exclusivamente los datos ficticios suministrados en el material de entrada o, si faltan datos, crea supuestos claramente identificados como tales. Mantén la coherencia entre cifras, porcentajes, gráficos y conclusiones. No inventes causas como si fueran hechos comprobados.

## Diseño visual

* Formato panorámico 16:9.

* Estética de consultoría estratégica y presentación para comité ejecutivo.

* Paleta: azul marino, blanco, gris claro y verde azulado como color de acento.

* Tipografía moderna, legible y profesional.

* Gráficos claros, tablas compactas y tarjetas KPI.

* Una idea principal por diapositiva.

* Evitar párrafos largos, imágenes de stock genéricas, adornos excesivos y gráficos tridimensionales.

* Incluir títulos que comuniquen conclusiones, no solamente nombres de categorías.

* Mostrar moneda, unidades, período de comparación y variaciones porcentuales.

* Incorporar notas breves cuando un indicador requiera interpretación.

El resultado debe parecer una presentación interna real de una multinacional aseguradora, con lenguaje ejecutivo, análisis cuantitativo y conclusiones respaldadas por los datos. No presentes los datos de demostración como resultados reales.

## 2. Datos ficticios para utilizar en la presentación

Estos son los datos base que podés cargar en Gamma junto con el prompt.

Primas emitidas · Q3 2026

# USD 1.280 M

+8,5 % vs. Q2

Ratio combinado

# 94,8 %

−1,2 puntos porcentuales

Satisfacción del cliente

# 84/100

+3 puntos

Retención de clientes

# 89 %

+1,5 puntos porcentuales

Siniestros dentro del SLA

# 91 %

+4 puntos porcentuales

Datos simulados para una demostración. M = millones de USD.

### Resultados financieros

|
Indicador

|

Q2 2026

|

Q3 2026

|

Objetivo Q3

|
| --- | --- | --- | --- |
|

Primas emitidas

|

USD 1.180 M

|

USD 1.280 M

|

USD 1.250 M

|
|

Ingresos reconocidos

|

USD 1.105 M

|

USD 1.195 M

|

USD 1.180 M

|
|

Resultado operativo

|

USD 105 M

|

USD 124 M

|

USD 120 M

|
|

Ratio combinado

|

96,0 %

|

94,8 %

|

95,0 %

|
|

Ratio de siniestralidad

|

65,0 %

|

63,8 %

|

64,0 %

|
|

Ratio de gastos

|

31,0 %

|

31,0 %

|

31,0 %

|

Los ratios combinados corresponden, por definición, a la suma del ratio de siniestralidad y el ratio de gastos. En este ejemplo, 63,8 % + 31,0 % = 94,8 %.

### Resultados por región

|
Región

|

Primas Q3

|

Variación vs. Q2

|

Ratio combinado

|
| --- | --- | --- | --- |
|

América Latina

|

USD 420 M

|

+11,0 %

|

96,2 %

|
|

Europa

|

USD 510 M

|

+6,0 %

|

92,5 %

|
|

Norteamérica

|

USD 350 M

|

+8,5 %

|

95,4 %

|
|

Total

|

USD 1.280 M

|

+8,5 % aprox.

|

94,8 % aprox.

|

### Resultados por línea de negocio

|
Línea

|

Primas Q3

|

Crecimiento trimestral

|

Ratio combinado

|
| --- | --- | --- | --- |
|

Automóviles

|

USD 480 M

|

+7,0 %

|

98,5 %

|
|

Hogar

|

USD 210 M

|

+5,0 %

|

91,0 %

|
|

Vida

|

USD 310 M

|

+10,0 %

|

No aplica en este ejemplo

|
|

Seguros corporativos

|

USD 280 M

|

+12,0 %

|

91,5 %

|
|

Total

|

USD 1.280 M

|  |  |

Nota: para mantener la coherencia del ejemplo, el ratio combinado consolidado se calcula sobre el negocio de seguros generales sujeto a ese indicador, mientras que Vida se analiza por separado. Los ratios regionales son ilustrativos.

### Operaciones y experiencia del cliente

|
Indicador

|

Q2 2026

|

Q3 2026

|

Objetivo Q3

|
| --- | --- | --- | --- |
|

Siniestros recibidos

|

185.000

|

198.000

|

195.000

|
|

Siniestros resueltos

|

176.000

|

193.000

|

190.000

|
|

Tiempo medio de resolución

|

8,2 días

|

6,9 días

|

7,0 días

|
|

Resolución dentro del SLA

|

87 %

|

91 %

|

90 %

|
|

Procesamiento automatizado

|

42 %

|

55 %

|

50 %

|
|

Satisfacción del cliente

|

81/100

|

84/100

|

83/100

|
|

NPS

|

+32

|

+37

|

+35

|
|

Retención de clientes

|

87,5 %

|

89,0 %

|

88,0 %

|
|

Operaciones por canales digitales

|

61 %

|

68 %

|

65 %

|

## 3. Objetivos ficticios para Q4 2026

Crecimiento

Alcanzar USD 1.350 millones en primas emitidas.

Rentabilidad técnica

Mantener el ratio combinado consolidado por debajo del 95 % en las líneas de negocio comparables.

Automatización

Elevar el procesamiento automatizado de siniestros al 62 %.

Experiencia del cliente

Alcanzar una satisfacción de 86/100 y una retención del 90 %.

Recomendación de presentación: mantené los datos financieros en una misma unidad y usá Q2 como comparación trimestral, aclarando que no se trata de una comparación interanual. Identificá toda la presentación como datos simulados para demostración, especialmente si vas a mostrarla ante un cliente o en una capacitación.
```
```

````
