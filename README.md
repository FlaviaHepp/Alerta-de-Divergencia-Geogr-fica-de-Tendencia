# 🌍Alerta de Divergencia Geográfica de Tendencia

## 📌Descripción del proyecto

Este proyecto implementa una alerta SQL para detectar divergencias de tendencia entre regiones geográficas, comparando la evolución temporal de una métrica clave entre distintas zonas.

El objetivo es identificar comportamientos anómalos o desalineados entre regiones, que pueden indicar:
- Cambios estructurales en la demanda
- Problemas operativos locales
- Errores de datos
- Riesgos comerciales o financieros

## 🎯Objetivos del proyecto

- Detectar diferencias significativas en la tendencia temporal de una métrica entre regiones.
- Comparar el desempeño regional contra un benchmark (promedio, región líder, histórico).
- Generar alertas tempranas para análisis y toma de decisiones.
- Automatizar controles geográficos mediante SQL.
- Facilitar el monitoreo continuo de KPIs regionales.

## 🏢Contexto de negocio

En organizaciones con presencia regional o internacional:
- Las métricas deberían evolucionar de forma relativamente consistente entre regiones comparables.

Una divergencia sostenida puede indicar:
- Caída de performance local
- Impacto de políticas/regulación regional
- Fallas operativas o logísticas
- Oportunidades de crecimiento diferencial

📌 Este tipo de alertas es clave para:
- BI & Analytics
- Planeamiento comercial
- Riesgo operativo
- Control de gestión
- Auditoría de datos

## 🧠Lógica de la alerta

La consulta SQL:
- Agrega la métrica por región y período.
- Calcula la tendencia temporal (variación absoluta o porcentual).

Compara cada región contra:
- El promedio global
- Otras regiones
- Un baseline histórico
- Detecta divergencias significativas cuando la diferencia supera un umbral.
- Marca las regiones y períodos afectados.

📌 El enfoque es flexible y configurable para distintos KPIs y ventanas temporales.

## 📊Ejemplos de divergencia detectada

- Una región con crecimiento negativo sostenido mientras el resto crece.
- Caídas abruptas locales no replicadas en otras zonas.
- Crecimientos atípicos que podrían indicar errores de carga o eventos excepcionales.
- Desalineación prolongada respecto al promedio global.

## 🛠️Tecnologías utilizadas

SQL

Compatible con:
- PostgreSQL
- BigQuery
- SQL Server
- Oracle
- MySQL (con ajustes menores)

## 📁Estructura del proyecto

├── alerta_de_divergencia_geografica_de_tendencia.sql
└── README.md

## ▶️Cómo utilizar la alerta

Abrir el archivo alerta_de_divergencia_geografica_de_tendencia.sql.

Configurar:
- Tabla fuente
- Métrica de interés
- Dimensión geográfica
- Ventana temporal
- Umbrales de divergencia
- Ejecutar la consulta en el motor SQL.
- Integrar resultados con:
- Dashboards
- Alertas automáticas
- Reportes ejecutivos

## 🚀Posibles extensiones

- Clasificar alertas por nivel de severidad.
- Guardar alertas históricas en una tabla.
- Integrar con herramientas de orquestación (Airflow, dbt).
- Visualizar divergencias en mapas o dashboards.
- Combinar con alertas de volumen o calidad de datos.

## 👤Autora

Flavia Hepp
Proyecto de SQL avanzado aplicado a monitoreo de tendencias y análisis geográfico.

***
🌍📊 **¿Todos los mercados suben… pero uno no? Ojo con esto.**

En análisis cuantitativo muchas veces miramos activos individuales… pero el verdadero insight aparece cuando levantamos la mirada.

Hoy estuve trabajando en un detector de **divergencias geográficas de tendencia**, y el resultado es bastante potente 👇

La idea es simple pero reveladora:

👉 Medir qué porcentaje de acciones está en tendencia alcista (Precio > SMA 200)
👉 Comparar cada país contra el promedio global
👉 Detectar desvíos significativos

---

💡 **¿Por qué importa esto?**

Porque los mercados globales suelen moverse con cierta sincronía.
Cuando un país se “desacopla”, algo está pasando:

* Cambios macroeconómicos
* Riesgo político
* O… una oportunidad antes de que el mercado lo reconozca

---

🚨 **Ejemplo real del insight:**

* USA: 90% de acciones en tendencia alcista
* Global: 85%
* País X: 45%

➡️ Esto no es ruido. Es una señal.

---

📈 Este tipo de análisis permite:

* Detectar mercados rezagados (posibles oportunidades)
* Identificar sobrecalentamientos
* Mejorar decisiones de asset allocation global
* Anticipar cambios macro antes que sean evidentes

---

🧠 Lo interesante es cómo algo tan simple como una SMA 200, cuando se escala a nivel global, se convierte en un indicador macro muy potente.

A veces no hace falta más complejidad… sino mejor contexto.

---

Si trabajás con datos de mercado o estás explorando estrategias cuantitativas, este tipo de insights abre muchas puertas 🚀

¿Te interesan este tipo de señales? Puedo compartir más ideas de este estilo.

