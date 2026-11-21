# Crime Analysis in Pakistan

## Introduction 

The available dataset of 3 years is used to predict crime counts of specific crimes in different regions of Pakistan. This is regression problem, it is useful for the police to plan resources, see trends and identify high risk areas.

## Dataset

https://opendata.com.pk/dataset/crimes-reported-by-type-and-provinces-in-pakistan-2018-2020/resource/59ccb28c-7f6c-4219-a807-7a1c3ba29256

## Workflow

- Data Cleaning
- Plotting Graphs
- Preprocessing: ColumnTransformer
- Feature Engineering
- Created different models (Baseline, RidgeCV, Decision Tree, Random Forest)
- Cross Validation
- Interpretation and Testing

## Results

                     Model  Mean Absolute Error  Mean Square Error  R2 Score
0                 Baseline           891.134134        2594.555477  0.902543
1              Ridge/Lasso           164.224921         492.503075  0.996488
2  Decision Tree Regressor           515.384615        2543.641272  0.906330
3  Random Forest Regressor           666.351980        2743.869371  0.891003

