# Clase Uno - 21 de Abril del 2026

# Roadmap

* Modulo 1 : Large Language Models 
    * Propietarios
        * ChatGPT
        * Gemini
        * Copilot
        * Claude
        * Perplexity
        * Grok
    * Open Source
        * Deepseek
        * Qwen
* Modulo 2 : Prompt Engineering
    * Como escribir prompts
    * Manejo del contexto
    * Patrones de Prompting
      * Rol/Persona
      * Interaccion
      * Formato de salida
* Modulo 3: Herramientas
    * Durante la cursada vamos a ver en forma intercalada diversas herramientas que usan IA
    * Texto-a-voz y Voz-a-Texto
    * Generar Presentaciones
    * Video institucionales (con avatar hablando)
    * ...
    * Criterio a la hora de reconocer que herramienta me puede servir para un problema determinado
* Modulo 4 : IA Creativa
  * Generacion de Imagenes
  * Generacion de Videos
  * Generacion de Canciones
  * Folleteria y diseño grafico
* Modulo 5
  * Criterios de uso de la IA
  * Seguridad, privacidad de los datos
  * IA Tradicional : Trabajar con Datos, reconocer patrones, hacer predicciones
  * (Automatizacion)
  * Agentes
* Modulo Extra : Ai-900 (Microsoft)
  * Azure, la nube, cloud computing. Pose una serie de herramientas de IA que uno puede en ensablar (como piezas de rompecabezas) en una solucion corpatva personaliza

---

# Formas de Contacto

* Instagram
   * https://www.instagram.com/mct.esteban.calabria/
* Linkedin
   * https://www.linkedin.com/in/esteban-calabria-7a44401a/
* Mail de ITE
   * esteban.calabria@institutotecnologicoeuropeo.com

---
# Large Language Models (LLM)

## Caracteristicas comunes Importantes

* Capacidad de usar herramientas (busqueda web)

## Propietarios

### ChatGPT

* Direccion : https://chatgpt.com/
* Puntos Destacado
   * Emular la conversacion humana
   * Memoria
      * Cierto conocimiento de la persona con la que esta hablando
   * La personalizacion
      * Instrucciones personalizas

#### Memoria

* Para ver que sabe de mi ChatGPT

```
En base a tu conomiento sobre mi, haceme un roast
```
* Si hacen click en nombre de usuario..(Abajo a la izquierda) y luego personalizacion...
* Podes en todo momento dentro de chatGPT decirle "Quiero que te acuerdes/memorices eso..."


#### Instrucciones Personalizadas

* En la partede personalizacion se le pueden carga instrucciones personalizadas

```
Queiro que respondas en rima. Todo lo que respondes debe ser en rima. No se aceptan textos que no rimen de tu parte
```

---

# Gemini

* El modelo de Google
      * https://gemini.google.com/app
* Puntos fuertes
   * Busca dar informacion basada en hechos (conocimiento Factico)
      * Pensar que google es un buscador de informacion y busca enriquecer las busqeudas con Inteligencia Artificial
   * MODO INVESTIGACION
      * Busca en muchas paginas de internet (+100) y elabora un informe
      * Hasta 3 investigaciones gratuitas por mes
      * (Hoy en dia el modo investigacion no es exclusivo de Gemini pero fue el primero que lo invento)

<img width="912" height="591" alt="image" src="https://github.com/user-attachments/assets/03e748dd-55db-434d-8741-78d0fc27037b" />

   * Integracion con el ecosistema de Google (Google Flights, Google Hotels, google Sheets, Google Calendar)
      * Google Calendar
         * "Creame un evento hoy a las 16:30 hasta las 18:00 que sea "Llevar a mi madre al medico"
      * Google Fights y Google Hotels
         * "Planificame con hotel y vuelos un fin de semana en Paris desde Madrid. Utiliza Google hotels y Google flights"
     


## Open Source


# Prompt Engineering

## Tips

* Utilizar ChatGPT para que me mejore los prompts

* Prompt Original

