# Daphnia
Desarrollado en el curso de Redes Neuronales por: Diego Quezada y Kevin Reyes.
## Objetivos
- Predecir la toxicidad acuática aguda a la especie Daphnia Magna.
- Evaluar la sensibilidad a hiperparámetros de las arquitecturas de redes neuronales.
- Comparar distintas arquitecturas de redes neuronales profundas.
- Comparar las distribuciones de los pesos generados por las distintas forma de inicializar los pesos de las capas.
- Analizar las distribuciones de los gradientes de las capas de la red neuronal profunda.
- Estudiar el efecto de la regularización en las redes neuronales profundas.
- Evaluar redes Extreme Learning Machines.
- Evaluar el uso de Dropout sobre las redes neuronales profundas.
- Estudiar el efecto del parámetro learning rate sobre el entrenamiento.
- Estudiar el efecto de los distintos optimizadores sobre el entrenamiento.
- Estudiar el efecto del parámetro Learning Decay sobre el entrenamiento.

## Descripción
Estudio comparativo de modelos predictivos de redes neuronales profundas para predecir la toxicidad acuática aguda a la especie Daphnia Magna.

## Conclusiones
- Valores muy altos para el parámetro Learning Decay generan un entrenamiento muy lento.
- El valor del learning decay es de gran importancia para lograr un buen entrenamiento.
- El optimizador SGD aumenta la capacidad de generalización lenta y continuamente. Adam y RMSprop generan un aprendizaje muy rápido, sin embargo desde un número determinado de epochs en adelante se comienza a sobreajustar. Adragad presenta un aprendizaje muy rápido y desde un número determinado de epochs el aprendizaje se vuelve lento y continuo como SGD. Los mejores errores de validación se encontraron con Adam y RMSprop.
- Un learning rate escogido de forma incorrecta podría generar divergencia en el entrenamiento, por el contrario, un buen learning rate podría acelerar considerablemente el aprendizaje de la red neuronal.
- La norma $L_1$ genera que existan pesos con valor cero en las distintas capas de la red neuronal, en cambio la norma $L_2$ genera pesos dispersos pero siempre centrados en cero.
- La introducción de Dropout efectivamente disminuye el sobreajuste sobre los datos.
- LA red Extreme Learning Machines tiene un desempeño destacable sobre las redes tradicionales, a pesar de tener un gran número de hiperparámetros no se observan problemas de sobreajuste y además se tiene un buen aprendizaje en pocas epochs.

## Stack de tecnologías
- Pandas.
- Numpy.
- Matplotlib.
- Plotly.
- Seaborn.
- Scikit-learn.
- Tensorflow.
- Keras.