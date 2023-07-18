# Alphabet Soup Tool


## Overview:


This tool is meant to help select the applicants for funding with the best chance of success in their ventures. The information was used to create a binary classifier that can predict whether applicants will be successful if funded.


## Results:


- ### Data Preprocessing
    - The variables targeted in this model are from a column of information labeled as "IS_SUCCESSFUL"
    - The different features considered are 'NAME','APPLICATION_TYPE','AFFILIATION','CLASSIFICATION','USE_CASE','ORGANIZATION','STATUS','INCOME_AMT','SPECIAL_CONSIDERATIONS','ASK_AMT','IS_SUCCESSFUL'.
    - Columns such as 'STATUS' can be discarded as the content on those columns is the same across all considerations.
- ### Compiling, Training, Evaluating the Model
    - Three different hidden layers are put into effect with respective 100, 50 and 20 neurons. Accuracy increased when the first layer was activated as "relu"--Rectified Linear Units, subsequently two more layers were activated as "Sigmoid' to output data between 0 and 1.
    - The model performed successfully with an accuracy averaging in the mid-90's.
    - The success of the model came after acknowledging the majority of the rows, originally the exploration walked through removing the "EIN" and "NAME" features and during the optimization the "NAME" feature was reconsidered with the benefit of increasing the model's successful accuracy.


## Summary


In conclusion, by removing only the "EIN" feature, adding hidden layers with different neurons (100,50,20) the  model performed with an accuracy of 77% to 96%. Recommending that the model considers the "NAME" feature, thus the model increases its accuracy by about five percentage points.

![An image showing different accuracy percentages for the same model with different parameters is meant to be here](https://github.com/13263952/deep-learning/blob/main/Images/example.png)

