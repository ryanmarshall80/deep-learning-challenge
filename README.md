# deep-learning-challenge
Ryan Marshall Homework 21 repository

Overview

In this assignment, I used machine learning to try and predict whether an application for a loan from Alphabet Soup will ultimately lead to the funds be used effectively by the applicant.

Results

The target for my model was the 'IS_SUCCESSFUL' column in the charity_data.csv file.

The variables, or features, of my model were the other columns in the csv file with the exception of the 'NAME' and 'EIN' columns as these did not include data relevant to model.

I attempted to use either two or four hidden layers for my neural network, and the number of neurons varied from 4 to 12. I felt that this could be sufficient to solve the problem at hand.

For the activation functions of the hidden layers, I tried using 'relu', 'tanh', and 'sigmoid' on different runs.

To try and optimize the model, I tried increasing the number of hidden layers and the number of neurons in each layer. Unfortunately, this did not result in reaching the target accuracy score. I also tried changing the activation functions used by the hidden layers but this did not result in the model reaching the target accuracy score, either. I then tried running my model for a higher number of epochs, but once again this did not bring me to the target accuracy score. For my last attempt, I went back and changed some of the data in preprocessing. I dropped the 'STATUS' and 'SPECIAL_CONSIDERATIONS' columns as it seemed the overwhelming majority of the data had the same values for these columns and I believed it may help simplify things for the model. In addition, I grouped the APPLICATION_TYPES into a smaller number of bins and did the same for the CLASSIFICATION. Ultimately, however, I still did not reach the target accuracy score.

Summary

Overall, I was able to get an accuracy score of over 0.73, so my model was able to predict whether an applicant would be able to use funds from Alphabet Soup effectively at a 73% rate. If I were to try to optimize my model once again in the future, I would try cleaning up the data more during preprocessing. I could bin the 'INCOME_AMT' and 'ASK_AMT' columns to try and limit the effect of possible outliers in those columns.
