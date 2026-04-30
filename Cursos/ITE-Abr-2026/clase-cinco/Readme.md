# Clase Cinco - 30 de Abril del 2026

# Repaso

* Prompt Engineering
  * Patrones de Prompting
    * Interaccion
    * Persona / Rol
    * Personalizacion de Salida
      * JSON, XML : Cuestiones Tecnicas
      * HTML : Util para imprimir como pdf con formato
      * CSV : Para exportar datos a excel
      * Markdown : Para excribir una plantilla en el formato exacto que quiero la respuesta y mantener el formato en Word al copiar
      * Mermaid : Para generar Graficos
* Herramientas
  * Napkin : Para enriquecer un texto con diagramas

# Personalizacion de salida

* Formatos de Salida
  * Lenguaje de programacion
    * Hay un lenguaje de programacion que se llama Python
    * Python lo que tiene es un monton de librerias
      * https://matplotlib.org/
      * Miren los graficos de ejemplos que trae
        * https://matplotlib.org/stable/gallery/index.html#
    * ChatGPT puede ejecutar codigo Python sin salir del Chat (no me acuerdo si la version gratuita lo permite)

```
Tengo estas facturas :"[FACTURAS DE LA CLASE PASADA] [O IMPORTAR UN EXCEL ADJUNTO]"
Armame en python con MatPlotLib un grafico "Bar chart with labels" donde se vea el gasto mes a mes diferenciado en color las distintas categorias por mes. Inlcuime la previsulaizacion en este chat.
```

* Genero este grafico

<img width="746" height="505" alt="image" src="https://github.com/user-attachments/assets/61f352ce-964e-4a19-828f-cbbfc3b46450" />


* Tambien funciona en Claude (que es muy fiable para el analisis de datos)

<img width="2360" height="1166" alt="facturas_zed_chart" src="https://github.com/user-attachments/assets/702034f8-4524-4cfc-9f89-56aae1fa93a4" />

# Uso de Herramientas

## Analisis de Datos con Copilot en Excelo

* Abrir un documento de Excel
* Pegarle el CSV a copilot para que lo importe