```
Tengo este prompt para el modo investigacion de gemini "Rubro construccion. Situacion geopolitica. Variacion de precios de materiales en proyectos de mas de 6 meses. Dada la situacion actual y la situaicon geopolita global quiero un estudio que refleje como impacta el tema de energia, guerra y demas en los precios de los materiales que se usan en contruccion para optimizar la planificacion en lo que es compras. Cuando conviene adelantar compras, cuando no. Que materiaes son mas afectador por la situacio global." mejoramelo. Devolver el prompt mejorado sin acotar nada mas
este inform es para alguien de España y eso puede hacer que no sea relevante lo que el iforme me contesta. En particular para por ejemplo madrid. Identificando tambien proveedores y situaicon regional de Espania y madrid.
```


* Prompt Mejorado

```
Actuá como un analista senior especializado en economía de la construcción, geopolítica y gestión de la cadena de suministro, con foco específico en España.

Necesito un informe profundo, estructurado y accionable sobre el rubro construcción en España, con énfasis en la región de Madrid, enfocado en proyectos con horizonte mayor a 6 meses, que analice cómo la situación geopolítica global actual impacta en la variación de precios de materiales.

El análisis debe contemplar:

1. Contexto macro y geopolítico:

* Impacto de conflictos internacionales (guerras activas, tensiones comerciales, sanciones)
* Influencia del precio de la energía en Europa (electricidad, gas)
* Inflación en la eurozona y políticas del BCE
* Impacto de aranceles, regulaciones ambientales y dependencia energética
* Efecto de la demanda europea y desaceleración/crecimiento regional

2. Contexto específico de España y Madrid:

* Situación del sector construcción en España (demanda, obra pública, vivienda)
* Dinámica de precios de materiales en España en los últimos años
* Particularidades logísticas y de abastecimiento en Madrid
* Dependencia de importaciones vs producción local
* Impacto de fondos europeos y políticas públicas

3. Materiales de construcción:
   Analizar los principales materiales (acero, cemento, hormigón, aluminio, cobre, madera, vidrio, plásticos, etc.) y detallar:

* Nivel de sensibilidad a factores geopolíticos
* Dependencia energética en su producción
* Dependencia de importaciones
* Volatilidad histórica reciente en España
* Riesgo proyectado a 6–12 meses

4. Clasificación estratégica:
   Agrupar materiales según:

* Alta volatilidad / riesgo
* Riesgo medio
* Baja volatilidad
  Justificar claramente cada categoría en el contexto español.

5. Proveedores y mercado local:

* Identificar principales proveedores y distribuidores en España y Madrid
* Diferenciar entre grandes proveedores industriales vs distribuidores locales
* Evaluar estabilidad de precios, disponibilidad y poder de negociación
* Analizar riesgos de desabastecimiento o dependencia de ciertos proveedores

6. Estrategia de compras:
   Desarrollar recomendaciones concretas para España/Madrid:

* Cuándo conviene adelantar compras
* Cuándo conviene esperar
* Estrategias de cobertura (stock, contratos a plazo, diversificación)
* Cómo negociar con proveedores en contextos inflacionarios
* Cómo reducir exposición a materiales volátiles

7. Escenarios futuros:
   Plantear al menos 3 escenarios:

* Optimista (normalización energética/geopolítica)
* Base
* Pesimista (escalada de conflictos / energía cara)
  Y explicar cómo impacta cada uno en costos y decisiones de compra.

8. Formato de salida:

* Explicaciones claras, didácticas y orientadas a negocio
* Tablas comparativas y matrices de riesgo
* Insights concretos (evitar generalidades)
* Enfoque práctico para toma de decisiones en planificación de compras

El objetivo es obtener un informe que permita optimizar la estrategia de compras en proyectos de construcción en España (especialmente Madrid), minimizando el riesgo ante la volatilidad global y local.

```


# Herramientas

## Text-to-Speech : Natural Readers

> https://www.naturalreaders.com/

* Esta herramienta me lee un texto
* Por ejemplo en el auto, el tren, mientras voy a correr puedo irhaciendoque lia me lea un texto extenso
* Funciona en el mobil
* Puntaje : 8/10
