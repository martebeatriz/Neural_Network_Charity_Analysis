# Neural_Network_Charity_Analysis

## Overview of the analysis: 

To demonstrate my knowledge of machine learning and neural networks, I created a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup. 

I used a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. The dataset had the following columns: 
* EIN and NAME—Identification columns
* APPLICATION_TYPE—Alphabet Soup application type
* AFFILIATION—Affiliated sector of industry
* CLASSIFICATION—Government organization classification
* USE_CASE—Use case for funding
* ORGANIZATION—Organization type
* STATUS—Active status
* INCOME_AMT—Income classification
* SPECIAL_CONSIDERATIONS—Special consideration for application
* ASK_AMT—Funding amount requested
* IS_SUCCESSFUL—Was the money used effectively

## Results

* Data Preprocessing

  * The target variable chosen was the "IS_SUCCESSFUL" column. 
  * The 'EIN' and 'NAME' columns were dropped. 
  * All other columns were used as the features for the model. 
* Compiling, Training, and Evaluating the Model
  * My neural model reflected these specifications:
    *  First hidden layer: 10 nodes, relu activation
    *  Second hidden layer: 8 nodes, relu activation
    *  Third hidden layer: 3 nodes, LeakyReLU activation
    *  Output layer: sigmoid activation 
  *  This model achieved a 74% accuracy which fell below the 75% target model performance.
  *  My original model had 2 hidden layers with 8 and 5 nodes respectively and both had relu functions. The output layer was sigmoid. This model also had an accuracy of 73%. I thought that adding more nodes and layers would achieve higher accuracy but it didn't. I also tried different functions on the third layer but that didn't help either. 
  *  I noticed that the INCOME_AMT column's values were unevenly distributed so I binned some values. That made no difference. 
  *  ![Income_Column_B4_Binning](https://user-images.githubusercontent.com/107375554/198097830-d2b0cd7f-f817-4d0d-ab4b-89f1e5c8bade.png)
  * ![Income_Column_Binned](https://user-images.githubusercontent.com/107375554/198098527-1e8331a1-82a0-4036-b221-6e3a262b569b.png)


## Summary
The overall results of my deep learning model were unsatisfactory. I'm still not sure how I could have made it better. I would have liked more time to trial and error with some other models. I think maybe a deep forest model may have worked better. 

