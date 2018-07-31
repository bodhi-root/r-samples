---
name: Titanic
description: Data set of passengers and survivors from the Titanic
bannerImage: docs/Titanic.png
smallImage: docs/Titanic_small.png
---
# Titanic Data Set

SOURCE: https://www.kaggle.com/c/titanic/data

## Overview

The data has been split into two groups:

* training set (train.csv)
* test set (test.csv)

__The training set__ should be used to build your machine learning models. For the training set, we provide the outcome (also known as the "ground truth") for each passenger. Your model will be based on "features" like passengers' gender and class. You can also use [feature engineering](https://triangleinequality.wordpress.com/2013/09/08/basic-feature-engineering-with-the-titanic-data/) to create new features.

__The test set__ should be used to see how well your model performs on unseen data. For the test set, we do not provide the ground truth for each passenger. It is your job to predict these outcomes. For each passenger in the test set, use the model you trained to predict whether or not they survived the sinking of the Titanic.

We also include __gender_submission.csv__, a set of predictions that assume all and only female passengers survive, as an example of what a submission file should look like.

## Data Dictionary

Variable | Definition | Key
--- | --- | ---
survival | Survival	| 0 = No, 1 = Yes
pclass | Ticket class | 1 = 1st, 2 = 2nd, 3 = 3rd
sex |	Sex	|
Age | Age in years |
sibsp	| # of siblings / spouses aboard the Titanic |
parch	| # of parents / children aboard the Titanic |
ticket | Ticket number |
fare | Passenger fare |
cabin	| Cabin number |
embarked | Port of Embarkation | C = Cherbourg, Q = Queenstown, S = Southampton

## Variable Notes

__pclass__: A proxy for socio-economic status (SES)

* 1st = Upper
* 2nd = Middle
* 3rd = Lower

__age__: Age is fractional if less than 1. If the age is estimated, is it in the form of xx.5

__sibsp__: The dataset defines family relations in this way...

* Sibling = brother, sister, stepbrother, stepsister
* Spouse = husband, wife (mistresses and fiancés were ignored)

__parch__: The dataset defines family relations in this way...
* Parent = mother, father
* Child = daughter, son, stepdaughter, stepson

Some children traveled only with a nanny, therefore parch=0 for them.
