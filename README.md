<a href="#">
    <img src="https://javier.rodriguez.org.mx/itesm/2014/tecnologico-de-monterrey-black.png" alt="ITESM" title="ITESM" align="right" height="60" />
</a>

# Detección de noticias falsas 📰

## Descripción del proyecto

El proyecto presenta un detector de noticias falsas con aprendizaje automático, en el cual se busca hacer un preprocesado de datos obtenidos de un dataset de Kaggle para su posterior clasificación binaria (verdadero o falso).

## Descripción del Dataset

Es un conjunto de datos creado para practicar la detección de noticias falsas mediante técnicas de aprendizaje automático y procesamiento de lenguaje natural. Contiene 20,000 artículos con etiquetas que indican si son reales o falsos (incluye metadatos). Aproximadamente un 5% de los datos presentan valores faltantes para simular desafíos reales con información incompleta.

- title - El titular del artículo
- text - El cuerpo completo de la noticia
- subject - La categoría o tema (por ejemplo, política, noticias mundiales, etc.)
- date - La fecha de publicación


# Proceso

## Obtener, generar o aumentar un set de datos.

El Dataset utilizado para el proyecto fue obtenido en la plataforma Kaggle. Posteriormente se almacenó en una carpeta de Google Drive para su manipulación dentro del modelo de Machine Learning (ML).

## Preprocesado y data splitting de Entrenamiento y Validación.

De forma manual, se separó la información contenida en el dataset para entrenar, validar y probar el modelo de ML.

-   Entrenamiento: 80%
-   Prueba: 20%

## Técnicas de escalamiento para aumentación y preprocesado

Se realizó la vectorización (TF-IDF) para eliminar palabras comunes en inglés y descartar palabras demasiado frecuentes del texto para manejarlo de una forma más eficiente. Se ajusta el vectorizador al conjunto de entrenamiento (X_train) y se transforma este conjunto en una matriz numérica basada en TF-IDF.

También se hizo un escalamiento debido a que es una **matriz dispersa** en la que la mayoría de los valores son ceros (como las que suelen generarse al usar representaciones como TF-IDF en procesamiento de texto).

## Resultados

[Ver el reporte de resultados obtenidos](Resultados_btenidos.pdf)

## Autor
Instituto Tecnológico y de Estudios Superiores de Monterrey

Alan Fernando Razo Peña - alanrazo2000@hotmail.com

## Bibliografía

[1] P. Kumar, P. Suthanthiradevi, C. A. Stephen, E. Abishek B, S. Sivakumar, and M. Mathiyarasu, “Analysis and Detection of Fake News Using Machine Learning,” May 2024, doi: 10.1109/aiiot58432.2024.10574761

[1]
I. Jahan et al., “Advanced machine learning techniques for fake news detection: A comprehensive analysis,” Magna Scientia Advanced Research and Reviews, vol. 12, no. 2, pp. 203–212, Dec. 2024, doi: 10.30574/msarr.2024.12.2.0198

[1]
S. Velumuru, “Fake News Detection System Using Machine Learning and Deep Learning,” Indian Scientific Journal Of Research In Engineering And Management, Apr. 2024, doi: 10.55041/ijsrem30766
