# deep-learning-challenge

## Overview of the analysis: 
The nonprofit foundation Alphabet Soup wants a tool that can help it select the applicants for funding with the best chance of success in their ventures. We use the features in the provided dataset to create a binary classifier that can predict whether applicants will be successful if funded by Alphabet Soup by using Machine Learning and Neural Networks to create a Deep Learning algorithm. 

Results: Using bulleted lists and images to support your answers, address the following questions:

## Data Preprocessing
What variable(s) are the target(s) for your model? 
What variable(s) are the features for your model?
What variable(s) should be removed from the input data because they are neither targets nor features?

Our target variable for this Deep Learning algortihm is called IS_SUCCESSFUL. This is a measure of whether the funding money was used successfully. 
The input variables used are: 
- APPLICATION_TYPE: Alphabet Soup application type
- AFFILIATION: Affiliated sector of industry
- CLASSIFICATION: Government organisation classification
- USE_CASE: Use case for funding
- ORGANIZATION: Organisation type
- STATUS: Active status
- INCOME_AMT: Income classification
- SPECIAL_CONSIDERATIONS: Special considerations for application
  
Although the specific company applying will likely impact whether a grant is successful, we did not include the Name of the company applying for the funding as this would likely result in overfitting of the model, and could leave Alphabet Soup open to acusations of bias. 

## Compiling, Training, and Evaluating the Model

How many neurons, layers, and activation functions did you select for your neural network model, and why?
Were you able to achieve the target model performance?
What steps did you take in your attempts to increase model performance?

Initially we used 2 hidden layers and an output layer, with 8 neurons each using a Rectified Linear Unit (ReLu) activation function. We chose this as a sort of standard setup, with ReLu being a very popular activation function, and not wanting to overload the model with nuance but still wanting some depth of field. We attempted optimization by trialilng different activation functions, different numbers of neurons, different numbers of layers, as well as reducing the input size. None of these methods were effective in raising the accuracy of the model from the initial setup. 

Summary: Summarise the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and then explain your recommendation.

This model was very difficult to optimise, likely due to the noisiness of the data. It is very difficult to identify outliers within this dataset, and the data does not lend itself to visualization to give any insight on how to structure the model. 
