# Práctica: Detección de anomalías en tráfico de red
Libreta de práctica para los estudiantes del curso CIB-209, Temas Especiales en Seguridad de Datos y Sistemas
## Aviso sobre los datos
Las 1000 conexiones del archivo trafico_red.csv son sintéticas, generadas para este ejercicio con el script generar_datos.py. No corresponden a tráfico real capturado en ninguna red. La columna es_ataque existe solo para calificar el resultado al final del ejercicio, ni Isolation Forest ni DBSCAN la usan durante el entrenamiento.
## Cómo ejecutar en Binder
1. Abrir el repositorio en Binder con el botón de abajo:
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/wrodriguez-cenfotec/ejercicio2_anomalias_trafico_red/HEAD?urlpath=%2Fdoc%2Ftree%2Fejercicio2_anomalias_trafico_red.ipynb)
2. La primera carga tarda unos minutos mientras se construye el entorno. Tener paciencia.
3. Ejecutar las celdas en orden, de arriba hacia abajo.
4. La sesión de Binder es temporal. Antes de cerrar, descargar la libreta o guardar capturas de los resultados.
## Qué hace la libreta
- Carga las 1000 conexiones de red, 30 de ellas ataques reales, y revisa el desbalance entre clases.
- Escala las variables y entrena un Isolation Forest para detectar anomalías.
- Entrena un DBSCAN como detector alternativo basado en densidad.
- Compara ambos algoritmos con precisión, recall y matriz de confusión.
- Visualiza en un gráfico las conexiones marcadas como anómalas por cada algoritmo.
- scikit-learn, detección de outliers. https://scikit-learn.org/stable/modules/outlier_detection.html
- scikit-learn, DBSCAN. https://scikit-learn.org/stable/modules/generated/sklearn.cluster.DBSCAN.html
- Binder. https://mybinder.org/
