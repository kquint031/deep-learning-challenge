# Module 21 Report: Deep Learning Challenge
## Overview of the Analysis

The purpose of the Deep Learning Challenge is to build a tool for Alphabet Soup, non-profit foundation, to help the selection process of applicants for funding, based on the best chances to successfully implement the requested funds. From the provided dataset that included information about each applicant, from Name & EIN identification columns, to application type, affiliation, classification of the organizationa, as well as status, income classification, special considerations for application need, the requeted fund amount, and whether the applicant has used money effectively. Dataset cleaning was necessary for better machine performance. 

## Data Processing
* The target variables in the model is whether the applicant has been successful or not, using values of 0 or 1 to indicate if the money was used effectively.
* The feature variables in the model are the remainder of the variables in the dataset: APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, SPECIAL_CONSIDERATIONS, INCOME_AMT.
* The columns that should be removed from the input data because they are neither targets nor features are EIN and NAME, as these columns are used for identification purposes and are not directly related to predicting the target variable 
  
## Compiling, Training, and Evaluating the Model
* The number of neurons in each layer I selected was within the range of 2 to 15, and the number of hidden layers was within the range of 1 to 6. The activation function can be either 'relu', 'tanh', or 'sigmoid'. I gave the algorithm the freedom to find the best configuration that maximizes the validation accuracy.
* Unfortunately, I was not able to meet the 75% target model performance. Additionally, I could not save the Optimized model in H5 format.
* In my attempts to increase the model performace I tried different neuron layer ranges, and different hidden layer numbers. I also increased the number of epochs so that the model would have a wider reference scope.

## Summary
The deep learning model achieved a validation accuracy of 0.72 in classifying the effectiveness of funding charitable organizations. While this is a promising outcome, it falls slightly short of the desired accuracy threshold of 75%. To potentially improve performance, I recommend exploring additional modifications to the neurons and hidden layers, but also try different predictive models for better outcome. 

## References
Code and analysis developed in support from UCB in class examples and lectures.
