# Clase Cinco - 18 de Noviembre del 2026

# Repaso


* Artefactos de Claude
  * Previsualizacion de ciertos formaos como el codigo
  * En ChatGPT gemini hay algo parecido que se llama Canvas
  * Permite editar parcialmente un entregable gastando menos tokens y evitando ediciones colaterales no de deseadas
* Vibe Coding
  * Generar aplicaciones con lenguaje natural sin escribir codigo
  * La IA escribe el codigo
* Texto-A-Voz
  * ChatGPT de por si tienen texto a voz incorporado
  * Una facil para usar directo : NaturalReaders
  * ElevenLabs la opcion por defecto para generacion de voz pero opciones gratuitas limitadas
* Diagramas y Presentaciones
  * Napkin
    * Enriquecer un texto con Diagramas
    * Ahora genera presetnaciones
  * Gamma
    * El mejor generador de presetanciones
  * PowerPoint
    * Para los que tienen la licencia 365
* Verificacion Cruzada con la IA
* Repositorio de Herramientas
  * There is an AI for That

---

# Video Intitucionales

## Hey Gen

* Ya habiamos visto lo que se puede hacer con HeyGen, ahora les toca a ustedes...

* Crear Video

* Generamos el siguiente Script con ChatGPT

```
Jensen Huang se va de Nvidia y el mercado entra en pánico. Pero ¿estamos ante el principio del fin de una era o frente a una oportunidad histórica de inversión?

La salida de su fundador provoca incertidumbre sobre el futuro de la compañía, especialmente por la falta de un sucesor definitivo y el riesgo de perder talento clave.

Sin embargo, hay algo importante: el negocio sigue creciendo. Nvidia mantiene una demanda extraordinaria de sus chips de inteligencia artificial, Blackwell avanza y Vera Rubin promete llevar su tecnología todavía más lejos.

La acción llegó a caer casi un 39% desde su máximo histórico. Y aquí aparece la gran pregunta: ¿está barata?

La estrategia analizada propone no vender por pánico ni invertir todo de golpe: acumular en tres etapas, esperar los resultados financieros y observar quién asumirá el liderazgo.

```

* Ahora a esperar que termine...

* Genero
  * https://app.heygen.com/videos/salida-juang-nvidia-7ce4729f0a1241218b781b19463b6835

# Interpete de codigo

* Los modelos de lenguaje tienen la capacidad de generar codigo y a la vez para el codigo que se genera en python (un lenguaje muy utilizado para el analsis de datos) tienen tambien la capacidad de ejectutar ese codigo (como vimos con los artefactos)

## Analizar Panillas de Calculo

* Voy a generar con excel una planilla de calculo "de mentirita" que voy a subir a este repo y la voy a analizar con el interprete de codigo
* Con google Sheets y Gemini genere una planilla de prueba con ventas qeu subi aqui

* NO LE VAMOS A PEDIR ASI
  * Si la IA no utiliza el interpete de codigo no son cofianles los resultados que sean cuentas matematicas
```
Quiero me analices el archivo adjunto y me calcules el total de ventas por producto
```

* Se lo pido asi
 * En lugar de que la IA me haga calculo, que genere un prorama en python que haga el calculo
 * Asi es mucho mas confiable
```
Quiero que utilices el interprete de codigo en pytho me analices el archivo adjunto y me calcules el total de ventas por producto
```

> [!NOTE]
> Los modelos de lenguaje generan texto (y en este caso algoritmos) pero no son bueno haciendo cuenta. Son muy propenso a errores

> [!NOTE]
> Si uso CSV en vez de XLS voy a gastar menos tokens porque hay un moton de informacion sobre el formato del archivo (negrita, colores) que el LLM no necesita para hacer los calculos pero procesarlo consume tokens

* ANTES
  * (prompt) + (Archivo Adjunto) -> (IA) -> (Respuesta probabilistica que puede tener errores)
* DESPUES
  * (prompt) + (Archivo Adjunto) -> (IA) -> (Codigo en python que hace el calculo) -> (Interprete de codigo) -> (Respuesta Verificar)

> [!NOTE]
> En 365 el interprete de codigo funciona mejor y de forma nativa con el agente precosntruido "Analista"

## Graficos con MatPlotLib

* MAtplotLib es una libreri de python para hacer graficos y diagramas
  * https://matplotlib.org/
  * https://matplotlib.org/stable/gallery/index#

```
Utiliza el interprete de codigo en Python y MatPlotLib para generar un histograma donde se ve el ingreso por rango de edad (cada 10 anios) considerando el promedio de ingresos de Madrid segun los datos que puedas recopilar
```

* Genero Esto

<img width="495" height="282" alt="image" src="https://github.com/user-attachments/assets/ec8e3b6e-4cba-41e1-9a61-245cc18b50b6" />

* Con este codigo

