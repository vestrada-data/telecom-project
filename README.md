# Análisis de una empresa de telecomunicaciones  - Sprint 7

Este repositorio contiene el análisis del caso ConnectaTel.



Trabajarás con tres datasets principales de información, relacionadas con usuarios, actividad y planes del servicio de telecomunicaciones:

**plans.csv:** Catálogo de planes con sus precios y beneficios. <br>
**users_latam.csv:**  Información de cada usuario (datos personales, plan, fecha de registro, churn). <br>
**usage.csv:** Actividad generada por los usuarios: llamadas, mensajes, duración, longitud. <br>

El dataset connectaTel` incluye  40,000 registros con valores faltantes, sentinels, outliers y problemas de calidad diseñados para simular datos reales del retail. :contentReference[oaicite:2]{index=2}

## 📂 Contenido del repositorio

- `notebooks/everpeak.ipynb`
  → Notebook principal con limpieza, EDA, distribuciones, outliers y conclusiones.

## ▶ Cómo abrir el notebook en Google Colab

Haz clic en el siguiente botón:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://github.com/vestrada-data/everpeak-analysis/blob/main/everpeak.ipynb)

O:

1. Abre el archivo `.ipynb` en GitHub
2. Haz clic en **Open in Colab**

## 📘 Cómo reproducir el análisis

1. Abre `notebooks/everpeak.ipynb`
2. Ejecuta las celdas en orden
3. El notebook carga automáticamente el dataset desde `/data/` o desde un enlace público (según corresponda)

## 🧠 Objetivo del análisis

- Identificar problemas de calidad de datos
- Construir un pipeline de limpieza reproducible
- Analizar comportamientos, distribuciones y outliers
- Generar insights para el equipo de Estrategia e
