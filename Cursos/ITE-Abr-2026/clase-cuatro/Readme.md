# Clase Cuatro - 28 de Abril del 2026

# Repaso

* Large Language Models
  * Propietarios
      * ChatGPT
          * Canvas
      * Claude
          * Artefactos
  * Open Source
      * Inportantes por todo el tema de datos sensibles y privacidad
      * Hugging Face
          * Repositorio de modelos Open Source
          * Spaces para probar modelos Open Source
      * Ejecutar un modelo localmente
          * LMStudio
  * Comparar modelos y elegir el mejor segun tarea
      * LMarena (arena.ai)
* Prompt Engineering
  * Componentes de un prompt
      * Tarea+contexto+rol+ejemplo+Fotmato+tono
  * Patrones de Prompting
    * Contexto
      * Interaccion / Prompt Chaining
      
# Prompt Engineeting

## Patron de Promting

### Rol / Persona

* Actua como si fueras....
* Se le dice a la IA desde que lugar quiero la respuesta

* Actividad
    * Solapa 1 :
      * "Quiero que me digas como construir una casa en un terreno. Dame una respuesta"
        * https://chat.qwen.ai/s/4b22b464-5f9a-472d-948e-9100f8ef4e70?fev=0.2.45
    * Solapa 2:
      * "Quiero que actues como un experto en construccion ecologica y sustentable. Quiero que me digas como construir una casa en un terreno"
        * https://chat.qwen.ai/s/61e5cab1-53cf-4ffc-9868-dce4730937f4?fev=0.2.45
    * Solapa 3:
      * "Actua como Amancio Ortega. Quiero que me digas como construir una casa en un terreno. Dame una respuesta"
        * https://chat.qwen.ai/s/0c6e9ad0-f002-4e2f-82a6-5b3f7602e238?fev=0.2.45
    * Solapa 4:
      * "Quiero que me conformes un panel de expertos especialista y que cada uno me de su vision. Quiero que me digas como construir una casa en un terreno. Dame un parrafo para cada especialista"
        * https://chat.qwen.ai/s/94baec68-1e72-41b1-82ec-c9ae2e39c257?fev=0.2.45

### Personalizacion de Salida 

* Considero que es uno de los mas utiles de todo
* Para pasar a las grandes ligas de prompt engineering
* Formatos de Salida
    * Tecnicos
      * Se usan en contextos tecnicos para importar informacion en sistemas
          * XML
          * JSON
        * Se utiliza para generar un pdf con formato
          * Aunque no sepamos escribir html, esta bueno saber que es, para que se usa y poder generar a partir de el pdfs con formato
          * HTML
          * El achivo html lo podes decargar y luego con ctrl+p (imprimir) guardarlo en un archivo pdf.
      * Trabajo con planillas de calculo
          * CSV (comma separated Values)
          * Ese archivo lo podemos abrir directamente desde excel o con google sheets

```
Dame una lista con los 10 edificios mas emblematicos del mundo. Quiero saber la altura, el lugar, el costo aproximado, el uso que se le da, el arquitecto o estudio responsable, cuando se consturyo, y un parrafo que lo describa.
```

####  En json

```json
[
  {
    "nombre": "Burj Khalifa",
    "altura_m": 828,
    "ubicacion": "Dubái, Emiratos Árabes Unidos",
    "costo_aproximado_usd": 1500000000,
    "uso": "Mixto (residencial, oficinas, hotel)",
    "arquitecto": "Adrian Smith (SOM)",
    "construccion": "2004-2010",
    "descripcion": "El edificio más alto del mundo, símbolo del crecimiento de Dubái. Su diseño en forma de Y optimiza la estabilidad estructural y permite múltiples usos."
  }
]
```

#### Em xml

