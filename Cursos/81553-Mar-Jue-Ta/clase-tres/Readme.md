# Clase Tres - 11 de Noviembre 2025

# Repaso

* LLM
  * Propietarios
    * ChatGPT
    * Gemini
    * Claude
    * Perplexity
    * Grok
  * Open Source
    * Groq (Motor de Inferencia)
    * Llama
    * Qwen
    * Deepseeek
    * Mistral
* LMArena
* Hugging Face
  * Spaces de Hugging Face
* Ejecutar LLM Localmente
  * LMStudio
  * Ollama

# Prompt Engineering

## Patrones de Prompting

- ### Patron Rol o Persona

Sin el patron:
```
Quiero vender mi Fiat 500 por internet. Redactame el posteo para ofrecerlo y venderlo.
```

Aplicando el patron persona:
```
Actua como un experto en marketing especialista en autos clasicos. Quiero vender mi Fiat 500 por internet. Redactame el posteo para ofrecerlo y venderlo.
```

Aplicando el patron persona como una persona:
```
Actua como Franco Colapinto. Quiero vender mi Fiat 500 por internet. Redactame el posteo para ofrecerlo y venderlo.
```
Ejemplos del patron persona
> https://github.com/f/awesome-chatgpt-prompts
> https://github.com/estebancalabria/Intro-Ia/tree/main/Prompt%20Engineering/Patrones%20de%20Prompting/Persona


- ### Patron Interaccion

Aplicando tambien el patron de interaccion
```
Actua como un experto nutricionista especialista en las ultimas tendencias de comidas saludables y suplementos nutricionales y quiero que me armes mi plan de alimentacion de la semana. Quiero que me hagas preguntas DE A UNA con repuestas cortas para tener toda la informacion necesaria para armarme el plan optimo. Una vez que tengas toda la informacion armame el plan Responder solamente lo solicitado como para copiar y pegar sin acotar nada mas.
```

- ### Personalizacion de Salida

Formatos de Salida para presetnar informacion

'''
Dame la lista de los mejores libros de stpehen king. Su titulo, anio, resumen trama corto, lista de personajes, ubicacion,
'''

* Tecnicos
   * XML y JSON
   * HTML
        * Sirve para generar PDFS
   * CSV (Comma Seppatated Values)
        * Para comunicarse desde y hacia excel
   * Plantilla Markdown

```markdown
# [Titulo]

**[Fecha de LAnzamiento]**

## Argumento

> [COMPLETAR EL ARGUMENTO DEL LIBRO]

## Personajes

* [Personaje 1]
* [Personaje 2]
...
* [Personaje N]

## Informacion
* Ubicacion Trama : [UBICACION TRAMA]
* Cantidad Capitulos : [CANTIDAD PALABRAS]
* Puntuacion Critica : [Puntuacion de 1 a 5]
---
```

* Generacion de Diagramas
  * Mermaid
     * https://mermaid.live/

Prompt mermaid en Claude
```
Armame un artfacto mermaid que se visualize en un diagrama de flujo el organigrama de Google.  Que tenga a lo sumo 4 nodos por nivel. En lo posible con los nombres de cada uno
```

Prompt mermaid en ChatGPT
```
Armame un diagrama de pie mermaid que muestre las carreras de 5 corredores reconocidos incluyendo Colapinto. Buscar la informacion que haga falta
```
Me genero
```mermaid
pie showData
    title Carreras disputadas en F1 (estimado a nov 2025)
    "Fernando Alonso (422)" : 422
    "Lewis Hamilton (377)" : 377
    "Max Verstappen (229)" : 229
    "Charles Leclerc (168)" : 168
    "Franco Colapinto (26)" : 26

```

* Generar codigo en Python
> https://colab.google/

Prompt para ChatGTP
```
Generame un codigo en python con matplotlib que sea un grafico de velas del bitcoin esta ultima semana
```

Me genero este codigo en colab
```python
import requests
import pandas as pd
import matplotlib.pyplot as plt
import matplotlib.dates as mdates
from datetime import datetime, timedelta

def fetch_ohlc_coin_gecko(coin_id='bitcoin', vs_currency='usd', days=7):
    """
    Obtiene datos OHLC para el coin_id durante ‘days’ días desde CoinGecko.
    Nota: revisá la documentación de CoinGecko para asegurarte del formato.
    """
    url = f'https://api.coingecko.com/api/v3/coins/{coin_id}/ohlc'
    params = {
        'vs_currency': vs_currency,
        'days': days
    }
    resp = requests.get(url, params=params)
    resp.raise_for_status()
    data = resp.json()
    # Formato esperado: [[timestamp, open, high, low, close], ...]
    df = pd.DataFrame(data, columns=['timestamp','open','high','low','close'])
    # Convertir timestamp (ms) a datetime
    df['datetime'] = pd.to_datetime(df['timestamp'], unit='ms')
    df.set_index('datetime', inplace=True)
    df = df[['open','high','low','close']]
    return df

def plot_candlestick(df, title='Candlestick Chart – Bitcoin (Last 7 Days)'):
    """
    Grafica velas de los datos OHLC del dataframe.
    """
    fig, ax = plt.subplots(figsize=(10,6))
    # Convertir fechas a números para matplotlib
    df['date_num'] = mdates.date2num(df.index.to_pydatetime())
    width = 0.6  # ancho de la vela en días (aprox)
    width2 = width * 0.4
    
    for idx, row in df.iterrows():
        date_num = mdates.date2num(idx)
        open_, high_, low_, close_ = row['open'], row['high'], row['low'], row['close']
        
        # Color: verde si cierre > apertura, rojo si cierre < apertura
        color = 'green' if close_ >= open_ else 'red'
        
        # Línea alta‐baja
        ax.plot([date_num, date_num], [low_, high_], color='black', linewidth=1)
        # Rectángulo apertura‐cierre
        rect = plt.Rectangle((date_num - width/2, min(open_, close_)),
                             width, abs(close_ - open_),
                             facecolor=color, edgecolor='black')
        ax.add_patch(rect)
    
    ax.xaxis_date()
    ax.xaxis.set_major_formatter(mdates.DateFormatter('%Y-%m-%d %H:%M'))
    plt.xticks(rotation=45)
    plt.title(title)
    plt.ylabel('USD')
    plt.grid(True)
    plt.tight_layout()
    plt.show()

if __name__ == '__main__':
    # Obtener datos de la última semana
    df_ohlc = fetch_ohlc_coin_gecko(coin_id='bitcoin', vs_currency='usd', days=7)
    plot_candlestick(df_ohlc)

```


- ## Tips de Prompt engineerign
* Ofrecer Recomensas
* Responder solamente lo solicitado como para copiar y pegar sin acotar nada mas.

# Gems

Gemini te permite crear tus propios GEMS y cargarle tanto documentos como informacion personalizada.

# Fine tunning de modelos

> https://www.youtube.com/watch?v=bIZMgHK8Y-8

