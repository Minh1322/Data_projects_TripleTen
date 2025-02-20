## Telecom Interconnect Churn Project

## Introduction
The telecom operator Interconnect would like to be able to forecast their churn of clients.

If it's discovered that a user is planning to leave, they will be offered promotional codes and special plan options. Interconnect's marketing team has collected some of their clientele's personal data, including information about their plans and contracts.

## Description

Interconnect mainly provides two types of services:

- Landline communication. The telephone can be connected to several lines simultaneously.
- Internet. The network can be set up via a telephone line (DSL, digital subscriber line) or through a fiber optic cable.

Some other services the company provides include:

- Internet security: antivirus software (DeviceProtection) and a malicious website blocker (OnlineSecurity)
- A dedicated technical support line (TechSupport)
- Cloud file storage and data backup (OnlineBackup)
- TV streaming (StreamingTV) and a movie directory (StreamingMovies)
- The clients can choose either a monthly payment or sign a 1- or 2-year contract. They can use various payment methods and receive an electronic invoice after a transaction.

## Conclusion
- All steps of my initial work plan were performed.
- Preprocessing the data is the first step to any data project, so that we can prepare our data for analysis with accurate data.
- Data cleaning is the next essential step before moving on to the actual exploratory data analysis. Exploratory data anaylsis needs to have correct data to achieve accurate analysis. 
- For exploratory data analysis, I analyze the data to figure out what story the data is telling and how to effectively extract the right information needed for model training. This is important for the next step where I prepare the features for model training, so that the model can perform the best.
- During the build models phase, I tested a group of different models with different hyperparameters using GridSearch to find the model that has the highest scoring for our needs. 
- Finally, we have to test our best model to see if the model is actually effective and consistent in achieving the results of predicting customer churn.
- Figuring out what features were important for the model training was a challenge because it is important what you choose as it can affect the model performance. 
- During model training, my AUC-ROC score was not as good as it should've been, so I had to experiment with more hyperparameters and features. 
- Figuring out the correct models and hyperparameters was very important to achieving the results needed for this project. 
- My final model was LightGBM with a ROC-AUC score of 0.861 and an accuracy of 0.897. 
