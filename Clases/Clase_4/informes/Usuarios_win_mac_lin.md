# Informe de Clasificación de Sistemas Operativos
## Modelo Random Forest

El modelo Random Forest logró una precisión del 76.47% en la clasificación de sistemas operativos de usuarios web. El modelo demuestra un rendimiento sólido, especialmente para la identificación de usuarios de Windows, mientras presenta algunos desafíos menores con usuarios de Linux y Mac.

## Dataset total: 170 usuarios

- Linux (Clase 0): 86 usuarios (50.6%)
- Windows (Clase 2): 44 usuarios (25.9%)
- Mac (Clase 1): 40 usuarios (23.5%)

Conjunto de prueba: 34 usuarios
- Linux: 17 usuarios
- Windows: 9 usuarios
- Mac: 8 usuarios

## Rendimiento del Modelo
Métricas Generales
- Precisión General: 76.47%
- Validación Cruzada: 67.59% (±16.81%)

# Rendimiento por Sistema Operativo

| Sistema Operativo | Precisión | Recall | F1-Score | Usuarios |
|-------------------|-----------|--------|----------|----------|
| **Linux**         | 80%       | 71%    | 75%      | 17       |
| **Mac**           | 100%      | 62%    | 77%      | 8        |
| **Windows**       | 64%       | 100%   | 78%      | 9        |

  
# Matriz de Confusión

<img width="845" height="707" alt="image" src="https://github.com/user-attachments/assets/6fb288f4-f937-4e8b-a47f-97c2d5d94106" />

##  PREDICCIÓN

| REAL \ PREDICCIÓN | Linux | Mac | Windows | Total |
|--------------------|-------|-----|---------|-------|
| **Linux**          | 12    | 0   | 5       | 17    |
| **Mac**            | 3     | 5   | 0       | 8     |
| **Windows**        | 0     | 0   | 9       | 9     |


# Predicciones Correctas ✅

- 12 usuarios Linux identificados correctamente
- 5 usuarios Mac identificados correctamente
- 9 usuarios Windows identificados correctamente
- Total correctas: 26/34 (76.47%)

# Errores de Clasificación ❌

- 5 usuarios Linux clasificados como Windows
- 3 usuarios Mac clasificados como Linux
- Total errores: 8/34 (23.53%)

# Fortalezas del Modelo:

Excelente para Windows: 100% de recall - detecta todos los usuarios de Windows
Alta precisión en Mac: Cuando predice Mac, acierta el 100% de las veces
Buena performance general: 76.47% de precisión es sólida para 3 clases

# Áreas de Mejora:

Confusión Linux-Windows: 5 usuarios Linux mal clasificados como Windows
Confusión Mac-Linux: 3 usuarios Mac mal clasificados como Linux
Recall bajo en Mac: Solo detecta 62% de usuarios Mac reales

# Patrones Identificados:

Linux vs Windows: El modelo tiene dificultad distinguiendo entre estos sistemas
Mac es único: Nunca confunde Mac con Windows (0 errores)
Windows es distintivo: Perfecto recall (100%) - características muy claras

# Comparación con Otros Modelos

| Modelo              | Precisión | Validación Cruzada |
|---------------------|-----------|--------------------|
| **Random Forest**   | 76.47%    | 67.59%             |
| **Logistic Regression** | 70.59%    | 63.94%             |
| **SVM**             | 67.65%    | 50.74%             |


# Conclusiones:

- Random Forest es efectivo para clasificar sistemas operativos con 76.47% de precisión
- Windows es el más fácil de identificar - características distintivas claras
- Mac tiene alta precisión pero baja cobertura (algunos usuarios Mac no se detectan)
- Linux presenta mayor variabilidad - algunos usuarios similares a Windows
