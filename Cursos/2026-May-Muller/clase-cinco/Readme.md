# Clase Cinco - 16 de Junio del 2026

# Repaso

* Prompt Engineering
  * Rol/Persona
  * Claude
      * Skills en Claude
  * Formatos De Salida
      * CSV
      * HTML
      * JSON
      * XML
      * Markdown
      * Mermaid
* Herramientas
  * Napkin
* IA Generativa Creativa
  * Qwen
  * Kimi

# Prompt Engineering 

## PAtrones de Salida en Codigo

### Ejemplo con MatPlotLib

* https://matplotlib.org/stable/gallery/index

```
Generame un diagramde pie con matplotlib con el porcetaje de deudores en Caba
```

* Genera este codigo en python

```python
import matplotlib.pyplot as plt
import matplotlib.patches as mpatches

labels = ['Préstamos\npersonales', 'Tarjetas\nde crédito', 'Empresas', 'Hipotecarios']
values = [12.0, 8.6, 2.5, 1.2]
colors = ['#d62728', '#ff7f0e', '#1f77b4', '#2ca02c']
explode = (0.05, 0.05, 0.05, 0.05)

fig, ax = plt.subplots(figsize=(8, 6))

wedges, texts, autotexts = ax.pie(
    values,
    labels=labels,
    autopct='%1.1f%%',
    colors=colors,
    explode=explode,
    startangle=140,
    textprops={'fontsize': 12},
    pctdistance=0.75
)

for at in autotexts:
    at.set_fontsize(11)
    at.set_fontweight('bold')
    at.set_color('white')

ax.set_title('Morosidad por tipo de línea crediticia\nArgentina – Diciembre 2025', fontsize=14, fontweight='bold', pad=20)

legend_labels = [f'{l.replace(chr(10), " ")} — {v}%" de mora' for l, v in zip(labels, values)]
patches = [mpatches.Patch(color=c, label=ll) for c, ll in zip(colors, legend_labels)]
ax.legend(handles=patches, loc='lower center', bbox_to_anchor=(0.5, -0.18), ncol=2, fontsize=10)

plt.figtext(0.5, -0.04, 'Fuente: BCRA, dic 2025. Los valores representan tasas de mora, no volumen de cartera.',
            ha='center', fontsize=8, color='gray')

plt.tight_layout()
plt.savefig('/mnt/user-data/outputs/morosidad_caba.png', dpi=150, bbox_inches='tight')
print("OK")
```

* Grafico Generado

<img width="425" height="399" alt="image" src="https://github.com/user-attachments/assets/2ba66f33-fcdf-484a-be2d-9c29a514371f" />


* Cuando quiero analizar datos
  * NO -> (Adjuntar Archivo) -> Pedir Analisis por la IA
      * LA Ia no procesar archivos de plantillas de calculo completos
      * No es mejor que los calculos matematicos
  * SI -> (Adjuntar archivo) -> Pedir el codigo en python que hace el analisis -> Dejar que lo ejecute el Proveedor IA ejecute el codigo en python

> [!NOTE]
> SI la ia que uso no ejecuta Python lo puedo hacer desde https://colab.google/

> [!NOTE]
> El analisis de Datos cae no necesariamente en IA generativa, sino en IA tradicional y ciencia de datos

### Ejemplo analisis de Datos


* Le pase un excel y me genero este codigo

```
import pandas as pd

df = pd.read_excel("/mnt/user-data/uploads/Info_Cartera_Columbia.xlsx")
print("Shape:", df.shape)
print("Columnas:", df.columns.tolist())
print("\nTramos únicos:", df['Tramo'].unique())
print("\nPor tramo:")
resumen = df.groupby('Tramo')['$ Capital'].agg(
    Cantidad='count',
    Total='sum'
).sort_values('Total', ascending=False)
resumen['Total_M'] = resumen['Total'] / 1_000_000
print(resumen.to_string())
print("\nTotal general:", df['$ Capital'].sum())

```

* Codigo Corregido

```
import pandas as pd
from google.colab import files
uploaded = files.upload()

import pandas as pd
df = pd.read_excel(list(uploaded.keys())[0])


print("Shape:", df.shape)
print("Columnas:", df.columns.tolist())
print("\nTramos únicos:", df['Tramo'].unique())
print("\nPor tramo:")
resumen = df.groupby('Tramo')['$ Capital'].agg(
    Cantidad='count',
    Total='sum'
).sort_values('Total', ascending=False)
resumen['Total_M'] = resumen['Total'] / 1_000_000
print(resumen.to_string())
print("\nTotal general:", df['$ Capital'].sum())
```

### OTro ejemplo en analisis de Datos

* Prompt

