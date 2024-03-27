# Proyecto 12 TripleTen
El servicio de venta de autos usados Rusty Bargain está desarrollando una aplicación para atraer nuevos clientes. Gracias a esa app, puedes averiguar rápidamente el valor de mercado de tu coche. Tienes acceso al historial: especificaciones técnicas, versiones de equipamiento y precios. Tienes que crear un modelo que determine el valor de mercado.
A Rusty Bargain le interesa:
- la calidad de la predicción;
- la velocidad de la predicción;
- el tiempo requerido para el entrenamiento

En este proyecto, hemos llevado a cabo un análisis exhaustivo de diferentes modelos de regresión para predecir el precio de los vehículos. Después de preparar los datos mediante la codificación de características categóricas y la división en conjuntos de entrenamiento y prueba, entrenamos varios modelos, incluyendo RandomForest, GradientBoosting, DecisionTree, LinearRegression, CatBoost, LGBM y XGB, ajustando hiperparámetros utilizando la validación cruzada.

Nuestro análisis reveló que los modelos de potenciación del gradiente, como GradientBoosting, CatBoost, LGBM y XGB, superaron significativamente a la regresión lineal en términos de calidad de predicción, medida por el error cuadrático medio de la raíz (RECM). Específicamente, encontramos que el modelo LGBM fue el mejor en términos de precisión de predicción, con un bajo error de prueba y entrenamiento, y un tiempo de entrenamiento razonablemente bajo en comparación con otros modelos.

Estos hallazgos sugieren que, para este conjunto de datos específico, los modelos de potenciación del gradiente son más adecuados para predecir el precio de los vehículos en comparación con la regresión lineal. Sin embargo, es importante destacar que la selección del mejor modelo puede depender del contexto y de los requisitos específicos del problema. Además, se debe tener en cuenta que el rendimiento de los modelos puede variar según la naturaleza y la calidad de los datos disponibles.

Además del análisis de los modelos de regresión, dedicamos una parte significativa de nuestro proyecto al preprocesamiento de datos para garantizar la calidad y la integridad de nuestros conjuntos de datos. Implementamos varias técnicas para abordar diferentes aspectos de los datos:

1. Imputación de datos faltantes: Utilizamos un modelo de imputación para manejar los valores faltantes (NaN) en nuestros datos. Esto nos permitió conservar la mayor cantidad posible de información valiosa en nuestros conjuntos de datos y evitar sesgos introducidos por la eliminación de filas o columnas con valores faltantes.

2. Tratamiento de datos inconsistentes: Identificamos y tratamos los datos inconsistentes mediante la aplicación de reglas de negocio y validaciones lógicas.

3. Gestión de datos atípicos (outliers): Abordamos los valores atípicos que podrían afectar negativamente el rendimiento de nuestros modelos de regresión. Esto incluyó la identificación de valores extremos mediante técnicas estadísticas y la posterior eliminación o transformación de estos valores para mitigar su impacto en el rendimiento del modelo.

Estas metodologías de preprocesamiento fueron esenciales para garantizar la integridad y la calidad de nuestros datos, lo que a su vez contribuyó al rendimiento mejorado de nuestros modelos de regresión. La atención cuidadosa a estos pasos nos permitió construir modelos más robustos y confiables para predecir con precisión los precios de los vehículos.

En conclusión, este proyecto proporciona un preprocesamiento de datos exahustivo, una comparación detallada de diferentes modelos de regresión y destaca la importancia de seleccionar cuidadosamente el modelo adecuado para obtener predicciones precisas en problemas de regresión de precios de vehículos.