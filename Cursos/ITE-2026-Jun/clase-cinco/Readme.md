# Clase Cinco - 2 de Julio 2026

# Repaso

* Large Language Models
  * Canvas / Artefactos
  * Perplexity
    * Investigaciones Academicas
    * Relacionado con el Grounding
* Uso de la API key
  * Python
* Prompt Engineering
    * Formato / Personalizacion de Salida
      * JSON
      * XML
      * HTML
        * Darle formato a la salida del LLM y generar pdfs
      * CSV
        * Interactuar con planilas de calculo
      * Markdown
        * https://es.wikipedia.org/wiki/Markdown
        * Para definir una plantilla con la salida exacta experada del llm
        * Es el formato por defecto en el que el llm genera la salida

---

# Prompt Engineering

## Formatos de Salida : Generacion de Diagramas

### Mermaid

* URL
  * https://mermaid.live/
* Usos
  * Es un lenguaje que le puedo solicitar a la IA para hacer diagramas
  * La mayoria de los modelos ya incluyen previsualizacion


* Voy a probar sobre el informe que hicimos con el modo investigacion de Gemini

```
Haceme un diagrama de pie mermaid donde se vea la distribucion del consumo de papel tissue por region de Espania
```

* Me genero este diagrama

```mermaid
pie title Distribución Estimada del Consumo de Papel Tisú en España
    "Andalucía" : 18.5
    "Cataluña" : 15.5
    "Comunidad de Madrid" : 13.7
    "Comunidad Valenciana" : 10.7
    "Galicia" : 7.6
    "País Vasco" : 5.5
    "Castilla y León" : 4.7
    "Resto de España" : 23.8
```

* Voy a probar con la previsualizacion en ChatGPT (o Claude)

```
Dame un diagrama de flowchart en mermaid que muestre el organigrama de espania en 3 niveles y maximo 3 cuadrados por nivel. Que sea aproximado.
```

* Me genero este diagrama

```mermaid
flowchart TD

%% Nivel 1
A[España]

%% Nivel 2
A --> B[Monarquía]
A --> C[Gobierno]
A --> D[Parlamento]

%% Nivel 3
B --> B1[Rey Felipe VI]

C --> C1[Presidente del Gobierno]
C --> C2[Consejo de Ministros]
C --> C3[Vicepresidencias]

D --> D1[Cortes Generales]
D --> D2[Congreso de los Diputados]
D --> D3[Senado]
```

### Generacion de Codigo para graficos

* Las IA (como chatGPT) muchas veces incluyen un entorno controlado donde ejecutan el codigo generado
 * La ejecucion de codigo muchas veces requiere tener creditos en los ultimo modelos

* Librerias de python utiles
  * MatPlotLib

* Utilice este prompt

```
Podes generar un grafico en matplotlib de stacked bar chart que muestre el ingreso de promedio de sueldos en Espania segun rango etario diferenciado en una misma barra entre hombres y mujeres?
```

* Primero genero este codigo en python

```python
import matplotlib.pyplot as plt

edades = ["<25", "25-34", "35-44", "45-54", "55-64", "65+"]
# Promedio simple de los subtramos quinquenales (INE, EES 2022)
mujeres = [11332.5, 20852.2, 23986.0, 26223.3, 27072.8, 25437.3]
hombres = [14386.9, 23564.1, 29391.6, 32280.4, 32658.2, 35612.0]

fig, ax = plt.subplots(figsize=(9,6))
ax.bar(edades, mujeres, label="Mujeres", color="#d17bb0")
ax.bar(edades, hombres, bottom=mujeres, label="Hombres", color="#4c72b0")

ax.set_title("Salario medio anual en España por rango etario y sexo (2022)")
ax.set_ylabel("Euros brutos anuales")
ax.set_xlabel("Rango etario")
ax.legend()
ax.grid(axis="y", alpha=0.3)

for i, (m, h) in enumerate(zip(mujeres, hombres)):
    ax.text(i, m/2, f"{m:,.0f}", ha="center", va="center", color="white", fontsize=8)
    ax.text(i, m+h/2, f"{h:,.0f}", ha="center", va="center", color="white", fontsize=8)

plt.tight_layout()
plt.savefig("salarios_espania.png", dpi=150)
```
  
* Me genero Claude este grafico
<img width="1350" height="900" alt="image" src="https://github.com/user-attachments/assets/8bf3f261-57c0-4dd8-8665-9a04b8360c0d" />

> [!NOTA]
> El resultado de la IA en casos el anterior hay que evaluarlos, contrastarlos, tomarlos com pinzas
