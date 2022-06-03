# Classifying Opioid Prescription Using Machine Learning Techniques
CAPP 30254—Machine Learning for Public Policy \
Group Members: Wesley Janson, Matt Kaufmann, Piper Kurtz, Angela The, Eujene Yum

The purpose of this project is to predict whether a person is likely to be prescribed opioids based on data from 2014-2019 Medical Expenditure Panel Surveys (MEPS), which is a large-scale survey of families and individuals, their medical providers, and employers across the United States.

## Final paper is "Classifying_Opioid_Prescriptions.pdf"

## To accomplish this task, we utilized 3 datasets:
- **Household Full-Year**: Household characteristic variables including race/ethnicity, sex, age, marital status, income, public assistance, employment, perceived physical and mental health status
- **Prescribed Medicine**: Prescribed any opioids, number of non-opioid prescriptions, insurance coverage
- **Medical Conditions**: Number of conditions, whether any of their conditions were due to injury
Our final dataset has 45 feature variables with 65,871 observations.

## Main directory
- **identification.py**: Python script with functions assisting in identification of relevant feature variables to include in 
    models. These functions are VIF Identification and Correlation matrix heatmap creation (useless and uninterpretable) 
    both called in models.py.

- **models.ipynb**: Main Python script used to create Logistic regression, decision tree, neural network, random forest, and ada boost models for analysis.

## Data Cleaning directory
- Note: All files are located in the folder **data_cleaning**

- **data_clean_hh.py**: Python script to perform data cleaning on the Household Component (HC) datasets from 2014-2019.

- **data_clean_pmf.py**: Python script to perform data cleaning and aggregation on the Prescribed Medicine (PMF) datasets from 2014-2019.

- **data_clean_mc.py**: Python script to perform data cleaning and aggregation on the Medical Conditions (MC) datasets from 2014-2019.

- **data_clean_mc.ipynb**: Notebook file to explore the Medical Conditions (MC) datasets and perform initial summary statistics on the aggregated dataset.

- **data_clean_combine.py**: Python script to merge the following cleaned (and aggregated) datasets together (on ID, 2014-2019): 1) Household Component, 2) Prescribed Medicine, and 3) Medical Conditions.

## Other directories
- Photos for report: Photos used in final report
- Milestones for class: Additional info used to demonstrate progress throughout the quarter