```
Quiero el codigo en python para colab en un artefacto que me calcule el ratio de plata que hemos recuperado por tramo. Que deje elegir el archivo interactivamente y que me muestre como resultado tanto texto como graficos en matplotlib
```

* Me genero

```
from google.colab import files
import pandas as pd
import matplotlib.pyplot as plt
import matplotlib.ticker as mticker

# ── Carga interactiva ──────────────────────────────────────────────────────────
print("Seleccioná el archivo Excel de cartera Columbia:")
uploaded = files.upload()
filename = list(uploaded.keys())[0]

cartera    = pd.read_excel(filename, sheet_name="Cartera")
rendicion  = pd.read_excel(filename, sheet_name="Rendicion")

# ── Cálculo por tramo ──────────────────────────────────────────────────────────
asignado  = cartera.groupby("Tramo")["$ Capital"].sum().rename("Asignado")
recuperado = rendicion.groupby("Tramo")["$ Rendido"].sum().rename("Recuperado")

df = pd.concat([asignado, recuperado], axis=1).fillna(0)
df["Ratio %"] = (df["Recuperado"] / df["Asignado"] * 100).round(2)
df = df.sort_values("Ratio %", ascending=False)

# ── Salida de texto ────────────────────────────────────────────────────────────
print("\n" + "="*65)
print(f"{'Tramo':<15} {'Asignado':>18} {'Recuperado':>18} {'Ratio %':>8}")
print("="*65)
for tramo, row in df.iterrows():
    print(f"{tramo:<15} {row['Asignado']:>18,.0f} {row['Recuperado']:>18,.0f} {row['Ratio %']:>7.2f}%")
print("-"*65)
total_asig = df["Asignado"].sum()
total_rec  = df["Recuperado"].sum()
print(f"{'TOTAL':<15} {total_asig:>18,.0f} {total_rec:>18,.0f} {total_rec/total_asig*100:>7.2f}%")
print("="*65)

# ── Gráficos ───────────────────────────────────────────────────────────────────
fig, axes = plt.subplots(1, 3, figsize=(18, 6))
fig.suptitle("Recupero por Tramo de Mora — Columbia", fontsize=14, fontweight="bold")

tramos  = df.index.tolist()
colores = ["#2ecc71" if r >= 10 else "#e67e22" if r >= 5 else "#e74c3c"
           for r in df["Ratio %"]]

# 1. Ratio %
axes[0].barh(tramos, df["Ratio %"], color=colores)
axes[0].set_xlabel("Ratio de Recupero (%)")
axes[0].set_title("Ratio % por Tramo")
axes[0].xaxis.set_major_formatter(mticker.FormatStrFormatter("%.1f%%"))
for i, v in enumerate(df["Ratio %"]):
    axes[0].text(v + 0.1, i, f"{v:.2f}%", va="center", fontsize=9)

# 2. Asignado vs Recuperado (en millones)
x      = range(len(tramos))
width  = 0.35
axes[1].bar([i - width/2 for i in x], df["Asignado"] / 1e6,    width, label="Asignado",   color="#3498db")
axes[1].bar([i + width/2 for i in x], df["Recuperado"] / 1e6,  width, label="Recuperado", color="#2ecc71")
axes[1].set_xticks(list(x))
axes[1].set_xticklabels(tramos, rotation=15, ha="right")
axes[1].set_ylabel("Millones $")
axes[1].set_title("Asignado vs Recuperado")
axes[1].yaxis.set_major_formatter(mticker.FuncFormatter(lambda v, _: f"${v:,.0f}M"))
axes[1].legend()

# 3. Distribución del recuperado (torta)
recuperado_no_cero = df[df["Recuperado"] > 0]["Recuperado"]
axes[2].pie(
    recuperado_no_cero,
    labels=recuperado_no_cero.index,
    autopct="%1.1f%%",
    startangle=140,
    colors=["#3498db", "#2ecc71", "#e67e22", "#e74c3c", "#9b59b6", "#1abc9c"]
)
axes[2].set_title("Distribución del Recuperado")

plt.tight_layout()
plt.show()
```

# Herrmientas

## Para presentaciones en PowerPoint : Gamma

* URL
  * https://gamma.app/signup?r=cjucljp9heegmkv
* Caracteristica
 * 
 
* Prompt para la presentacion

```
Quiero una presentacion sobre la morosidad en argentina como incremento en 2026 y las razones
```

* Prompt para la landing

```
Quiero una landing para una persona Juan Perez para intimarlo a pagar una deuda que tiene con el Banco Macro. Que explique los beneficios y la verguenza social de no pagar
``

* Puntaje
  * 9 / 10

## Video Instucionales : Hey Gen

> Para la proxima...
