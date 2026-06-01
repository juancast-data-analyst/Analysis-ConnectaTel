# ConnectaTel – Análisis de Comportamiento de Clientes - Proyecto Sprint 7

Este repositorio contiene el análisis realizado durante el Sprint 7 del proyecto ConnectaTel, una empresa de telecomunicaciones con operaciones en México y Colombia.

Los datasets `plans`, `users_latam` y `usage` incluyen información de **4,000 clientes** y **40,000 registros de uso** (llamadas y mensajes) del año 2024, con valores faltantes, sentinels, outliers y problemas de calidad diseñados para simular datos reales del sector telecomunicaciones.

---

## 📂 Contenido del repositorio

- `notebooks/S7_Project-ConnectaTel.ipynb`
  → Notebook principal con carga de datos, limpieza, estadísticas descriptivas, detección de outliers, segmentación de clientes y conclusiones ejecutivas.

- `data/plans.csv`
  → Catálogo de planes (precio mensual, minutos incluidos, GB, costos por excedente).

- `data/users_latam.csv`
  → Información de clientes: edad, ciudad, fecha de registro, plan contratado y fecha de churn.

- `data/usage.csv`
  → Detalle de uso real: llamadas (duración en minutos) y mensajes (longitud en caracteres).

---

## ▶️ Cómo abrir el notebook en Google Colab

Haz clic en el siguiente botón:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/juancast-data-analyst/Analysis-ConnectaTel/blob/main/S7_Project_ConnectaTel.ipynb)

O manualmente:

1. Abre el archivo `.ipynb` en GitHub
2. Haz clic en **Open in Colab**

---

## 📘 Cómo reproducir el análisis

1. Abre `notebooks/S7_Project-ConnectaTel.ipynb` en Google Colab o Jupyter
2. Sube los tres archivos CSV a la carpeta `/datasets/` (o ajusta las rutas según tu entorno)
3. Ejecuta las celdas en orden de arriba hacia abajo
4. El notebook está estructurado en 8 pasos secuenciales; cada uno tiene instrucciones y celdas de validación

---

## 🧠 Objetivos

### Objetivo del análisis

Evaluar el comportamiento de los clientes de ConnectaTel para identificar patrones de uso, detectar comportamientos atípicos y comprender qué segmentos muestran necesidades diferenciadas, con el fin de optimizar la oferta comercial y mejorar la experiencia del usuario.

## Objetivo del análisis

- Integrar y limpiar datos provenientes de tres fuentes distintas
- Detectar problemas de calidad: nulos, sentinels, fechas fuera de rango y tipos incorrectos
- Construir un perfil estadístico del uso (llamadas y mensajes) por cliente y por segmentos demográficos
- Identificar outliers y comportamientos atípicos mediante métodos estadísticos y visuales
- Segmentar clientes por edad, país y nivel de consumo
- Generar insights y recomendaciones comerciales accionables para el equipo de ConnectaTel

---

## 🛠️ Herramientas utilizadas

- Python 3.9
- `pandas` · `numpy` · `matplotlib` · `seaborn`
- Jupyter Notebook / Google Colab
  
---

## 📊 Etapas del análisis

| Paso | Descripción |
|------|-------------|
| 1 | Carga y exploración de los 3 datasets |
| 2 | Identificación de problemas de calidad de datos |
| 3 | Limpieza: sentinels, fechas, nulos e imputación |
| 4 | Estadísticas descriptivas por variable |
| 5 | Visualización: histogramas y boxplots |
| 6 | Segmentación por edad, país y nivel de uso |
| 7 | Conclusiones e insights ejecutivos |
| 8 | Publicación del notebook y README en GitHub |

---

## 💡 Principales hallazgos

- El **73.6% de los usuarios** tiene un perfil de uso medio, sin un plan adecuado para sus necesidades reales
- Solo el **19% de la base** corresponde a clientes menores de 30 años, lo que representa una oportunidad de captación
- Se detectaron **~150 usuarios con comportamiento atípico** (alto consumo fuera de rango normal) con alto riesgo de churn
- Los datos sucios ocultaban que la edad promedio real del cliente es **13 años mayor** que lo registrado inicialmente

---
👤 Autor
Juan Castelblanco - Analista de Datos - ConnectaTel
Sprint 7 - Análisis de Comportamiento de Clientes 2024

📝 Licencia
Este proyecto es de uso educativo y forma parte del programa de análisis de datos.

*Fecha de análisis: Febrero 2026 | ConnectaTel Data Analytics Team*
