# Suicide Prediction with Advanced ML Techniques

This is the final project for DS-UA 301, Advanced Techniques in ML and Deep Learning. 

## Description

This project aims to apply advanced ML and DL techinques to build a prediction model and to evaluate the benefits and problems of the techiniques. The dataset used is the 2019 youth risk behavior dataset, which is widely used by social scientists to study the problem of youth suicide. The goal of this project is to find the best way to approach the problem using advanced ML/DL, while keeping the issue of equality in mind. 

**Approaches**:

Traditional ML methods and techiques (widely used before):

- Logistic regression, bagging and boosting models (Random Forest and XGBoost)

- Grid Search hyperparmeter tuning

Advanced ML/DL methods and techiques (not widely used before):

- Neural network, with a flexible structure

- Hyperband hyperparmeter tuning

Other Methods (not widely used before):

- Auto Machine Learning (using H2O library)

- Auto Feature Engineering (using AutoFeat)

After applying the above techniques, the time and the performance of each techinique are recorded. In addition, the model will be evaluated on different subset of the data (race) to identify any equality issues.

## Description of the repository and code structure

- 'state_data_2019.csv': the original data

- 'state_data_2019_processed_training.csv': the processed data using 'pre_processing.ipynb'

- 'pre_processing.ipynb': data preprocessing script

- 'base_tuning_models.ipynb': hyperparameter tuning script

- 'automl_autofeat_models.ipynb': automl script

- 'performance_evaluation.ipynb': evaluate the performance of different models on the test set; final analysis

- 'GBM_5_AutoML_2_20221218_193524': the best automl model produced by AutoML

## Example to execute the code:

To retune the hyperparameters: run cells in 'base_tuning_models.ipynb' to find the best hyperparmeters for each model. Then, update the hyperparmeters in 'performance_evaluation.ipynb' to re-examine the performance.

To evaluate the performance: run cells in 'performance_evaluation.ipynb' to train the models from pre-tuned hyperparameters. Then, their performance are evaluated and useful figures and metrics are calculated.

To test automl: run cells in 'automl_autofeat_models.ipynb'. By default, the script saves a copy of the model to be used by 'performance_evaluation.ipynb'. 

## Reference

Romanelli, M., Sheftall, A.H., Irsheid, S.B. et al. Factors Associated with Distinct Patterns of Suicidal Thoughts, Suicide Plans, and Suicide Attempts Among US Adolescents. Prev Sci 23, 73–84 (2022). https://doi.org/10.1007/s11121-021-01295-8

Ivey-Stephenson AZ, Demissie Z, Crosby AE, Stone DM, Gaylor E, Wilkins N, Lowry R, Brown M. Suicidal Ideation and Behaviors Among High School Students - Youth Risk Behavior Survey, United States, 2019. MMWR Suppl. 2020 Aug 21;69(1):47-55. doi: 10.15585/mmwr.su6901a6. PMID: 32817610; PMCID: PMC7440198.

https://www.cdc.gov/healthyyouth/data/yrbs/results.htm