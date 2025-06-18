# Implementación Regresión Lineal Sin Framework
Este proyecto implementa un modelo de regresión lineal simple utilizando el algoritmo de gradiente descendente para ajustar los parámetros. El objetivo es predecir los valores de la columna Valks (la variable dependiente) basándose en la columna Celsius (la variable independiente) del archivo Valhalla23.csv.

Criterio para la Selección de Tasa de Aprendizaje y Parámetros Iniciales
Tasa de Aprendizaje(α): Se seleccionó una tasa de aprendizaje pequeña (0.0001) para asegurar que el modelo converja lentamente pero de manera estable. Esto evita que los saltos en la actualización de los parámetros sean demasiado grandes, lo que podría llevar a que el modelo no converja correctamente.

Parámetros Iniciales: Los valores iniciales de 𝜃_0 y 𝜃_1 se establecieron en 0. Esto facilita el inicio del proceso de entrenamiento, ya que se parte de una línea recta que cruza el origen, permitiendo que el gradiente descendente ajuste los parámetros de manera óptima.

Número de Iteraciones: Se decidió aumentar el número de iteraciones a 10,000 para asegurar que el modelo tenga suficiente tiempo para ajustarse a los datos. Aunque un número menor de iteraciones puede ser suficiente en algunos casos, más iteraciones ayudan a reducir el error final si el modelo no ha alcanzado la convergencia.

## Correcciones Realizadas:
- Se incrementó el numero de iteraciones a 10,000.
- Se disminuyó el valor de la tasa de aprendizaje a 0.0001
