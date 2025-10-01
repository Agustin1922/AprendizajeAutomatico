
# Informe Comparativo: Árbol de Decisión vs. K-NN en Detección de Spam

El objetivo de esta clase fue aplicar y comparar dos algoritmos de clasificació **Árbol de Decisión** y **K-Nearest Neighbors (K-NN)**  en mi caso elegi un problema de ciberseguridad relacionado con la detección de mensajes de correos electrónicos spam.

El dataset utilizado contiene mensajes clasificados en dos categorías: spam (correos maliciosos o no deseados) y ham (correos legítimos), el data set fue sacado de la pagina de Kaggle (**SMS Spam Collection Dataset**).
Convertí las etiquetas a números (0 para "ham" y 1 para "spam"), transformé los textos con TF-IDF, dividí los datos en entrenamiento y prueba, entrené los modelos y evalué los resultados.

## Resultados obtenidos

Después de entrenar ambos modelos y evaluar su desempeño en el conjunto de prueba, se obtuvieron los siguientes resultados:

Resultados del Árbol de Decisión
- Precisión: 0.98 (clase 0), 0.92 (clase 1)
- Recall: 0.99 (clase 0), 0.84 (clase 1)
- F1-Score: 0.98 (clase 0), 0.88 (clase 1)
- Accuracy: 0.97095937799043
  
El Árbol de Decisión tuvo un buen rendimiento, especialmente para identificar mensajes no spam (clase 0), con alta precisión y recall. Para spam (clase 1), el recall fue un poco menor, lo que significa que algunos mensajes spam no fueron detectados.

Resultados de K-NN
- Precisión: 1.00 (clase 0), 1.00 (clase 1)
- Recall: 0.88 (clase 0), 0.28 (clase 1)
- F1-Score: 0.94 (clase 0), 0.44 (clase 1)
- Accuracy: 0.961604748688995

K-NN mostró una precisión perfecta para ambas clases, pero su recall para spam fue muy bajo (0.28), lo que indica que detectó muy poco spam. Esto sugiere que el modelo tuvo problemas para generalizar en esta clase.


## Análisis comparativo

El Árbol de Decisión tuvo una accuracy un poco mayor (0.97 vs 0.96) y un mejor equilibrio entre precisión y recall, especialmente para la clase spam. K-NN, aunque perfecto en precisión, falló en detectar la mayoría de los mensajes spam, lo que lo hace menos útil para esta tarea. 

## Conclusión

El Árbol de Decisión es el modelo más adecuado en este caso porque ofrece un mejor balance entre precisión y recall. El K-NN puede ser útil en algunos escenarios, pero en este dataset su desempeño es mucho peor para detectar spam.
