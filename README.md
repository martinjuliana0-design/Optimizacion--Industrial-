# Análisis de Optimización de Calidad y Mantenimiento Industrial

---
# Contexto 

En entornos de manufactura de alta demanda, la falta de visibilidad sobre la relación entre el mantenimiento y la calidad genera pérdidas económicas significativas. Este proyecto analiza el comportamiento operativo de una planta industrial que produce diversas líneas de productos (Automotive, Textiles, Electronics, etc.) en tres turnos rotativos. El desafío principal fue identificar por qué ciertas máquinas mantienen niveles altos de defectos a pesar de la inversión en mantenimiento y cómo las brechas en la programación de servicios impactan el costo final del desperdicio.

---
# Objetivos 

* Identificar Causas Raíz: Localizar las máquinas y turnos con mayor concentración de fallas mediante herramientas de Inteligencia Artificial.
* Evaluar la Eficiencia del Mantenimiento: Determinar si la distribución de horas de servicio actual está reduciendo efectivamente la tasa de defectos.
* Cuantificar el Impacto Financiero: Traducir las métricas de ingeniería (piezas defectuosas) a impacto económico ($) para el negocio.
* Proponer Acciones Preventivas: Establecer recomendaciones basadas en datos para optimizar la calidad del proceso.

---
# Metodología 

Para el desarrollo de este análisis se siguió un flujo de trabajo de análisis de datos profesional:

1. Exploración y Limpieza: Tratamiento del dataset para asegurar consistencia en las categorías de productos, turnos y registros de máquinas.
2. Modelado de Datos: Estructuración de tablas en Power BI para permitir un filtrado dinámico por año, mes y tipo de producto.
3. Análisis de Causa Raíz: Implementación de un Esquema Jerárquico (Decomposition Tree) para desglosar los defectos desde el turno hasta la variable técnica específica.

---
# Hipótesis

La implementación de un programa de mantenimiento preventivo basado en el análisis de datos históricos reducirá el tiempo de inactividad de las máquinas en un 15% y disminuirá los defectos de producción en un 10% durante el primer semestre de aplicación." Variable independiente: Frecuencia de mantenimiento preventivo. Variable dependiente: Tasa de defectos y horas de inactividad

---
# KPIs Analizados 

El dashboard se sustenta en métricas calculadas específicamente para reflejar el estado de la planta:

* Volumen de producción
* % Producto no conforme
* Eficacia de mantenimiento
* Impacto economico

---
# Tecnologías 

* Power BI Desktop: Como herramienta principal de visualización y modelado.
* DAX (Data Analysis Expressions): Utilizado para la creación de todas las métricas de negocio y lógica de indicadores.
* Análisis Avanzado: Uso de visuales de IA nativos de Power BI para detección de factores influyentes.

---
# Dashboard 

El informe final se divide en tres secciones estratégicas:
1. Panel de Control (Cabecera): Tarjetas de alto nivel para monitoreo inmediato de producción y costos.
2. Análisis Temporal y Operativo: Comparativa de % de defectos vs. producción y desglose de fallas por turno.
3. Módulo de Diagnóstico: Matriz de rendimiento por máquina y esquema de descomposición para la identificación de la causa raíz.

---
# Conclusiones

Tras el análisis exhaustivo, se obtuvieron las siguientes conclusiones accionables:
* Ineficiencia en Mantenimiento: Se detectó que la Máquina 2 recibe una alta inversión de horas (110.38h) pero mantiene una de las tasas de defectos más altas (195), lo que sugiere que el mantenimiento actual es reactivo y no preventivo.
* Punto Crítico Detectado: El turno Noche (Night) en la línea de Textiles presenta la mayor vulnerabilidad. El análisis de IA confirmó que la Máquina 8 dispara sus errores cuando el mantenimiento llega a 0 horas.
* Impacto Económico Proyectado: El análisis identifica un costo acumulado de $92,220 USD durante el bienio 2024-2025. Implementar una redistribución del mantenimiento preventivo en las máquinas críticas (19, 2 y 16) permitiría una reducción estimada del 10% en la tasa de defectos, lo que se traduce en un ahorro de $9,222 USD para el próximo ciclo de 24 meses (aprox. $4,600 USD anuales).

---
# Recomendación

Redistribuir las horas de mantenimiento de máquinas estables hacia las críticas y establecer protocolos de inspección obligatorios al inicio del turno noche para mitigar el riesgo de piezas no conformes.
