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

