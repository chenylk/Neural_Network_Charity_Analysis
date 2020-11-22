# Neural_Network_Charity_Analysis

## Overview
  * The purpose of the analysis was to create a binary classifier that is capable of predicting whether applicants will be successful with the funding of Alphabet Soup. A csv dataset containing 34,000+ organizations that recieved funding from Alphabet Soup was used to create a model that could predict future outcomes. 
  
## Results
  * Data Preprocessing
    1. The 'IS_SUCCESSFUL' variable was the target variable in this analysis. This variable indicated whether each company was worth the funding.
    2. The feature variables in this model were 'APPLICATION_TYPE','AFFILIATION','CLASSIFICATION','USE_CASE','ORGANIZATION','INCOME_AMT', and 'SPECIAL_CONSIDERATIONS'. These features were all determining factors in whether an organization was successful or not. 
    3. The removed input variables were the 'EIN' and 'NAME' columns because they had nothing to do with the success of an organization. These variables are just labels used as identifiers.
   
  * Compiling, Training, and Evaluating the Model
    1. Two hidden layers were used for this model, with the first hidden layer using 8 nodes and the second hidden layer using 5 nodes. I chose these numbers of nodes because I wanted to pick a number between the number of input variables and the number of output variables. 2 hidden layers felt like the right amount whereas if I used more, I could run into the problem of overfitting. As for the activation functions, I used the relu function for the hidden layers and the sigmoid function for the output layer. The relu is the most widely used function for hidden layers and the sigmoid function generates a value between 0 and 1. This distinction of values from the sigmoid function is what I need my model to predict since I am determining if a organization is succesful or not. 
    2. I was not able to achieve the target model performance.
    3. I tried to remove some of the "less useful" features. I also tried removing and adding hidden layers. More items were binned in certain features. The activation functions were substituted out for different ones. The epochs were increased and decreased to find a more optimal model. I, however, could not get the accuracy to pass the 75% threshold. 
    
## Summary
  * Overall, the deep learning model was more decently accurate. The model just about predicted the success of an organization 3/4 of the time. We could potentially look at ensemble learning models to achieve a higher accuracy rate. One potential model would be the random forest classifier. With the right amount of estimators the model could potentially be used as a great predictor of an organization's success. 
