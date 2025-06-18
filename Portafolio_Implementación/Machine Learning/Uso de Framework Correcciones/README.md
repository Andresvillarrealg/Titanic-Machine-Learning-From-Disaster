# Uso de Framework Regresión Logistica

Este repositorio contiene la implementación de modelos de clasificación utilizando regresión logística para predecir la clase de diferentes vinos basándose en varias características químicas del dataset proporcionado.

## Archivos incluidos:

wine.data: Archivo de datos que contiene las características químicas de los vinos, así como las clases a las que pertenecen.

wine.names: Archivo que describe las características presentes en el dataset de vinos.

Uso de Framework Correccion.ipynb: Script principal que implementa los modelos de regresión logística para diferentes combinaciones de características y realiza la evaluación de los mismos.

README.md: Este archivo que contiene la explicación del proyecto y detalles importantes sobre el entrenamiento de los modelos.


## Estructura del código

Carga de datos: El script carga el dataset wine.data y define las características que se utilizarán para la clasificación.

Selección de características: Se entrenan varios modelos utilizando diferentes características:

Un modelo basado en la característica Alcohol.

Un modelo basado en la característica Ash.

Un modelo que utiliza ambas características y sus términos al cuadrado.

Entrenamiento de modelos: Se dividen los datos en conjuntos de entrenamiento y prueba. Luego, se entrena un modelo de regresión logística para cada combinación de características.

Evaluación del modelo: Se generan matrices de confusión y se calculan los F1-scores para comparar el rendimiento de cada modelo.


## Hiperparámetros:

Para el entrenamiento de los modelos de regresión logística, se seleccionaron los siguientes hiperparámetros:

Tasa de aprendizaje: Utilizamos el valor por defecto de LogisticRegression que realiza un ajuste basado en la función de pérdida. No se ajustó explícitamente.

Número de iteraciones (max_iter): Se estableció en 1000 para garantizar que el algoritmo converja de manera adecuada durante el entrenamiento.

El criterio utilizado para seleccionar estos hiperparámetros fue asegurar la convergencia y un rendimiento adecuado en una cantidad razonable de iteraciones.


## Resultados:

Modelo basado en Alcohol: F1 Score: 0.7719

Modelo basado en Ash: F1 Score: 0.4375

Modelo con ambas características y términos al cuadrado: F1 Score: 0.8128

El modelo que utiliza ambas características y sus cuadrados tuvo el mejor desempeño, según el F1-score.

## Correcciones Realizadas

A diferencia de la entrega anterior las correcciones que tiene esta entrega son las siguientes:

-Se cambió el algoritmo implementado de regresión lineal a regresión logistica ya que era incorrecto.

-Se añadió el archivo README que no se tenía antes.
