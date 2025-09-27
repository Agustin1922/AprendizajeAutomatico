# Informe sobre los factores que influyen en la presión arterial
## Exploración inicial

El dataset incluye variables de edad, peso, horas de ejercicio, estrés, ingresos, horas de TV y la presión arterial como variable objetivo.
De la exploración estadística se observó que:
- La presión arterial aumenta en promedio con la edad y el peso.
- El nivel de estrés también muestra correlación positiva con la presión arterial.
- En cambio, los ingresos y las horas de TV no presentan una relación fuerte.


## El análisis de correlaciones muestra que las variables con mayor relación con la presión arterial son:

- Peso (r = 0.59): existe una correlación positiva moderada, lo que indica que a mayor peso, mayor presión arterial.

- Edad (r = 0.42): también se observa una relación positiva, aunque algo menor que el peso.

- Estrés (r = 0.37): presenta correlación positiva, sugiriendo que niveles más altos de estrés tienden a incrementar la presión arterial.

- Horas de ejercicio (r = -0.36): la relación es negativa, lo que significa que hacer más ejercicio se asocia con una presión arterial más baja.

En contraste:

- Horas de TV (r = 0.04) y Ingresos (r = -0.01) no muestran relación relevante con la presión arterial.

## Evaluación de los modelos

Modelo completo (todas las variables)

- R² = 0.708 → explica un 70.8% de la variabilidad de la presión arterial.

- RMSE = 10.36, MAE = 8.60 → errores moderados.

- Modelo simplificado (edad, peso, estrés y ejercicio)

- R² = 0.743 → explica un 74.3% de la variabilidad, incluso mejor que el modelo completo.

- RMSE = 9.72, MAE = 8.23 → menor error, lo que indica mejor ajuste.

Esto confirma que las variables edad, peso, estrés y ejercicio son las que realmente aportan valor explicativo.

# Conclusiones

Los factores que influyen de manera significativa en la presión arterial son principalmente:
- Peso: el predictor más fuerte, con un impacto claro en el aumento de la presión arterial.
- Edad: influye de manera positiva, aunque en menor medida que el peso.
- Estrés: también aumenta la presión arterial, aunque con un efecto algo más débil.
- Ejercicio: actúa como factor protector, reduciendo los niveles de presión arterial.

En cambio, los ingresos económicos y las horas de televisión no tienen un peso significativo, por lo que no son buenos predictores en este contexto.

El modelo simplificado con solo cuatro variables no solo mejora el ajuste (R² mayor), sino que también ofrece mayor interpretabilidad y eficiencia.
