## Zyfra Machine Learning Project

## Introduction
Prepare a prototype of a machine learning model for Zyfra. The company develops efficiency solutions for heavy industry.
The company develops efficiency solutions for heavy industry.
The model should predict the amount of gold recovered from gold ore. You have the data on extraction and purification.

The model will help to optimize the production and eliminate unprofitable parameters.

You need to:

- Prepare the data
- Perform data analysis
- Develop and train a model

## Description

1. Prepare the data

1.2. Check that recovery is calculated correctly. Using the training set, calculate recovery for the rougher.output.recovery feature. Find the MAE between your calculations and the feature values. Provide findings.

1.3. Analyze the features not available in the test set. What are these parameters? What is their type?

1.4. Perform data preprocessing.

2. Analyze the data

2.1. Take note of how the concentrations of metals (Au, Ag, Pb) change depending on the purification stage.

2.2. Compare the feed particle size distributions in the training set and in the test set. If the distributions vary significantly, the model evaluation will be incorrect.

2.3. Consider the total concentrations of all substances at different stages: raw feed, rougher concentrate, and final concentrate. Do you notice any abnormal values in the total distribution? If you do, is it worth removing such values from both samples? Describe the findings and eliminate anomalies. 

3. Build the model

3.1. Write a function to calculate the final sMAPE value.

3.2. Train different models. Evaluate them using cross-validation. Pick the best model and test it using the test sample. Provide findings.

## Conclusion
- A lot of columns had missing values that we filled using forward and backwards fill.
- Manually calculated recovery value and found out that the MAE was 9.30
- Figured out which columns were not in the test set and initiated our train and test sets with that information
- Concentrations of au went up after each cycle.
- Concentrations of ag were initially up but afterward went down again in the last cycles.
- Concentrations of pb only went up a bit, but then didn't go up after the last cycle.
- The best model was the decision tree regressor model, with the lowest sMAPE value at 12.9. 
- We tested our test set on this model and it aquired a final sMAPE score of 10.5.
- A constant model was also made to compare our final model and it outperformed it by a small margin.
