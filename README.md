### Análisis de una empresa de telecomunicaciones  - Sprint 7

Este repositorio contiene el análisis del caso ConnectaTel.

 ## 🎯 Objetivo General

El objetivo es identificar patrones de uso, detectar comportamientos atípicos y comprender qué segmentos de clientes muestran necesidades diferenciadas, con el fin de optimizar la oferta comercial y mejorar la experiencia del usuario.

Trabajaremos con tres datasets principales de información, relacionadas con usuarios, actividad y planes del servicio de telecomunicaciones:

*plans.csv:*  Catálogo de planes con sus precios y beneficios. <br>
*users_latam.csv:*  Información de cada usuario (datos personales, plan, fecha de registro, churn). <br>
*usage.csv* Actividad generada por los usuarios: llamadas, mensajes, duración, longitud. <br>

Contamos con  40,000 registros con valores faltantes, sentinels, outliers y problemas de calidad diseñados para simular datos reales.

## 📂 Contenido del repositorio

- `notebooks/connectaTel.ipynb`
  → Notebook principal con limpieza, EDA, distribuciones, outliers y conclusiones.

  ## 🧠 Objetivo del análisis

- Identificar problemas de calidad de datos
- Limpieza  básica (reemplazar sentinels, convertir fechas, impitar o marcar NA)
- Summary statistics
- Visualización & outliers
- Segmentación
- Analizar comportamientos, distribuciones y outliers
- Generar insights para Stakeholders
  
## ▶ Cómo abrir el notebook en Google Colab

Haz clic en el siguiente botón:

[![Open In Colab](https://colab.research.google.com/drive/11yrhUvfrQaq69nP1ZmriXNMOP2RkErim#scrollTo=ee7c578d)

O:

1. Abre el archivo `connectaTel.ipynb` en GitHub
2. Haz clic en **Open in Colab**

## 📘 Cómo reproducir el análisis

1. Abre `notebooks/connectaTel.ipynb`
2. Ejecuta las celdas en orden
3. El notebook carga automáticamente el dataset desde `/data/` o desde un enlace público (según corresponda)


