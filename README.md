# Neural_Network_Charity_Analysis

## Analysis Overview

The goal of this project is to examine and classify the success of philanthropic donations using deep-learning neural networks and the TensorFlow framework in Python.
For the analysis, we employ the following methods:

- Preprocessing the data for the neural network model
- Compile, train and evaluate the model
- Optimize the model

## Resources

- Data Source: charity_data.csv
- Software: Python 3.9, Anaconda Navigator, Conda 4.8.4, Jupyter Notebook 6.3.0

## Results

### Data Preprocessing

- The columns EIN and NAME were eliminated from the input data since they contained identity information.
- The binary data in the IS SUCCESSFUL column indicates whether or not the charitable donation was utilised properly. The target variable for our deep learning neural network is then this variable.
- The features for our model are the columns APPLICATION TYPE, AFFILIATION, CLASSIFICATION, USE CASE, ORGANIZATION, STATUS, INCOME AMT, SPECIAL CONSIDERATIONS, and ASK AMT.
- The categorical variables were encoded, separated into training and testing datasets, and the features were standardised.

### Compiling, Training, and Evaluating the Model

- To increase the performance of the model, we applied bucketing to the feature ASK_AMT and organized the different values by intervals.
- We increased the number of neurons on one of the hidden layers, then we used a model with three hidden layers.
- We also tried a different activation function (tanh) but none of these steps helped improve the model's performance.
- - There are two hidden layers in this deep-learning neural network model, each containing 80 and 30 neurons.
- There are 43 characteristics and 25,724 samples in the input data.
- Because this is a binary classification, the output layer is made up of a single neuron.
- For the hidden layers, we use the activation function ReLU to speed up the training process. Sigmoid is employed on the output layer because our output is a binary categorization.
- The optimizer for this compilation is adam, and the loss function is binary crossentropy.
- The model's accuracy is less than 75%. This is an unsatisfactory result in terms of predicting the outcome of charitable donations.

## Summary

The profound learning neural organization model didn't arrive at the objective of 75% precision. Taking into account that this objective level is quite normal and we could say that the model isn't outflanking. 

Since we are in a double order circumstance, we could utilize a managed AI model, for example, the Random Forest Classifier to consolidate a large number of choice trees to produce an arranged yield and think about its exhibition in contrast to our profound learning model.
