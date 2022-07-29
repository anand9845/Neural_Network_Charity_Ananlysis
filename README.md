# Neural_Network_Charity_Ananlysis

Detailed Report on Alpabet Soup Charity Project using TensorFlow

1. Overview:
    The purpose of this project is to build a model that is trained on the features of the alpabet soup charity
    file and then uses the model to predict that whether it was successful or not.

2. Data:
    . The data is in the form of a CSV containing 10 features in the start.
    . The data consists of 1 Target variable and 9 features.
    . The data has 34299 rows
    . 2 rows that are irrelevant are removed at the start.
    
3. Data Preprocessing:
    . The column "IS_SUCCESSFUL" is the target variable.
    . Rest of the Columns are the features.
    . The column "EIN" and "NAME" are removed because they are not relevant they are not a feature or a target         variable.
    . I used One Hot Encoding to encode the categorical variables inside the Feature Columns.
    . The data is scaled using Standard Scaler.
    . The data is split into training and testing data.
    . 20% of the data is used for testing and 80% is used for training.

4. Compiling,Training and Evaluating the Model
    . The model is compiled using the Adam Optimizer.
    . The model is trained for 20 epochs.
    . The model is evaluated on the testing data.
    . The Loss function is Cross Entropy.
    . The Metrics is Accuracy.
    . For optimization, the model is trained again changing the neurons and adding more hidden layers.
    . In the initial training, the model is trained for 20 epochs.
    . Input features are actually the scaled data length which is 43.
    . Iniitially for hidden layer 1 i used 100 neurons and for hidden layer 2 i used 50 neurons.
    . The neurons in the output layer is 1 because we are trying to predict whether the data is successful or not.
    . I used relu as activation function for the hidden layers.
    . I used sigmoid as activation function for the output layer.
    . I have reached a mark of 74& accuracy.
    . For increasing the accuracy, I increased the number of neurons in the hidden layers also i changed the activation function to sigmoid and also tried changing the optimizer to SGD and loss to MSE(mean squared error).
    . The accuracy is still not surpassing 74%.
    . I selected loss as BCE(Binary Cross entropy) and optimizer as Adam because by looking at the data we are dealing with binary classification and these provide best classification accuracy.
    . Also Relu actvates the > 0 module so it is better to use relu as activation function.
    . Batch size means the number of data points that are used to train the model at a time.
    
    
    
