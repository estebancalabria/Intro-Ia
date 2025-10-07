# Clase Dos - 07 de Octubre del 2025

## Repaso

* Diferentes LLM (plataformas)
  * Propietarios
      * ChatGPT
          * Memoria
          * Personalizacion
          * Optimizado para conversaciones amigable
      * Gemini
          * Integrada con la suite de Google
      * Claude
          * Artefactos (Previsualizacion)
  * Open Source

## Conceptos

* Determinismo : La IA no es deterministica. Ante el mismo prompt puede dar resultados diferentes

## LLM 

* Propietarios
  * Gemini
    * Modo Deep Research
      * Activarlo en la parte de herramientas
      * TEngo una cantidad limitada de Investigaciones por Mes en la version Gratuita

## Prompt Engineering

### Tips para prompt Enginerring

- #### **Ultimate Prompting Tip** : Utilizar ChatGPT como escritor de Prompts.

**Actua como un experto en prompt engineering**(1) y **quiero que me redactes el siguiente prompt para Gemini de manera efectiva**(2) : "Haceme una Investigacion exhaustiva sobre criptomonedas, tendencias, alternativas de inversion, precauciones, etc.". **Devolveme el prompt optimizado para copiar y pegar sin acotar nada mas.**(3)

Deglosando el prompt
1. Rol que quiero que tome la IA
2. Objetivo, la tarea concreta que le estoy solicitando
3. Formato de salida esperado

Respuuesta:
'''txt
Eres un/una **analista experto/a en criptomonedas y mercados financieros**. Realizá **una investigación exhaustiva, actualizada y neutral** sobre criptomonedas: tendencias, alternativas de inversión, riesgos y precauciones. Entregá resultados claros, accionables y citados. Usá un lenguaje profesional pero accesible para un público con conocimientos básicos-intermedios en finanzas. Actualizá la información **hasta el 7 de octubre de 2025**.

Requerimientos de contenido y estructura (ordenada y completa):

1. **Resumen ejecutivo (máx. 200 palabras)**: puntos clave, conclusiones principales y recomendaciones rápidas para un inversor con perfil conservador, moderado y agresivo.

2. **Panorama actual del mercado**:

   * Capitalización total del mercado cripto, dominancia de Bitcoin y Ethereum, y principales tendencias macro (DeFi, NFTs, L2, Web3, stablecoins, CBDCs, zk-rollups, etc.).
   * Datos cuantitativos recientes (precios, variaciones 24h/7d/30d, volúmenes) y señales macro relevantes (tasas, inflación, políticas regulatorias).

3. **Tendencias tecnológicas y de adopción**:

   * Innovaciones técnicas (ej.: rollups, proof-of-stake, sharding, privacidad, interoperabilidad).
   * Casos de uso emergentes y adopción institucional (custodia, ETFs, pagos, soluciones empresariales).

4. **Alternativas de inversión**:

   * Clasificación por perfil de riesgo: (a) Reserva de valor (ej. BTC), (b) Plataformas de contratos inteligentes (ETH, L2s), (c) DeFi (proveedores de liquidez, lending), (d) Stablecoins y yield strategies, (e) Tokens de infraestructura y oráculos, (f) NFTs y metaverso (con aclaración de alto riesgo).
   * Ventajas, desventajas, métricas clave a evaluar (TVL, market cap, volumen, tokenomics, utilidad real, equipo, adopción).

5. **Estrategias prácticas y ejemplos**:

   * Estrategias de asignación (porcentaje sugerido según perfil), estrategias de entrada (DCA, laddering), gestión de riesgos (stop-loss, take-profit, rebalanceo).
   * Ejemplos numéricos ilustrativos.

6. **Precauciones, riesgos y señales de alerta**:

   * Riesgos de mercado, tecnológicos, regulatorios, operativos (custodia/exchanges), deliquidez, rug pulls, y riesgo de contraparte.
   * Lista de "red flags" en proyectos/tokenomics y checklist de due diligence.

7. **Aspectos regulatorios y fiscales**:

   * Panorama global (EE. UU., UE, LatAm) y pasos regulatorios clave hasta la fecha indicada.
   * Consideraciones fiscales generales para inversores minoristas (no dar asesoramiento legal personalizado).

8. **Herramientas y fuentes para seguimiento**:

   * Fuentes y dashboards recomendados (on-chain explorers, агрегadores de datos, informes de exchanges y firmas de research), cómo usarlos y qué métricas vigilar.

9. **Plan de acción de 30/90/365 días**:

   * Acciones concretas a corto, mediano y largo plazo para perfiles conservador/moderado/agresivo.

10. **Resumen final y recomendaciones concretas**:

    * 5 puntos accionables prioritarios y una recomendación de asignación por perfil.

11. **Apéndice técnico y glosario**:

    * Explicación breve de términos clave y métricas on-chain.

Formato de entrega:

* Entregá el informe en **texto estructurado** con encabezados claros y numerados según lo solicitado.
* Al final, incluí **una sección de referencias** con **links y fechas** de las fuentes (mínimo 8 fuentes, priorizando informes oficiales, publicaciones académicas, exchanges reconocidos y medios especializados).
* Proveé además **un bloque JSON** al final con las métricas clave sintetizadas, por ejemplo:

{
  "fecha_actualizacion": "2025-10-07",
  "market_cap_total_usd": ...,
  "dominancia_btc_pct": ...,
  "top_trends": ["DeFi", "zk-rollups", "..."],
  "recomendacion_conservador": {"asignacion_crypto_pct": ..., "instrumentos_recomendados": [...]},
  "recomendacion_moderado": {...},
  "recomendacion_agresivo": {...}
}

Criterios de calidad:

* Explicá supuestos y limitaciones del análisis.
* Señalá claramente cuando se producen estimaciones o inferencias (marcarlas como "estimación").
* Mantené un tono imparcial y evitá consejos financieros personalizados; en su lugar, entregá opciones y criterios para decidir.
* Incluí citas (en línea o al final) con enlaces y fecha de publicación.

Instrucciones finales:

* Si un dato no puede verificarse hasta la fecha indicada, indicá qué se intentó buscar y por qué no fue posible confirmar.
* Resumí todo nuevamente en **un TL;DR de 3 frases** al comienzo del informe.

Comenzá la investigación y entregá el informe siguiendo exactamente esta estructura.

```
- #### Uitlizar el optimizador de prompts de OpenAI

> https://platform.openai.com/chat/edit?models=gpt-5&optimize=true

## Uso de API

## Herramientas de IA

##... Sorpresa...
