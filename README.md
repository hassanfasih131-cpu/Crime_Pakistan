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

0                     Model     Mean Absolute Error     Mean Square Error     R2 Score

0                   Baseline              891.134134           2594.555477     0.902543

1                 Ridge/Lasso              164.224921            492.503075     0.996488

2     Decision Tree Regressor           515.384615        2543.641272     0.906330

3     Random Forest Regressor              666.351980           2743.869371     0.891003



## Findings or Recommendations:
- For the most part the crime rate in the Main Provinces is much higher and lean more towards the positive side
- Despite being part of the Main Province, Balochistan in some cases lean more towards the negative side, likely due to its smaller population compared to the other provinces
- For the Special jurisdictions crime rate lean more towards the negative.
- Pakistan railways have an overall low crime baseline but it spiked considerably in case of Other/Petty Theft
- Violent crimes like Murder is more common in Balochistan compared to the other crime types
- Cattle theft is less common in more urbanised regions such as Islamabad, but more common in places that depend on live stock for -income such as Gilgit Baltistan
- Dacocity consistently shows a negative baseline, showing that it is much more rare nation wide

## Limitations:
- There is limited data of only 3 years with a small sample size, which limited the information we could gather
- The model predicts raw reported counts rather than per-capita crime rates, heavily populated provinces like Punjab appear more dangerous regardless of the actual risk per area
Feature importance does not prove causation
##Example Prediction

   Year     Region Type of Crime  Predicted_Crimes
0  2021     Punjab         Theft             15206
1  2021  Islamabad        Murder                59
2  2021      Sindh      Dacocity               703
3  2021        KPK       Robbery               284

