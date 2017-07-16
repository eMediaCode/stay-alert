# Stay Alert! The Ford Challenge

This is the code for my attempt at the *Stay Alert!* challenge by the Ford Motor Company to detect alertness in drivers.

## Overview

I built a decision tree classifier and a random forest classifier that predict whether a driver is alert. I built the model using the [Scikit-learn](http://scikit-learn.org/stable/) library. The inputs are numeric, and the outputs are binary (indicating whether the driver is alert). 

Here are the accuracies for both models:

| Model  | Accuracy |
| ------------- | ------------- |
| Decision Tree Classifier  | 64.4%  |
| Random Forest Classifier  | 88.2%  |

## Dependencies

- numpy
- pandas
- scikit-learn

Install dependencies using [pip](https://pip.pypa.io/en/stable/).

## Dataset

I used the dataset provided by Ford Motor Company (input/ford_train.csv and input/ford_test.csv) with 604,329 observations (trials experiments) and 32 attributes.

- The first column is the **Trial ID** - each period of around 2 minutes of sequential data has a unique trial ID. For instance, the first 1210 observations represent sequential observations every 100ms, and therefore all have the same trial ID.
- The second column is the **observation number** - this is a sequentially increasing number within one trial ID.
- The third column has a value **X** for each row where:

  - X = 1     if the driver is **alert**, and
  - X = 0     if the driver is **not alert**.

- The next 8 columns with headers P1, P2 , …….., P8  represent **physiological data**.
- The next 11 columns with headers E1, E2, …….., E11  represent **environmental data**.
- The next 11 columns with headers V1, V2, …….., V11  represent **vehicular data**.

## Predictions

The predictions for each model can be found as follows:

| Model  | Predictions |
| ------------- | ------------- |
| Decision Tree Classifier  | /dtree.csv  |
| Random Forest Classifier  | /rfc.csv  |