```csv
factura,fecha,proveedor,categoria,detalle,monto,subtotal,iva,total
ZED-001,2025-01-15,Constructora Orbital SL,Materiales,Movimiento de suelo,98450,118650,24916.5,143566.5
ZED-001,2025-01-15,Constructora Orbital SL,Servicios,Alquiler excavadora cuántica,12300,118650,24916.5,143566.5
ZED-001,2025-01-15,Constructora Orbital SL,Servicios,Estudio geotérmico avanzado,7900,118650,24916.5,143566.5

ZED-002,2025-02-14,Hormigones del Futuro SA,Materiales,Hormigón reforzado,210000,444000,93240,537240
ZED-002,2025-02-14,Hormigones del Futuro SA,Materiales,Estructura de titanio ligero,145000,444000,93240,537240
ZED-002,2025-02-14,Hormigones del Futuro SA,Mano de obra,Mano de obra especializada,89000,444000,93240,537240

ZED-003,2025-03-18,Ingeniería Atlas,Servicios,Diseño estructural avanzado,75000,135000,28350,163350
ZED-003,2025-03-18,Ingeniería Atlas,Servicios,Simulación sísmica,32000,135000,28350,163350
ZED-003,2025-03-18,Ingeniería Atlas,Servicios,Supervisión técnica,28000,135000,28350,163350

ZED-004,2025-04-16,Materiales Europa,Materiales,Ladrillos inteligentes,88000,163500,34335,197835
ZED-004,2025-04-16,Materiales Europa,Materiales,Mortero autonivelante,21500,163500,34335,197835
ZED-004,2025-04-16,Materiales Europa,Mano de obra,Mano de obra,54000,163500,34335,197835

ZED-005,2025-05-15,Techos Globales SL,Materiales,Cubierta termo-reactiva,120000,202000,42420,244420
ZED-005,2025-05-15,Techos Globales SL,Servicios,Impermeabilización avanzada,44000,202000,42420,244420
ZED-005,2025-05-15,Techos Globales SL,Mano de obra,Instalación,38000,202000,42420,244420

ZED-006,2025-06-17,ElectroNova,Materiales,Cableado inteligente,67000,197000,41370,238370
ZED-006,2025-06-17,ElectroNova,Materiales,Panel central IA,89000,197000,41370,238370
ZED-006,2025-06-17,ElectroNova,Mano de obra,Instalación,41000,197000,41370,238370

ZED-007,2025-07-15,AquaSystems,Materiales,Tuberías autorreguladas,54000,166000,34860,200860
ZED-007,2025-07-15,AquaSystems,Materiales,Sistema de reciclaje de agua,73000,166000,34860,200860
ZED-007,2025-07-15,AquaSystems,Mano de obra,Instalación,39000,166000,34860,200860

ZED-008,2025-08-14,Revestimientos Premium,Materiales,Revestimiento nano-cerámico,61000,142000,29820,171820
ZED-008,2025-08-14,Revestimientos Premium,Materiales,Pintura inteligente,45000,142000,29820,171820
ZED-008,2025-08-14,Revestimientos Premium,Mano de obra,Mano de obra,36000,142000,29820,171820

ZED-009,2025-09-16,Pisos Infinity,Materiales,Piso auto-limpiante,98000,158000,33180,191180
ZED-009,2025-09-16,Pisos Infinity,Materiales,Adhesivos industriales,18000,158000,33180,191180
ZED-009,2025-09-16,Pisos Infinity,Mano de obra,Instalación,42000,158000,33180,191180

ZED-010,2025-10-15,Carpintería Nova,Materiales,Puertas acústicas premium,72000,221000,46410,267410
ZED-010,2025-10-15,Carpintería Nova,Materiales,Ventanas inteligentes,110000,221000,46410,267410
ZED-010,2025-10-15,Carpintería Nova,Mano de obra,Instalación,39000,221000,46410,267410

ZED-011,2025-11-14,Iluminación Lux,Materiales,Sistema lumínico adaptativo,64000,131000,27510,158510
ZED-011,2025-11-14,Iluminación Lux,Materiales,Sensores inteligentes,38000,131000,27510,158510
ZED-011,2025-11-14,Iluminación Lux,Mano de obra,Instalación,29000,131000,27510,158510

ZED-012,2025-12-12,Urbanismo Verde,Servicios,Jardinería bio-sintética,57000,177000,37170,214170
ZED-012,2025-12-12,Urbanismo Verde,Materiales,Cerramiento perimetral,84000,177000,37170,214170
ZED-012,2025-12-12,Urbanismo Verde,Mano de obra,Mano de obra,36000,177000,37170,214170
```

* Generar un grafico con copilot

```
Generame otro libro donde se vea un grafico pivoteable para poder analizar los gastos por mes y por categoria
```

# Herramientas

# Generacion de Presentaciones

* Habiamos visto la generacion de presetaciones dentro de Qwen como herramienta especializada
* Mejor herrmienta hoy
   * Gamma
     * https://gamma.app/signup?r=cjucljp9heegmkv
   *  No solo genera presentaciones sino tambien es un editor tipo power point
 
* Prompt usadp
```
Crea una presentación profesional, moderna y visualmente atractiva para un proyecto ficticio educativo de desarrollo inmobiliario en Madrid, orientado a atraer inversores.

Contexto del proyecto: Se trata de un desarrollo inmobiliario innovador en Madrid llamado "Residencial Horizonte Madrid", un complejo de viviendas premium sustentables con enfoque en tecnología, eficiencia energética y alta rentabilidad. El proyecto está estratégicamente ubicado en una zona de alto crecimiento urbano, con excelente conectividad, cercanía a centros comerciales, educativos y transporte público.

Objetivo de la presentación: Convencer a potenciales inversores de financiar el proyecto, destacando rentabilidad, seguridad, innovación y oportunidad de mercado.



Claim atractivo (ej: “Invertí en el futuro de Madrid”)

Llamado a la acción

“Sumate como inversor”

Beneficios exclusivos por inversión temprana
```

* Generamos esta prsentacion:
  * https://gamma.app/docs/Invierte-en-el-futuro-de-Madrid-aumjexnqe9mh691
* Y esta landing
  * https://residencial-horizonte-ma-12qt21b.gamma.site/
