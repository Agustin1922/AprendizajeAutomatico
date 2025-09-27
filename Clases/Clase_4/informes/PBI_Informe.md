# Informe de Análisis PIB Mundial

## Correlaciones y Modelos Predictivos (2019-2023)

Este informe analiza las correlaciones entre el PIB de 50 países y el PIB mundial durante el período 2019-2023, desarrollando modelos predictivos para identificar qué combinaciones de países mejor explican las variaciones del PIB mundial.

Hallazgos Clave:

- El modelo "Top 5 correlacionados" logra una predicción perfecta (R² = 1.0000)
- Chile, Corea del Sur y España muestran las correlaciones más altas con el PIB mundial
- Alemania presenta la correlación más negativa (-0.803), seguida de Malasia y Hungría
- Los modelos basados en correlaciones estadísticas superan significativamente a los basados en intuición económica

## Análisis del PIB Mundial

Evolución del PIB Mundial (2019-2023)

2019: $58.58 billones
2020: $64.52 billones (+10.1%)
2021: $61.72 billones (-4.3%)
2022: $63.91 billones (+3.5%)
2023: $69.48 billones (+8.7%)

Observaciones:
- Crecimiento significativo en 2020 a pesar de la pandemia
- Contracción en 2021, posiblemente por ajustes metodológicos o efectos diferidos
- Fuerte recuperación y crecimiento en 2023

<img width="553" height="502" alt="image" src="https://github.com/user-attachments/assets/6c3e8a4f-e478-4faf-ad46-6e38922405d6" />

## Análisis de Correlaciones por Grupos
Economías Emergentes Asiáticas:
- Corea del Sur (+0.877) y Vietnam (+0.759) muestran alta correlación
- Contrasta con Malasia (-0.642), sugiriendo diferentes patrones de crecimiento

Economías Latinoamericanas:
- Chile (+0.882) y Colombia (+0.827) altamente correlacionadas
- Argentina (+0.059) prácticamente no correlacionada
- Perú (-0.476) en contra-tendencia

Economías Desarrolladas:
- Alemania (-0.803) y Estados Unidos (-0.204) en contra-tendencia
- España (+0.839) como excepción notable
- Sugiere que economías maduras pueden tener dinámicas diferentes al agregado mundial
  
# Evaluación de Modelos Predictivos
## Resultados Comparativos
  <img width="690" height="162" alt="image" src="https://github.com/user-attachments/assets/1676783d-027e-4807-9543-3ac956edc4bb" />

# Mejor Modelo: Top 5 Correlacionados
Composición: Chile, Corea del Sur, España, Colombia, Vietnam
Rendimiento: R² = 1.0000, MSE = 2.44e-05
Características del modelo:
- Combina economías de diferentes regiones (Asia-Pacífico, Europa, Latinoamérica)
- Incluye tanto economías desarrolladas como emergentes
- Todas con correlaciones individuales > 0.75

# Conclusiones

- Economías medianas como mejores predictores: Países como Chile y Corea del Sur son mejores indicadores del PIB mundial que Estados Unidos o China.
- Patrones contra-intuitivos: Las correlaciones negativas de grandes economías desarrolladas sugieren dinámicas económicas más complejas de lo esperado.
- Necesidad de más datos: Los resultados perfectos (R² = 1.0) indican probable sobreajuste, requiriendo validación con más años de datos.
