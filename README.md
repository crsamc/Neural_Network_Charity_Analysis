# Neural_Network_Charity_Analysis
## Overview
Beks has come a long way since her first day at that boot camp five years ago—and since earlier this week, when she started learning about neural networks! Now, she is finally ready to put her skills to work to help the foundation predict where to make investments.
With your knowledge of machine learning and neural networks, you’ll use the features in the provided dataset to help Beks create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup.
From Alphabet Soup’s business team, Beks received a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. Within this dataset are a number of columns that capture metadata about each organization.

- Deliverable 1: Preprocessing Data for a Neural Network Model
- Deliverable 2: Compile, Train, and Evaluate the Model
- Deliverable 3: Optimize the Model
- Deliverable 4: A Written Report on the Neural Network Model (README.md)

## Results
Data Preprocessing
1. The column `IS_SUCCESSFUL` is considered the target for this model. 
2. The columns `APPLICATION_TYPE`, `AFFILIATION`, `CLASSIFICATION`, `USE_CASE`, `ORGANIZATION`, `STATUS`, `INCOME_AMT`, `SPECIAL_CONSIDERATIONS`, and `ASK_AMT` are considered to be the features for this model.
3. The columns `EIN` and `NAME` are neither targets nor features, and have been removed from the input data.

Compiling, Training, and Evaluating the Model
1. In the neural network model there are 2 hidden layers, the first layer has 80 and the second layer has 30 neurons. For the hidden layers, the activation functions were ReLu, and Sigmoid was used for the output layer.
2. In Deliverable 3, I was unable to achieve the target model performance goal of 75%.
3. To increase the performance of the model, I dropped `INCOME_AMT` along with `EIN` and `NAME`. I increased the hidden layers amount to 3 and added 10 neurons in that layer. I also used the (elu) function in the hidden layers activation function.

## Summary:
The deep learning neural network model did not reach the target of 75% accuracy. I was able to increase the original accuracy of 72.79% to 73.11% by dropping the `INCOME_AMT` column. However, with attempt 2 and 3, I was only able to reach accuracy of 72.94% and 72.83% respectively. 

A Random Forest Classifier could be used as an alternative to the deep learning classification model in this project. This type of model is good for binary classification problems.
