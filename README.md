# Análisis Exploratorio del Dataset Goodbooks-10k 📚

**Autora:** Nerea Curri  
**Proyecto:** EDA (Análisis Exploratorio de Datos) sobre 10.000 libros de Goodreads.  
**Contacto:** nereacurri1@gmail.com

---

## Resumen
Este proyecto realiza un EDA completo del dataset *Goodbooks-10k*.  
Se incluyen: limpieza de datos, análisis univariado, análisis bivariado, detección de outliers, transformación logarítmica para variables de popularidad y una exploración temporal (publicaciones por año).

## Contenido del repositorio
- `EDA_goodreads_Nerea.ipynb` — Notebook principal (Google Colab compatible).  
- `goodreads-eda-nerea.PDF` — Versión exportada en PDF del notebook.  
- `requirements.txt` — Librerías necesarias.  

## Cómo ejecutar
**Opción rápida (recomendada):**  
1. Abrí el notebook en Google Colab: `File > Upload notebook` y subí `EDA_goodreads_Nerea.ipynb` o usá `Open in Colab` si pegás el link.  
2. Ejecutá todas las celdas.

**Opción local:**  
1. Cloná el repo.  
2. `pip install -r requirements.txt`  
3. Abrí el notebook con JupyterLab o Jupyter Notebook.

## Principales hallazgos
- `average_rating` se concentra alrededor de **4.0** (poca dispersión).  
- `ratings_count` y `work_text_reviews_count` son altamente asimétricos; pocos libros concentran la mayoría de interacciones.  
- La transformación `log(1+x)` permite visualizar la masa central y detectar outliers.  
- No existe evidencia de una relación lineal fuerte entre popularidad y rating promedio.

## Próximos pasos sugeridos
- Análisis por género (si el dataset lo permite).  
- Modelado predictivo simple (e.g., predecir si un libro superará X ratings).  
- Sistema de recomendaciones básico (content-based).

