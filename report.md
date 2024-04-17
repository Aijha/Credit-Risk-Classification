# Module 12 Report

## Overview of the Analysis

The goal of this analysis was to predict whether loans would be healthy (low risk) or high risk using information about the loans and the people who took them out. This data included things like the borrower's income, debt-to-income ratio, and the loan's interest rate.

We thought that by using this data, we could build a model that would predict whether loans were high risk or healthy, helping us understand the risk level of the loans we provide.

One thing to note is that most loans in the data were healthy, so the data was unbalanced. This could make the model biased if we didn't take it into account.

To create the model, we first split the data into a training set and a testing set. We used the training set to train a logistic regression model to classify loans as either healthy or high risk.

After training the model, we tested it on the test set to see how well it predicted the loan statuses. We compared the model's predictions with the actual loan statuses to evaluate its performance.

## Results

We judged the model's performance using balanced accuracy, a confusion matrix, and precision and recall scores.

The balanced accuracy was 95%. The model performed slightly better with healthy loans than high-risk loans.
The confusion matrix showed very low rates of false positives, with only 0.5% of loans wrongly predicted as healthy.
The false negative rate was higher at 9%, meaning some loans were wrongly assessed as high risk when they were actually healthy.
The precision for healthy loans was 99.7%, showing that nearly all healthy loan predictions were accurate.
The recall for healthy loans was 99.5%, meaning the model correctly identified 99.5% of healthy loans.
The precision and recall for high-risk loans were slightly lower at 84.7% and 91% respectively, showing the model isn't as good with these loans.

* Machine Learning Model 1:
    Confusion Matrix:

Predicted Healthy: 18,663 (actual healthy) and 102 (actual high risk)
Predicted High Risk: 56 (actual healthy) and 563 (actual high risk)

## Summary

The model has very high accuracy overall. To decide if it should be used, we need to consider the business impact of following its recommendations. For example, how much could we lose from loans labeled as healthy but are actually high risk?

We may also want to review the false predictions to see if they involve larger or smaller loans than average, which would help us understand the risk.

Overall, the model does a great job estimating which loans will be healthy and which will be high risk."
