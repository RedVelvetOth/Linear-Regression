## Visualising The Data

![alt text](image.png)

Visualising the data on a log-scale shows a logaraithmic relationship between *t* and *p*

## Models and Results

| Model                       | RMSE        | MAE           | R2   |
| --------------------------- | ----------- | ------------- | ---- |
| Linear Regression           | 13097353.00 | 319709.08     | 0.10 |
| Random Forest (Logged Data) | 1.81        | 1.41          | 0.19 |
| Logged Linear Regression    | 1.58        | 1.23          | 0.38 |
| XGBoost (Logged Data)       | 1.53        | 1.18          | 0.42 |
| AdaBoost (Logged Data)      | 1.56        | 1.21          | 0.39 |
| Gradient Boost (Logged Data)| 1.53        | 1.18          | 0.42 |
| CatBoost (Logged Data)      | 1.53        | 1.18          | 0.42 |
| YDF (Logged Data)           | 1.53        | 1.18          | 0.42 |
| SVM (Logged Data)           | 1.52        | 1.16          | 0.42 |

## Second Approach 

Reshuffled the data and got a new train and test data set. Here are the result after using the previous models 

| Model                       | RMSE        | MAE           | R2   |
| --------------------------- | ----------- | ------------- | ---- |
| AdaBoost (Logged Data)      | 1.47        | 1.12          | 0.44 |
| Gradient Boost (Logged Data)| 1.46        | 1.11          | 0.45 |
| CatBoost (Logged Data)      | 1.46        | 1.11          | 0.45 |
| YDF (logged Data)           | 1.46        | 1.11          | 0.45 |

## DNN Model

| Layer (type)  | Output Shape |
| ------------- | ------------ |
| Normalization | (None, 1)    |
| Dense         | (None, 64)   |
| Dense_1       | (None, 64)   |
| Dense_2       | (None, 1)    |

| Model                       | RMSE        | MAE           | R2   |
| --------------------------- | ----------- | ------------- | ---- |
| DNN (Logged Data)           | 1.46        | 1.10          | 0.46 |