```xml
<edificios>
  <edificio>
    <nombre>Burj Khalifa</nombre>
    <altura_m>828</altura_m>
    <ubicacion>Dubái, Emiratos Árabes Unidos</ubicacion>
    <costo_aproximado_usd>1500000000</costo_aproximado_usd>
    <uso>Mixto (residencial, oficinas, hotel)</uso>
    <arquitecto>Adrian Smith (SOM)</arquitecto>
    <construccion>2004-2010</construccion>
    <descripcion>El edificio más alto del mundo, símbolo del crecimiento de Dubái. Su diseño en forma de Y optimiza la estabilidad estructural y permite múltiples usos.</descripcion>
  </edificio>
  </edificios>
```

### En html

```
Me poader armar un html unico que se vea profeional y elegante para poder exportar mi lista en un pdf y darsela a un cliente
```

* Con eso generamos un pdf

### En CSV

```
Generarme la lista en CSV
```

* Genero
```
nombre,altura_m,ubicacion,costo_aproximado_usd,uso,arquitecto,construccion,descripcion
"Burj Khalifa",828,"Dubái, Emiratos Árabes Unidos",1500000000,"Mixto (residencial, oficinas, hotel)","Adrian Smith (SOM)","2004-2010","El edificio más alto del mundo, símbolo del crecimiento de Dubái y de los límites actuales de la ingeniería."
"Eiffel Tower",300,"París, Francia",1500000,"Turístico y antena","Gustave Eiffel","1887-1889","Ícono global de la arquitectura en hierro y símbolo cultural de París."
"Empire State Building",443,"Nueva York, EE.UU.",40000000,"Oficinas y turismo","Shreve, Lamb & Harmon","1930-1931","Representa la ambición industrial estadounidense y el estilo Art Deco."
"Sydney Opera House",65,"Sídney, Australia",102000000,"Centro cultural","Jørn Utzon","1959-1973","Diseño icónico inspirado en velas, fusiona arquitectura y escultura."
"Sagrada Família",172,"Barcelona, España",25000000,"Basílica","Antoni Gaudí","1882-presente","Obra maestra del modernismo, inspirada en la naturaleza y aún en construcción."
"Guggenheim Museum Bilbao",50,"Bilbao, España",100000000,"Museo","Frank Gehry","1993-1997","Ejemplo icónico de arquitectura contemporánea que revitalizó una ciudad."
"Fallingwater",30,"Pensilvania, EE.UU.",155000,"Residencial (museo)","Frank Lloyd Wright","1935-1939","Integración perfecta entre arquitectura y naturaleza sobre una cascada."
"Louvre Pyramid",21.6,"París, Francia",100000000,"Entrada de museo","I. M. Pei","1984-1989","Intervención moderna que combina historia y diseño contemporáneo."
"Petronas Towers",452,"Kuala Lumpur, Malasia",1600000000,"Oficinas","César Pelli","1993-1998","Torres gemelas inspiradas en geometría islámica."
"Taipei 101",508,"Taipéi, Taiwán",1900000000,"Oficinas y observatorio","C.Y. Lee","1999-2004","Diseño inspirado en el bambú que combina tradición y tecnología."
```

> [!NOTE]
> Lo podemos importar en el excel en 365 o en el google sheets
> Tambien vimos que dentro del 365 si tengo la licencia con copilot puedo hacer cambios directamente en el documento

> [!NOTE]
> Puedo pegarle directamente el CSV en el chat de copilit embebido en excel para que cree el libro con la informacion

#### Markdwon

* Es el lenguaje interno que usa ChatGPT para darle formato al texto

# Consultas

* Para generar presentaciones
  * Vamos a ver luego la mejor herramienta para generar presentacion
  * Tambien podemos generar presetnaciones con qwen que casualmente tiene una herramienta especifica para ello
    * https://chat.qwen.ai/s/1e7e0eab-5720-444e-affe-ba44316157f6?fev=0.2.45

# Glosario

* Alucinacion : Cuando la IA se vuelve loca y contesta en forma inconexa, incoherente, cambia que no le pedi, contesta lo que no se pidio, etc...
* No Determinismo de la IA
