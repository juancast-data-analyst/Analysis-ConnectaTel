# Analysis--ConnectaTel – Sprint 7

Este repositorio contiene el análisis completo realizado durante el Sprint 7 del caso ConnectaTel, empresa de telecomunicaciones en Latinoamérica.
El proyecto trabaja con tres datasets (plans.csv, users.csv, usage.csv) que incluyen información de 4,000 clientes y 40,000 registros de uso del año 2024, con valores faltantes, centinelas, outliers y problemas de calidad diseñados para simular datos reales del sector telecomunicaciones.

## 📂 Contenido del repositorio
📦 connectatel-analysis/
├── 📓 notebooks/
│   └── S7_Project-ConnectaTel.ipynb  → Notebook principal con carga, limpieza, EDA, segmentación y análisis ejecutivo
├── 📊 data/
│   ├── plans.csv           → Catálogo de planes (Básico y Premium)
│   ├── users.csv           → Información de 4,000 clientes
│   └── usage.csv           → 40,000 registros de uso (llamadas, mensajes, datos)
├── 📄 outputs/
│   └── Analisis_Ejecutivo_ConnectaTel.md  → Reporte ejecutivo con insights y recomendaciones
└── 📖 README.md            → Este archivo

## ▶️ Cómo abrir el notebook en Google Colab
Haz clic en el siguiente botón:
Mostrar imagen

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](S7_Project_ConnectaTel.ipynb)

O manualmente:

Abre el archivo S7_Project-ConnectaTel.ipynb en GitHub
Haz clic en Open in Colab (botón superior)
Ejecuta las celdas en orden secuencial


## 📘 Cómo reproducir el análisis
Google Colab (recomendado)

Haz clic en el badge de Colab arriba
Ejecuta todas las celdas: Runtime > Run all
Los datasets se cargan automáticamente desde la carpeta /data/


## 🧠 Objetivo del análisis
Como analista de datos en ConnectaTel, el objetivo es evaluar el comportamiento de los clientes para:

✅ Identificar problemas de calidad de datos (centinelas, nulos, fechas inválidas)
✅ Construir un perfil estadístico del uso (llamadas y mensajes) por cliente y por segmentos demográficos.
✅ Segmentar clientes por edad y nivel de uso para personalización de ofertas
✅ Detectar outliers y patrones de uso extremo (power users)
✅ Analizar y Visualizar distribuciones de llamadas, mensajes y minutos consumidos
✅ Generar insights accionables para el equipo de Marketing y Producto


## 🛠️ Tecnologías utilizadas

Python 3.x
Pandas → Manipulación y limpieza de datos
NumPy → Cálculos numéricos y estadísticas
Matplotlib & Seaborn → Visualizaciones (histogramas, boxplots, gráficos de barras)
Jupyter Notebook → Entorno de desarrollo interactivo


## 📈 Estructura del análisis
El notebook sigue un flujo estructurado en 8 pasos:

### 🧩 Carga y exploración inicial

Importación de 3 datasets
Revisión de estructura (.shape, .info(), .head())


### ⚠️ Identificación de problemas de calidad

Detección de nulos, centinelas y valores inválidos
Análisis de fechas fuera de rango


### 🧹 Limpieza de datos

Reemplazo de centinelas (-999, "?")
Corrección de fechas imposibles
Justificación de nulos MAR


### 📊 Estadísticas agregadas por usuario

Resumen de uso: mensajes, llamadas, minutos
Creación de tabla user_profile


### 📉 Visualización de distribuciones

Histogramas por edad y uso
Identificación de patrones y asimetrías


### 🔍 Detección de outliers

Método IQR (Rango Intercuartílico)
Decisión: mantener outliers de negocio


### 🎯 Segmentación de clientes

Por nivel de uso (Bajo/Medio/Alto)
Por edad (Joven/Adulto/Adulto Mayor)


### 📝 Análisis ejecutivo

Insights accionables
Recomendaciones priorizadas

👤 Autor
Juan Castelblanco - Analista de Datos - ConnectaTel
Sprint 7 - Análisis de Comportamiento de Clientes 2024

📝 Licencia
Este proyecto es de uso educativo y forma parte del programa de análisis de datos.
