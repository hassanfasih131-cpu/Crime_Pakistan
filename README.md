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

<img width="503" height="169" alt="image" src="https://github.com/user-attachments/assets/6bf34db6-9251-44a4-bda8-6e54711fa431" />

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

## Example Prediction

<img width="376" height="90" alt="image" src="https://github.com/user-attachments/assets/01b0a831-f2fb-485e-8b7e-1c6d7c12acdb" />

## How to run

repo link: https://github.com/hassanfasih131-cpu/Crime_Pakistan.git

pip install -r requirements.txt

Crime_Pakistan.ipynb

Use Google Collab / Jupyter

Install the file from the link above for analysis

## Structure

- Crime_Pakistan.ipynb
- README.md
- requirements.txt
- images.md

## Author

Hassan Fasih
