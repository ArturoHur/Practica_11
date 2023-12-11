# MLP

Este código muestra la implementación de una red neuronal para resolver el problema del operador lógico XOR. Aquí hay una descripción de la lógica detrás de este código:

**1.- Preparación de datos:**

> Se leen los datos de entrenamiento y prueba del archivo CSV utilizando Pandas.
La función normalize se utiliza para normalizar los datos entre 0 y 1, y se aplica a las características de entrada.



**2.- Función de activación:**

> Se define la función de activación sigmoide, comúnmente utilizada en capas ocultas de redes neuronales para introducir no linealidad en la red.



**3.- Clase de la red neuronal:**

> NeuralNetwork_XOR es la clase principal que contiene métodos para la propagación hacia adelante, hacia atrás, el cálculo de la pérdida, la inicialización de pesos, el entrenamiento y la predicción.
Los pesos (weights1 y weights2) se inicializan aleatoriamente y se ajustan durante el entrenamiento para optimizar la red.



**4.- Entrenamiento del modelo:**

> Se crea una instancia de la red neuronal (NeuralNetwork_XOR) y se entrenan tres modelos con diferentes inicializaciones de pesos.
Se selecciona el mejor modelo basado en la precisión en los datos de entrenamiento.



**5.- Evaluación del modelo:**

> Se evalúa la precisión del modelo seleccionado en los datos de entrenamiento y prueba.

Se visualiza la pérdida durante el entrenamiento y las predicciones del modelo en los datos de prueba, mostrando los datos reales y las predicciones.
En resumen, este código implementa una red neuronal simple para resolver el problema de XOR, una tarea clásica para demostrar la capacidad de las redes neuronales para modelar relaciones no lineales.


La Segunda Parte del código implementa una red neuronal para resolver un problema de clasificación con datos generados usando 'make_gaussian_quantiles' de Scikit-Learn. Aquí tienes un resumen de la lógica:

**Creación de datos Gaussian-quantiles:**

> Se generan datos usando 'make_gaussian_quantiles' que crea muestras a partir de distribuciones gaussianas con diferentes características.



**Normalización de datos:**

> Se define una función 'normalize' para normalizar los datos entre 0 y 1.



**Preparación de datos:**

> Los datos generados se normalizan y se dividen en conjuntos 'x_train' (características) e 'y_train' (etiquetas).



**Definición de la red neuronal:**

> Se define la clase NeuralNetwork_GaussianQuantiles para la red neuronal.

> Se inicializan los pesos, se implementa la función de activación ReLU y la función sigmoide, y se define la propagación hacia adelante (_forward_propagation) y hacia atrás (_back_propagation).



**Entrenamiento del modelo:**

> Se inicializa un modelo de red neuronal con capa de entrada de 2 nodos, capa oculta de 2 nodos y capa de salida de 1 nodo.

> El modelo se entrena usando los datos de entrenamiento (x_train e y_train) durante un número específico de iteraciones.

> Durante cada iteración, se realiza la propagación hacia adelante, se calcula la pérdida, se realiza la propagación hacia atrás y se actualizan los pesos.



**Predicción y evaluación del modelo:**

> Se hacen predicciones sobre los datos de entrenamiento.

> Se evalúa la precisión del modelo en los datos de entrenamiento usando 'metrics.accuracy_score'.



**Visualización de la pérdida:**

> Se muestra la gráfica de la pérdida durante el entrenamiento para visualizar cómo la pérdida cambia a lo largo de las iteraciones.



Este código implementa una red neuronal simple para resolver un problema de clasificación, utilizando datos generados con distribuciones gaussianas y luego entrenando el modelo para predecir estas clases.
