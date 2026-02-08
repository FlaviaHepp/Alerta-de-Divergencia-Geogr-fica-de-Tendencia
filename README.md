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
