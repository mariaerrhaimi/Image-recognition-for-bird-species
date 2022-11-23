# Predictive Modelling Competition 🐣


### LAST GROUP ACTIVITY! 👹
hey

For this group project, we are making a model to recognize bird species names based on their image using tensorflow.

*first thing we did was import our necessary libraries and packages needed for this project

we donloaded our dataset from kaggle:https://www.kaggle.com/datasets/gpiosenka/100-bird-species

*next we manually created a subset of our training ,validation and test dataset to run it in less time.

* batch size: The batch size refers to the number of samples processed before the model is updated.
* epoch: the number of passes that have been made through the training dataset.
*since our data is already split we can skip that part

*next we can visualize our data: Here we have used pyplot module from matplotlib library to view our training dataset. 

*Now  we can design the CNN (Convolutional Neural Network) model. We decided to use the Sequential model since its  the most commonly used model as it consists of three convolution layers (Conv2D, MaxPooling2D, and Dense) with 128 units on top of it is activated by a ReLU activation function(‘relu’). 
       1-we rescale our data first.
       2-Conv2D:this layer creates a convolution kernel that is convolved with the layer input to produce a tensor of outputs.
       3-Max pooling is a pooling operation that selects the maximum element from the region of the feature map covered by the filter. Thus, the output after max-pooling layer would be a feature map containing the most prominent features of the previous feature map. 

*next we compile To view training and validation accuracy for each training epoch, pass the metrics argument to model.compile() method.we used ‘adam’ optimizer and SparseCategoricalCrossentropy() loss function to evaluate the loss. 

*next we Train the model using model.fit() method that allows the machine to learn patterns by providing training and validation dataset to the model.we can see with each epoch that the accuracy changes and gets better  

*finally we Created plots of accuracy and loss on the training and validation sets to consider bias and variance


How to choose the best epochs and batch size:
The best epoch and batch size can be determined through trial and error. Start with a small batch size and a low number of epochs. If the model does not converge, or if the training accuracy is not high enough, then increase the batch size and/or the number of epochs. Keep doing this until the model converges with a high training accuracy.
