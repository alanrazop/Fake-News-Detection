<a href="#">
    <img src="https://javier.rodriguez.org.mx/itesm/2014/tecnologico-de-monterrey-black.png" alt="ITESM" title="ITESM" align="right" height="60" />
</a>

# Detección de noticias falsas 📰

## Descripción del proyecto 
El proyecto presenta un detector de noticias falsas, en el cual se busca hacer un preprocesado de datos obtenidos de un dataset de Kaggle para su posterior clasificación binaria (verdadero o falso).

## Descripción del Dataset
Es un conjunto de datos creado para practicar la detección de noticias falsas mediante técnicas de aprendizaje automático y procesamiento de lenguaje natural. Contiene 20,000 artículos con etiquetas que indican si son reales o falsos (incluye metadatos). Aproximadamente un 5% de los datos presentan valores faltantes para simular desafíos reales con información incompleta.

- title A short headline summarizing the article (around 6 words).
- text The body of the news article (200–300 words on average).
- date The publication date of the article, randomly selected over the past 3 years.
- source The media source that published the article (e.g., BBC, CNN, Al Jazeera). May contain missing values (~5%).
- author The author's full name. Some entries are missing (~5%) to simulate real-world incomplete data.
- category The general category of the article (e.g., Politics, Health, Sports, Technology).
- label The target label: real or fake news.

# Proceso
## Obtener, generar o aumentar un set de datos.
El Dataset utilizado para el proyecto fue obtenido en la plataforma Kaggle. Posteriormente se almacenó en una carpeta de Google Drive para su manipulación dentro del modelo de Machine Learning (ML).

## Preprocesado y data splitting de Entrenamiento y Validación.
De forma manual, se separó la información contenida en el dataset para entrenar, validar y probar el modelo de ML.
* Entrenamiento: 80%
* Prueba: 20%

## Técnicas de escalamiento para aumentación y preprocesado
Se realizó la vectorización (TF-IDF) para eliminar palabras comunes en inglés y descartar palabras demasiado frecuentes del texto para manejarlo de una forma más eficiente. Se ajusta el vectorizador al conjunto de entrenamiento (X_train) y se transforma este conjunto en una matriz numérica basada en TF-IDF.

También se hizo un escalamiento debido a que es una **matriz dispersa** en la que la mayoría de los valores son ceros (como las que suelen generarse al usar representaciones como TF-IDF en procesamiento de texto).
