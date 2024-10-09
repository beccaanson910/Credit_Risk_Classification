# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis: To determine if ML could predict the results by comparing the predictions to the actual results.

* Explain what financial information the data was on, and what you needed to predict. The data was on bank loans: high-risk and healthy loans. In order to predict, the actual default status of the loan was needed.

* Provide basic information about the variables you were trying to predict (e.g., `value_counts`). The variables that were being predicted are healthy loan and high-risk loan.

* Describe the stages of the machine learning process you went through as part of this analysis. The required data was first separated from the rest of the dataframe for the prediction. This was done by creating a new dataframe from the loan status and setting it as the "y" value. All other columns from the original dataframe were set to "X". Both the "X" and "y" dataframes were split further in training and testing variables. A logistic regression model was then created and used to make the predictions. A confusion matrix was created to compare the results and a classification report was printed to show the accuracy of the model compared to the original data.

* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any other algorithms).For logistic regression it is imperative to have a dataset with labeled examples, each of which has a binary outcome of 0 or 1 and one or multiple features.A logistic regression model will help in determining the probability of a loan becoming healthy or hih-risk. And this can be achieved by training the model. A trained model can create predictions and state the accuracy of the prediction using metrics like accuracy, precision, f-1 score, and support.The limitaions to logistic regression are complex relations and non-linear data.

## Results

Using bulleted lists, describe the accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
    * Description of Model 1 Accuracy, Precision, and Recall scores.

        * Accuracy: This is the ratio of the number of correct predictions to the cumulative number of predictions made by the model. It measures the correctess of the predictions across the classes. The accuracy of this model was 99%.

        * Precision: This is the measure of the proportion of accurately predicted positive cases from all the cases that were predicted as positive.The precision of this model was 99% for the healthy loans and 94% for the high-risk loans.

        * Recall Scores: This is the percentage of relevant data points that this model correctly identified. Usinf this model 100% of the relevant healthy loan data points and 84% of the relevanr high-risk loan data points were correctly identified.

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:

* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )
The logistic regression model does a good job at predicting the healthy loans (0) with a precision of 99% and a recall of 100%, whereas the high-risk loans, although it did pretty good but not as good as the healthy loans with a precison of 94% and a recall of 84%. The data shows that model performs best for the healthy loans because it has a higher prediction rate for healthy loans versus high-risk loans. The performance may be dependent on the problem that we are trying to solve, and in this case, a higher prediction rate for the healthy loans is beneficial.


If you do not recommend any of the models, please justify your reasoning.
