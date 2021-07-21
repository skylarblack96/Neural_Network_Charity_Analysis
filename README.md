# Neural_Network_Charity_Analysis

## Overview
The purpose of this analysis is to create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup. With more than 34,000 organizations that have recieved funding in past years we will preproccess the data for a neural network model, compile, train, and evaluate the model, and optimize the model for the best results.

## Results
### Data Preproccessing
- Our target variable for our model is the IS_SUCCESSFUL variable which tells us whether the application was successful or not.
- Our feature variables for our model are APPLICATION_TYPE, INCOME_AMT, and SPECIAL_CONSIDERATIONS.
- The variables that are neither target or feature variables and therefore were removed were EIN, NAME, and ASK_AMT.

### Compiling, Training, and Evaluating the Model
- Three layers were used. The first layer with 200 nodes, the second with 100, and the third with 50. The first, second, and third layers all have relu activation functions. The output layer has sigmoid as its activation function. To optimize the neural network I chose three layers each with the activation function of relu because it returns values zero to infinity. The output function was chosen to be different from the layers, therefore I chose the sigmoid activation function which transforms the output range between zero and one.
- I was able to achieve a model performance of 0.742, .008 from the target performance of 0.75.
- To try and increase model performance I added layers and changed up the number of nodes for each layer. I also changed the activation functions and found that relu gave better results for each layer and sigmoid worked best for the output layer. I removed the ASK_AMT from the variables which increased model peformance the most.

## Summary
Overall the neural network model gave a performace of 0.742 after optimizing it with more layers, nodes, different activation functions, and deleted variables. Since the data provides a binary outcome of each application I would suggest a supervised learning model. Random Forest would rank the input variables based on importance and it is able to handle the many input variables. 
