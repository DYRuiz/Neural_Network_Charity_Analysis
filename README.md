# Neural Network Charity Analysis

## Overview
The purpose of this analysis is to create a binary classifier capable of prediciting the success of investments made by Alphabet Soup based on a dataset applicants who have received over the years.  

## Results

#### Data Preprocessing

Variables included in the input were:
- APPLICATION_TYPE (feature)
- AFFILIATION (feature)
- CLASSIFICATION (feature)
- USE_CASE (feature)
- ORGANIZATION (feature)
- STATUS (feature)
- INCOME_AMT (feature)
- SPECIAL_CONSIDERATIONS (feature)
- ASK_AMT (feature)
- IS_SUCCESSFUL (target)

In the first iteration, idenfication columns EIN and NAME were removed from the input data.  In the optimization iterations, APPLICATION_TYPE and SPECIAL_CONSIDERATIONS were also removed.  

#### Compiling, Training, and Evaluating the Model

For consistency and comparability across models, the number of neurons (80 layer 1, 30 layer 2) were kept constant in all iterations.  One instance of an optimization attempt had three layers (10 neurons) and another used a leaky ReLU versus ReLU activation function.  All were attempts to mitigate any outliers or features that were preventing accruary improvements.  
  
## Summary

Although inputs perceived to be unrelated to determining the sucess of an investment were removed in optimization attempts, the accuracy of the models actually decreased from the first iteration.  Likewise, adding additional epochs in the training and hidden-layers proved equally disappointing.  Based on these results, it would be reasonable to explore different models of logistic regression such as a random forest classifier.  Using this model would provide more insight on which features were actually important in determining sucess rather than guessing.   