```python
import matplotlib.pyplot as plt
import numpy as np

edades = ["≤25", "26–35", "36–45", "46–55", "56–65", ">65"]
ingresos = [22680, 32346, 39197, 44128, 42228, 42848]

fig, ax = plt.subplots(figsize=(10, 6))
bars = ax.bar(edades, ingresos, width=0.72, edgecolor="black", linewidth=0.7)

ax.set_title("Ingreso bruto anual medio por rango de edad\nComunidad de Madrid · 2024",
             fontsize=15, pad=16)
ax.set_xlabel("Rango de edad (años)", fontsize=11)
ax.set_ylabel("Ingreso bruto anual medio (€)", fontsize=11)
ax.set_ylim(0, 50000)
ax.grid(axis="y", linestyle="--", alpha=0.35)
ax.set_axisbelow(True)

for bar, value in zip(bars, ingresos):
    ax.text(bar.get_x() + bar.get_width()/2, value + 700,
            f"€{value:,.0f}".replace(",", "."),
            ha="center", va="bottom", fontsize=10)

fig.text(0.5, 0.01,
         "Fuente: Agencia Tributaria de España, Mercado de trabajo y pensiones 2024. "
         "Salario Medio Estimado Anual (SME), ambos sexos.",
         ha="center", fontsize=8, color="dimgray")
plt.tight_layout(rect=[0, 0.04, 1, 1])

path = "/mnt/data/ingreso_medio_edad_madrid_2024.png"
plt.savefig(path, dpi=180, bbox_inches="tight")
plt.show()
print(path)

```

---
# BREAK
# Hasta y 30
---

# Automatizacion

* Teoria de Referencia
  * https://www.instagram.com/p/DIPbzoPOS6v/?img_index=1

* Antes 
  * La automatizacion es antes de la inteligencia artificial
* Despues
   * Automatizacion + IA   = Angente autonomo  -----> "El nirvana de la productividad"
 
* Herramientas de Automatizacion
  * Zappier
    * https://zapier.com/
    * Supo ser el lide de la industria al principio, pero las opciones gratuitas son limitads
  * PowerAutomate
    * Funciona integrado con herramienta 365
    * Requiere licencia de Microsoft
    * Ideal para organizaciones que ya trabajan con Microsoft
  * N8n
     * https://n8n.io/
     * El lider den automatizacion hoy.
     * Es Open Source. Se puede instalar localmente sin tener que pagarle a un tercer.
       * Aunqeu tambien se puede usar como servicio online con subcripcion pagando
     * Tiene una curva de aprendizaje mas alta
  * Make
     * https://www.make.com/
     * Se puede usar en forma gratuita online con limites bastante amplios
     * Es la opcion mas sencilla de todas
     * Ideal para empezar
   
* Como funciona una automatizacion
  * Integran herramientas
     * Whatapp, Telegram, Google Sheets, Word, Excel, Calendario Goole, Access
  * Todo comienza con un Trigger o Disparador
     * Cada x tiempo (Scheduled)
     * Cuando agregan una fila a un exceal
     * Cuando se agrega un evento a un calendario
     * Cuando recibo un mensaje en whatsap...
   * Son herramienta low-code / no-code
     * No se programa nada en lenguaje de programaicon
     * Se arma el flujo visualmente
     * No requiere conocimientos de programacion
    
* Fijense la pagina de templates en Make y cual les resuena con su trabajo y sus tareas diarias
   * Chatbot en Whsatap
   * Rellenar Google Sheets con respuestas de forms

## Automatizacion sin IA

* Herramientas a integrar
   * Calendario de Google
     * https://calendar.google.com/
   * Google Sheets

* Setup
    * Abrir el calendario de Google
    * Crear un documento de google Sheets
      * Darle al documento un nombre reconocible "Sandbox Make"
      * Crearle las columnas "Evento, Inicio, Fin"
        * La columna Inicio y Fin la amos a poner de tipo Fecha 
           * Selecciono la columna -> menu Format -> Number -> DateTime
    * Asegurarse qeu tanto el Google Sheets como el Calendar esten en la misma cuenta

* Cada vez que me conecto a una herrramienta aparece en la opcion de Credentials

* Vamos a la opcions Scenarios y ponemos "Create Scenario"
 
*  Creamos el disparador o trigger
  *  Buscamos Google Calendar
  *  Elegimos Watch Events (El que dice la pabra trigger en la descripcion(
  *  Creamos una conexion con nuestro calendario de Google
    *  Elijo el calendario Principal
         
<img width="279" height="434" alt="image" src="https://github.com/user-attachments/assets/24e718dd-27fe-4191-9daf-59596d2ba466" />

* Probar el Trigger
   * Crearmos un evento en nuestro calendario
   * Ejecutamos la automatizacion
 
> [!NOTE]
> Es sumamente importante cada paso que doy en la automatizacion ir verificandolo

* Generar automaticamente la fila de Excel
  * Agregamos un nodo nuevo
  * Elegimos Google Sheets
  * Luego elegimos el nodo "Add a Row"
  * Podemos reutilizar la conexion que teniamos o crear una conexion nueva
  * Elegimos el archivo y el libro
  * Mapeamos las variables del triger a la planilla
     * Evento (A) -> Summary
     * Inicio (B) -> Start
     * Fin (C)  -> End

<img width="494" height="440" alt="image" src="https://github.com/user-attachments/assets/02e1bb08-8693-46e4-87c7-51b3107ff3e5" />

* Darle Save y verificarlo
   * Creamos un evento
   * Ejecutamos la automatizacion
      * (Ahora la ejecutamos manual pero una vez creada se ejecuta sola)
    * Vemos la planilla
       * Deberia agregarse el evento solo
 
> [!NOTE]
> Felicidades programaron su primera automatizacion (sin IA) 

---

