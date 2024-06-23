# Alphabet Soup Charity - Deep Learning

## Overview 

The purpose of the analysis was to build a tool that can help Alphabet Soup select the applicants for funding with the best chance of success in their ventures. 
Our goal was to use machine learning and neural networks to apply target/features on the dataset, create a binary classifier that was capable of predicting whether investors would be successful if funded by Alphabet Soup. 
We received a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years.

## Data Preprocessing

 - IS_SUCCESSFUL is the target and the feature column chosen data for the model and it is marked 1 for successful. 

 - EIN and Name should be removed from the input data because they are neither targets nor features

## Neural Network Model

For this Model Performance was used 2 hidden layers with respectively 80 and 30 as neurons and RELU as activation.

![alt text](https://github.com/larissarmourap/deep-learning-challenge/blob/main/Images/Model%20performance%20with%202%20layers.png)

The target predictive accuracy asked for this model were 75% or higher 75%, but on the model performanced the accuracy achieved is 72%.

![alt text](https://github.com/larissarmourap/deep-learning-challenge/blob/main/Images/Accuracy%20model%20performance.png)


The steps I used to increase the model performance in the optimization, were dropping additional columns as EIN', 'NAME','AFFILIATION','SPECIAL_CONSIDERATIONS','USE_CASE','ORGANIZATION.
Decreasing the number of application types to include values >300, and classification count > 600, also the epoch = 10, changed the activation hidden layer from **relu** to **tanh**. 
The accuracy did not reach 75%. Accuracy, in fact, decreased to 62%.

![alt text](https://github.com/larissarmourap/deep-learning-challenge/blob/main/Images/Accuracy%20optimization%20model%20with%204%20layers.png)

The best result model based on the analysis were the model used with 2 layers, 80 and 30 as numbers of neurons. The accuracy on this model was 72,7% for the relu and sigmoid activations. Since the random forest classifier is less affected by outliers, it should be the next step.
