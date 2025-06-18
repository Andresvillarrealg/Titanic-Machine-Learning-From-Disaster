# Regresión con SGD Regressor

Este proyecto implementa un modelo de regresión lineal utilizando el algoritmo SGDRegressor de la librería scikit-learn. El propósito es ajustar un modelo a los datos proporcionados y evaluar su desempeño utilizando la métrica del error cuadrático medio (MSE).

## Archivos incluidos
SGDRegressor.ipynb: El notebook de Jupyter que contiene el código para la implementación del modelo de regresión.

Valhalla23.csv: Archivo de datos utilizado en el notebook. Este archivo contiene las características de entrada y los valores objetivo para entrenar el modelo.

## Estructura del código

### Paso 1: Importación de bibliotecas

Se importan las siguientes bibliotecas:

-pandas para manipulación de datos.

-numpy para operaciones numéricas.

-train_test_split para dividir los datos en conjuntos de entrenamiento y prueba.

-SGDRegressor para implementar la regresión lineal.

-mean_squared_error para calcular el error cuadrático medio (MSE).

-matplotlib para generar gráficos comparativos.

### Paso 2: Carga de datos
El archivo Valhalla23.csv se carga en un DataFrame de pandas. Las características se separan del valor objetivo, que se desea predecir utilizando el modelo.

### Paso 3: División de datos
Los datos se dividen en conjuntos de entrenamiento y prueba usando la función train_test_split. Se asegura que el conjunto de prueba sea el 20% de los datos.

### Paso 4: Entrenamiento del modelo
Se utiliza el algoritmo SGDRegressor para entrenar el modelo sobre el conjunto de entrenamiento. Durante el entrenamiento se optimizan los coeficientes del modelo utilizando el descenso de gradiente estocástico.

### Paso 5: Evaluación del modelo
El modelo se evalúa calculando el Mean Squared Error (MSE) tanto para el conjunto de entrenamiento como para el conjunto de prueba, lo que permite verificar el ajuste y la precisión del modelo.

### Paso 6: Gráfica de comparación
Se genera una gráfica que compara las predicciones del modelo con los valores reales para el conjunto de prueba, lo que permite una evaluación visual del desempeño del modelo.

## Hiperparámetros
El modelo SGDRegressor tiene los siguientes hiperparámetros ajustados:

-Tasa de aprendizaje: Utiliza la configuración predeterminada de SGDRegressor para el ajuste con descenso de gradiente.

-Número de iteraciones: Se utiliza el número por defecto que asegura que el modelo tenga tiempo de converger.

-Semilla aleatoria: Se utiliza una semilla aleatoria para asegurar reproducibilidad.
