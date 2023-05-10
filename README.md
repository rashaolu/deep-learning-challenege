# Overview 
The nonprofit foundation Alphabet Soup wants a tool that can help it select the applicants for funding with the best chance of success in their ventures. With your knowledge of machine learning and neural networks, you’ll use the features in the provided dataset to create a binary classifier that can predict whether applicants will be successful if funded by Alphabet Soup.

From Alphabet Soup’s business team, you have received a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years.

In this challenge We Process the Data, Compile, Train, and Evaluate the Model, Optimize the Model to increase the accuracy of the model.

# Results
The results of the model yielded an accuracy of 0.7419.
The test data has an accuracy of 0.7279300093650818, and a loss of Loss: 0.5542796850204468. This indicates that that model will be succesful in predicting the outcomes.
When optimizing the model I tried 3 different ways to get better results of the model. 
* For the first optimization attempt yielded an accuracy of 0.7428.
* The second optimization attempt yielded and accuracy of 0.7417.
* The third optimization attempt yielded an accuracy of 0.7413.

## Data Processing
* The variables of the model that is the target is the ['IS_SUCCESSFUL'] column of the application_df.
* The variables of the model that is the feature are the rest of the coumns in the application_df.
* The ['EIN'],['NAME'] coulmns were removed from the application_df becasue they are neither targets nor features.

## Compiling, Training, and Evaluating the Model
* I selected 2 hidden layers and an outer layer for the model. There were 80 neurons in the first layer, and 30 neurons in the second layer. I made the input features be equal to the length of the X_train data. I used relu as the activation function for both of the hidden layers, and used sigmoid as the activation function for the outer layer.
* I was able to achieve target model performance. The model had great accuracy that is close to the test data accuracy. 
* In order to increase the performace of the model I added another hidden layer but decreased the amount of nodes per layer and increased the epochs to 120. 
* For the first optimization I increased the number of hidden layers as well as increasing the number of epochs.
* For the second optimization attempt I decreased the number of nodes and decreased the number of epochs and kept 3 hidden layers. 
* For the third optimization attempt I used 2 hidden layers, lowered the number of nodes per layer and changed the activation function for the second hidden layer.

## Summary 
The overall results of the deep learning model is that the model does an adequate job of predicting the outcome of the data with an 74% accuracy. Increasing the number of hidden layers, and maybe changing the activation function and increasing the number of epochs might be some recommendations on how to optimize the data and solve the classification problem.