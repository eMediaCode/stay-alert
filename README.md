# Stay Alert! The Ford Challenge

This is the code for my attempt at the *Stay Alert!* challenge by the Ford Motor Company to detect alertness in drivers.

## Overview

I built a decision tree classifier and a random forest classifier that predict whether a driver is alert, using the [Scikit-learn](http://scikit-learn.org/stable/) library. The inputs are numeric, and the outputs are binary (indicating whether the driver is alert). 

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

I used the dataset provided by Ford Motor Company (input/ford_train.csv and input/ford_test.csv) with 604,329 observations (trial experiments) and 32 attributes.


| Column  | Definition |
| ------------- | ------------- |
| TrialID  | Experiment trial ID  |
| ObsNum  | Observation number  |
| IsAlert  | Is the driver alert or not?  |
| P1, P2, ..., P8  | Physiological data  |
| E1, E2, ..., E11  | Environmental data  |
| V1, V2, ..., V11  | Vehicular data  |

_**Note:** The actual names and measurement units of the physiological, environmental and vehicular data are not disclosed in this challenge._

## Predictions

The predictions for each model can be found as follows:

| Model  | Predictions |
| ------------- | ------------- |
| Decision Tree Classifier  | /dtree.csv  |
| Random Forest Classifier  | /rfc.csv  |
