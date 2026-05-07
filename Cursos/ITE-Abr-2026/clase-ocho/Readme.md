# Repaso

* IA Creativa
  * Generacion de Canciones
    * Suno
  * Generacion de Videos
    * Efectos con PikaLabs
* Machine Learning
* Agentes
  * NotebookLM

# NotebookLM

* Me quedaron pendientes los audios y el video
  * Audio
    * https://notebooklm.google.com/notebook/1efbbdd0-23a5-4b9e-9b1d-05c3b5f922d7/artifact/9e039948-0f66-41c8-88d0-e8ee1fa3b0b5?utm_source=nlm_web_share&utm_medium=google_oo&utm_campaign=art_share_1&utm_content=&utm_smc=nlm_web_share_google_oo_art_share_1_
  * Video
    * https://notebooklm.google.com/notebook/1efbbdd0-23a5-4b9e-9b1d-05c3b5f922d7/artifact/29c0035a-316c-45ee-ac30-2bbd37c24de0?utm_source=nlm_web_share&utm_medium=google_oo&utm_campaign=art_share_1&utm_content=&utm_smc=nlm_web_share_google_oo_art_share_1_

# Machine learning

* Repaso de como se usa para predecir datos
* Ejemplo de la construccion para predecir el costo de  construccion final
  * Las primeras filas son datos que ya conozco de proyectos que tuve y la  ultima fila fue datos de un proyecto que se va a hacer

``` markdown
| Metros Cuadrado | Cantidad Personas | Tipo Hormigon | Cantidad Aberturas | Costo Final | Pred:Costo Final |
| :-------------- | :---------------- | :------------ | :----------------- | :---------- | :--------------- |
| 20              | 2                 | 1             | 4                  | 1500        |                  |
| 20              | 1                 | 1             | 10                 | 3000        |                  |
| 20              | 1                 | 1             | 4                  | 1270        |                  |
| 50              | 1                 | 1             | 8                  | 4000        |                  |
| 30              | 2                 | 2             | 2                  | 2000        |                  |
| 20              | 1                 | 1             | 4                  | 1000        |                  |
| 25              | 2                 | 1             | 4                  | 2000        |                  |
| 20              | 2                 | 1             | 4                  | 1500        |                  |
| 20              | 1                 | 1             | 10                 | 3000        |                  |
| 20              | 1                 | 1             | 4                  | 1270        |                  |
| 50              | 1                 | 1             | 8                  | 4000        |                  |
| 30              | 2                 | 2             | 2                  | 2000        |                  |
| 20              | 1                 | 1             | 4                  | 1000        |                  |
| 25              | 2                 | 1             | 4                  | 2000        |                  |
| 20              | 2                 | 1             | 4                  | 1500        |                  |
| 20              | 1                 | 1             | 10                 | 3000        |                  |
| 20              | 1                 | 1             | 4                  | 1270        |                  |
| 50              | 1                 | 1             | 8                  | 4000        |                  |
| 30              | 2                 | 2             | 2                  | 2000        |                  |
| 25              | 1                 | 1             | 2                  |             | 1845-06-01       |
```


# Ai-900 : Azure

* Azure : Es una pataforma (se queda chico) donde podes alquilar un conjunto de serivicios para desplegar nuestras soluciones en la nube
  * Desde el auge de la IA azure incluyo un monton de servicios de IA
  * Gran parte de estos servicios son gratis

* URL
  * https://portal.azure.com/
* Ahi creamos una subscripcion
   * Try it 200 dolares por un mes para usar gratis
     * Te requiere registrarte con la tarjeta de credito
   * Promociones
* Servicios de IA Disponible

## AI Foundry

* Tiene un monton de servicios para sar soporte al desarrollo de soluciones de IA
* Muchos de estos servicios se pueden utilizar de forma gratuita

* Aquí tenés la lista con bullets y sub-bullets:

- Foundry
- Azure OpenAI
  - Te da acceso a muchos LLM inclusive los de OpenAI a un menor costo
- AI Search
  - Indexar documentacion semantica
    - (Ej busco sobre animales y me devuelve manuales de perros)
    - Busco una falla en un calefon en lenguaje muy coloquial y me defuelve manuales tecnicos de gas
- Bot services
    - DEsarrollar un bot de atencion al cliente (integrando por ejemplo con una base de conocimiento con AI Search)
- Computer vision
    - Detectar en un video cuando apatecen personas sin necesidad de tener a alguien mirando todo el tiempo la camara 
- Custom vision
   - Entrenar a modelos que detecten productos defectuosos en una linea de produccion
- Content safety
   - Me ayuda a moderar contenido online sin tener que hacerlo manualmente (insultos, cosas de lugar, etc)
- Document intelligence
   - Me permite digitalizar automaticamente todo lo que se maneja en papel (sacarle una foto a un remito) y pasarlo a texto en un formato estandar
- Face API
  - Se puede utilizar para tomar presentismo o registro automatico en una empresa (quien sale y entra del edificio)
- Health Insights
  - Para centros de salud
- Machine Learning
  - Lo que hicimos en SimpleML for sheets pero cuando trabajo con millones y millones de datos
- Immersive reader
  - PAra usabilidad
- Language service
  - Para analisis automatico de texto en forma economica como por ejemplo reconocer comentarios negativos en google
- Speech service
  - PAra convertir de texto a voz y vos a texto
- **Translator**
  - Para trabajar en diferentes idiomas
