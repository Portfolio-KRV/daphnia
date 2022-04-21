# Daphnia
Developed in the Neural Networks course by: Diego Quezada and Kevin Reyes.
## Objectives
- Predict acute aquatic toxicity to the species Daphnia Magna.
- Evaluate the sensitivity to hyperparameters of neural network architectures.
- Compare different architectures of deep neural networks.
- Compare the distributions of the weights generated by the different ways of initializing the weights of the layers.
- Analyze the distributions of the gradients of the layers of the deep neural network.
- Study the effect of regularization in deep neural networks.
- Evaluate Extreme Learning Machines networks.
- Evaluate the use of Dropout on deep neural networks.
- Study the effect of the learning rate parameter on training.
- Study the effect of the different optimizers on training.
- Study the effect of the Learning Decay parameter on training.

## Description
Comparative study of predictive models of deep neural networks to predict acute aquatic toxicity to the species Daphnia Magna.

## Conclusions
- Very high values ​​for the Learning Decay parameter generate a very slow training.
- The value of learning decay is of great importance to achieve good training.
- The SGD optimizer increases the ability to generalize slowly and continuously. Adam and RMSprop generate very fast learning, however from a certain number of epochs onwards it starts to overfit. Adragad is a very fast learner and from a certain number of epochs the learning becomes slow and continuous like SGD. The best validation errors were found with Adam and RMSprop.
- An incorrectly chosen learning rate could generate divergence in training, on the contrary, a good learning rate could considerably accelerate the learning of the neural network.
- The $L_1$ rule generates that there are weights with a value of zero in the different layers of the neural network, while the $L_2$ rule generates scattered weights but always centered at zero.
- The introduction of Dropout effectively decreases the overfitting on the data.
- The Extreme Learning Machines network has a remarkable performance over traditional networks, despite having a large number of hyperparameters, no overfitting problems are observed and it also has good learning in a few epochs.

## Technology stack
- Pandas.
- Numpy.
- Matplotlib.
- Plotly.
- Seaborn.
- Scikit-learn.
- Tensorflow.
- Keras.