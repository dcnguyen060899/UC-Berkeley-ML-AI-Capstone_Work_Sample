# UC-Berkeley-ML-AI---Capstone_Work_Sample
# Comprehensive EDA Insight Report

## Executive Summary

This report provides an exploratory data analysis (EDA) of a hospital dataset to uncover patterns and insights related to patient readmissions and length of stay. The analysis focuses on various factors such as hospital type, ward type, admission type, severity of illness, and other key features. The goal is to provide actionable insights for hospital management and policy-making to enhance patient care and optimize hospital operations.

## Key Insights

### Patient Readmissions

#### Total Readmissions by Hospital Type
![Total Readmissions by Hospital Type Code](images/Total_Readmissions_by_Hospital_Type_Code.png)
- **Observation**: Hospital type 'a' has the highest number of readmissions, followed by types 'b' and 'c'.
- **Interpretation**: This suggests that hospital type 'a' might be handling more complex cases or has a larger capacity.

#### Total Readmissions by City Code Hospital
![Total Readmissions by City Code Hospital](images/Total_Readmissions_by_City_Code_Hospital.png)
- **Observation**: Cities with hospital codes '1' and '2' have the highest readmissions.
- **Interpretation**: Indicates these hospitals are likely in urban areas with higher patient inflow.

#### Total Readmissions by Hospital Region
![Total Readmissions by Hospital Region Code](images/Total_Readmissions_by_Hospital_Region_Code.png)
- **Observation**: Regions 'X' and 'Y' have higher readmissions compared to region 'Z'.
- **Interpretation**: Suggests regional differences in hospital capacities or patient demographics.

#### Total Readmissions by Department
![Total Readmissions by Department](images/Total_Readmissions_by_Department.png)
- **Observation**: Gynecology department has the highest readmissions.
- **Interpretation**: This could indicate a higher volume of cases or a need for specialized follow-up care in this department.

#### Total Readmissions by Ward Type
![Total Readmissions by Ward Type](images/Total_Readmissions_by_Ward_Type.png)
- **Observation**: Ward type 'R' has the highest number of readmissions, followed by ward types 'Q' and 'S'. Ward types 'P', 'T', and 'U' have significantly lower readmissions.
- **Interpretation**: This suggests that ward type 'R' handles a higher volume of patients or more complex cases that lead to higher readmissions. The lower readmissions in ward types 'P', 'T', and 'U' may indicate either lower patient volumes or more effective patient management.

#### Total Readmissions by Ward Facility Code
![Total Readmissions by Ward Facility Code](images/Total_Readmissions_by_Ward_Facility_Code.png)
- **Observation**: Ward facility code 'F' has the highest number of readmissions, followed by codes 'E' and 'D'. Codes 'A', 'B', and 'C' have lower readmissions.
- **Interpretation**: This indicates that ward facility 'F' might be serving a larger or more critically ill patient population, resulting in higher readmissions. Facilities 'A', 'B', and 'C' might have better discharge planning or serve less critical cases.

#### Total Readmissions by Type of Admission
![Total Readmissions by Type of Admission](images/Total_Readmissions_by_Type_of_Admission.png)
- **Observation**: Trauma admissions have the highest number of readmissions, followed by emergency admissions. Urgent admissions have the lowest readmissions.
- **Interpretation**: The higher readmissions for trauma cases reflect the critical and often complex nature of these patients, requiring more frequent readmissions. Emergency cases also show high readmissions due to their acute nature, while urgent cases have comparatively lower readmissions.

#### Total Readmissions by Severity of Illness
![Total Readmissions by Severity of Illness](images/Total_Readmissions_by_Severity_of_Illness.png)
- **Observation**: Patients with moderate severity of illness have the highest number of readmissions, followed by those with extreme and minor severity.
- **Interpretation**: This suggests that patients with moderate severity of illness are more likely to be readmitted, possibly due to ongoing health issues that require repeated hospital care. Patients with extreme severity might have higher mortality rates or more intensive care leading to fewer readmissions, while those with minor severity are less likely to be readmitted.



### Length of Stay

#### Length of Stay by Hospital Type
![Hospital Type Code vs Length of Stay](images/Hospital_Type_Code_vs_Length_of_Stay.png)
- **Observation**: Variability in the length of stay is observed across different hospital types.
- **Interpretation**: Hospital type 'a' has more variability, suggesting it handles a broader range of patient conditions.

#### Length of Stay by Department
![Department vs Length of Stay](images/Department_vs_Length_of_Stay.png)
- **Observation**: Departments such as surgery and TB & Chest disease show longer lengths of stay.
- **Interpretation**: This is expected as these departments typically handle more severe or complex cases.

#### Length of Stay by Ward Type
![Ward Type vs Length of Stay](images/Ward_Type_vs_Length_of_Stay.png)
- **Observation**: Ward types 'T' and 'U' have longer lengths of stay.
- **Interpretation**: Indicates these wards may cater to more critical or long-term care patients.

#### Length of Stay by City Code Hospital
![City Code Hospital vs Length of Stay](images/City_Code_Hospital_vs_Length_of_Stay.png)
- **Observation**: Consistent length of stay across various city codes, but some variability is seen indicating different patient management practices.

#### Length of Stay by Hospital Region
![Hospital Region Code vs Length of Stay](images/Hospital_Region_Code_vs_Length_of_Stay.png)
- **Observation**: Similar length of stay patterns across regions 'X', 'Y', and 'Z'.
- **Interpretation**: Indicates a standardized approach to patient care and management across regions.

#### Length of Stay by Type of Admission
![Type of Admission vs Length of Stay](images/Type_of_Admission_vs_Length_of_Stay.png)
- **Observation**: Trauma admissions tend to have longer stays compared to emergency and urgent admissions.
- **Interpretation**: Reflects the critical nature of trauma cases requiring extended care.

#### Length of Stay by Severity of Illness
![Severity of Illness vs Length of Stay](images/Severity_of_Illness_vs_Length_of_Stay.png)
- **Observation**: As expected, patients with extreme severity of illness have longer stays.
- **Interpretation**: Emphasizes the need for intensive care and prolonged treatment for more severe cases.

### Other Observations

#### Correlation Matrix
![Correlation Matrix of Selected Numerical Features](images/Correlation_Matrix.png)
- **Observation**: Number of visitors with patients shows a positive correlation with the length of stay.
- **Interpretation**: Suggests that patients with more visitors might be staying longer due to more severe conditions or extended recovery times.

#### Distribution of Admission Deposits
![Distribution of Admission Deposit](images/Distribution_of_Admission_Deposit.png)
- **Observation**: Admission deposits show a normal distribution with most values clustering around the mean.
- **Interpretation**: Indicates a standardized billing approach across different admissions.

#### Distribution of Visitors with Patients
![Distribution of Visitors with Patient](images/Distribution_of_Visitors_with_Patient.png)
- **Observation**: Majority of patients have 0-5 visitors, with a sharp drop-off beyond that.
- **Interpretation**: Reflects social support patterns for hospitalized patients.

## Recommendations

- **Focus on High Readmission Departments**: Departments like gynecology with high readmissions should be assessed for possible improvements in patient follow-up care and discharge planning.
- **Regional and Hospital Type Differences**: Address discrepancies in readmission and length of stay across different regions and hospital types to ensure uniformity in patient care.
- **Enhance Trauma Care Facilities**: Given the longer stays for trauma admissions, hospitals should ensure adequate resources and specialized care for these patients.
- **Patient Support Programs**: Implement programs to support patients with longer lengths of stay, including social support and post-discharge follow-ups.

From the distribution from readmission and length of stay across features, I have notice that readmission and length of stay distribution has similar pattern. However, note that not all features that has the same distribution pattern bettewn readmission and length of stay. For example, ward facility code has the highest readmission in code F. But all ward facility codes exhibit a similar pattern in length of stay, with a high concentration of shorter stays (1-3 days).

### Insights from Readmission and Length of Stay Patterns in Categorical Features

The summary statistics and visualizations suggest a pattern where patients with higher readmission counts tend to have longer stays. This pattern can also be observed across different categorical features, such as the type of admission, severity of illness, and hospital departments. Here are some specific insights:

#### Readmission Count vs Length of Stay

The summary statistics table indicates that the mean length of stay decreases slightly as the readmission count increases up to 10, then starts increasing again.

Certainly! Here is a concise version of the table in Markdown format:

| Readmission Count | Count   | Mean   | Std    | Min | 25% | 50% | 75% | Max  |
|-------------------|---------|--------|--------|-----|-----|-----|-----|------|
| 0                 | 92017.0 | 33.10  | 21.59  | 5.0 | 15.0| 25.0| 35.0| 110.0|
| 1                 | 71668.0 | 31.94  | 21.88  | 5.0 | 15.0| 25.0| 35.0| 110.0|
| 2                 | 53133.0 | 31.99  | 21.88  | 5.0 | 15.0| 25.0| 35.0| 110.0|
| 3                 | 37477.0 | 31.75  | 21.83  | 5.0 | 15.0| 25.0| 35.0| 110.0|
| 4                 | 25141.0 | 31.34  | 21.68  | 5.0 | 15.0| 25.0| 35.0| 110.0|
| 5                 | 15875.0 | 30.76  | 21.51  | 5.0 | 15.0| 25.0| 35.0| 110.0|
| 6                 | 9583.0  | 30.14  | 21.28  | 5.0 | 15.0| 25.0| 35.0| 110.0|
| 7                 | 5529.0  | 30.40  | 21.97  | 5.0 | 15.0| 25.0| 35.0| 110.0|
| 8                 | 3187.0  | 30.04  | 22.22  | 5.0 | 15.0| 25.0| 35.0| 110.0|
| 9                 | 1791.0  | 30.66  | 23.90  | 5.0 | 15.0| 25.0| 35.0| 110.0|
| 10                | 1030.0  | 31.57  | 25.14  | 5.0 | 15.0| 25.0| 35.0| 110.0|
| 11                | 630.0   | 31.52  | 25.81  | 5.0 | 15.0| 25.0| 35.0| 110.0|
| 12                | 357.0   | 33.64  | 27.95  | 5.0 | 15.0| 25.0| 35.0| 110.0|
| 13                | 246.0   | 35.41  | 30.26  | 5.0 | 15.0| 25.0| 42.5| 110.0|
| 14                | 172.0   | 37.18  | 31.40  | 5.0 | 15.0| 25.0| 55.0| 110.0|
| 15                | 116.0   | 44.40  | 36.61  | 5.0 | 15.0| 25.0| 65.0| 110.0|
| 16                | 90.0    | 45.94  | 38.12  | 5.0 | 15.0| 35.0| 82.5| 110.0|
| 17                | 66.0    | 47.88  | 36.68  | 5.0 | 15.0| 35.0| 75.0| 110.0|
| 18                | 49.0    | 49.90  | 33.80  | 5.0 | 25.0| 35.0| 65.0| 110.0|
| 19                | 42.0    | 51.07  | 34.44  | 5.0 | 25.0| 45.0| 75.0| 110.0|
| 20                | 34.0    | 47.35  | 35.87  | 5.0 | 25.0| 35.0| 70.0| 110.0|
| 21                | 29.0    | 57.93  | 38.42  | 5.0 | 25.0| 55.0| 85.0| 110.0|
| 22                | 24.0    | 55.21  | 32.92  | 5.0 | 15.0| 65.0| 85.0| 110.0|
| 23                | 20.0    | 64.00  | 35.60  | 5.0 | 32.5| 75.0| 87.5| 110.0|
| 24                | 18.0    | 54.72  | 32.88  | 5.0 | 35.0| 50.0| 75.0| 110.0|
| 25                | 16.0    | 50.31  | 38.23  | 5.0 | 20.0| 50.0| 75.0| 110.0|
| 26                | 13.0    | 60.38  | 40.02  | 5.0 | 25.0| 55.0| 110.0| 110.0|
| 27                | 11.0    | 67.73  | 40.15  | 5.0 | 40.0| 75.0| 110.0| 110.0|
| 28                | 10.0    | 58.50  | 41.17  | 15.0| 25.0| 45.0| 103.8| 110.0|
| 29                | 9.0     | 62.22  | 46.11  | 5.0 | 15.0| 85.0| 110.0| 110.0|
| 30                | 7.0     | 44.29  | 38.56  | 5.0 | 20.0| 35.0| 60.0| 110.0|
| 31                | 6.0     | 47.50  | 39.21  | 5.0 | 17.5| 55.0| 110.0| 110.0|
| 32                | 5.0     | 68.00  | 35.64  | 15.0| 55.0| 75.0| 85.0 | 110.0|
| 33                | 5.0     | 62.00  | 39.94  | 15.0| 35.0| 55.0| 95.0 | 110.0|
| 34                | 4.0     | 86.25  | 23.23  | 55.0| 77.5| 90.0| 98.8 | 110.0|
| 35                | 4.0     | 30.00  | 28.87  | 5.0 | 5.0 | 30.0| 55.0 | 55.0 |
| 36                | 3.0     | 51.67  | 5.77   | 45.0| 50.0| 55.0| 55.0 | 55.0 |
| 37                | 3.0     | 48.33  | 5.77   | 45.0| 45.0| 45.0| 50.0 | 55.0 |
| 38                | 3.0     | 61.67  | 20.82  | 45.0| 50.0| 55.0| 70.0 | 85.0 |
| 39                | 2.0     | 72.50  | 53.03  | 35.0| 53.8| 72.5| 91.3 | 110.0|
| 40                | 2.0     | 62.50  | 67.18  | 15.0| 38.8| 62.5| 86.3 | 110.0|
| 41                | 2.0     | 92.50  | 24.75  | 75.0| 83.8| 92.5| 101.3| 110.0|
| 42                | 2.0     | 72.50  | 53.03  | 35.0| 53.8| 72.5| 91.3 | 110.0|

- Patients with 0 readmissions have a mean stay of approximately 33 days.
- The mean length of stay for patients with 1-10 readmissions remains relatively stable around 31-32 days.
- For patients with more than 10 readmissions, the mean length of stay increases significantly, suggesting that a subset of patients with frequent readmissions require extended hospital stays due to complications or chronic conditions.


#### 1. Type of Admission

- **Emergency**: Patients admitted through emergency services tend to have varied lengths of stay, with a noticeable portion having longer stays. This category also sees frequent readmissions, indicating that patients admitted in emergencies may require longer recovery times and are more likely to be readmitted.
- **Trauma**: Trauma cases show a higher readmission count, and these patients also tend to have longer stays. This suggests that trauma patients often require extensive care and follow-up treatments, leading to longer hospital stays and higher readmission rates. Refer to the [Total Readmissions by Type of Admission](#total-readmissions-by-type-of-admission) and [Type of Admission vs Length of Stay](#length-of-stay-by-type-of-admission) images.
- **Urgent**: Urgent admissions also display a pattern of higher readmission counts and longer lengths of stay, though not as pronounced as trauma cases. This indicates that urgent cases, while serious, might not require as prolonged care as trauma cases but still exhibit a significant need for readmission and extended stays.

#### 2. Severity of Illness

- **Extreme**: Patients with extreme severity of illness have the longest lengths of stay and highest readmission counts. This is expected, as more severe cases generally require longer hospitalization and are at a higher risk of complications leading to readmission. Refer to the [Severity of Illness vs Length of Stay](#length-of-stay-by-severity-of-illness) and [Total Readmissions by Severity of Illness](#total-readmissions-by-severity-of-illness) images.
- **Moderate**: Patients with moderate severity show a balanced pattern but still exhibit significant lengths of stay and readmission counts, indicating that even moderate cases can be complex and require careful management.
- **Minor**: Minor severity cases have the shortest stays and lowest readmission counts, suggesting that these patients recover quicker and have a lower likelihood of complications that necessitate readmission.

#### 3. Hospital Departments

- **Radiotherapy**: Patients in the radiotherapy department have varied lengths of stay, with a significant number having longer stays. This department also sees higher readmission rates, likely due to the ongoing nature of cancer treatments.
- **Anesthesia**: The anesthesia department has moderate lengths of stay and readmission counts, reflecting the typical recovery times associated with surgical procedures.
- **Gynecology**: Gynecology patients generally have shorter stays and lower readmission counts, suggesting efficient treatment and recovery processes. Refer to the [Total Readmissions by Department](#total-readmissions-by-department) image.
- **TB & Chest disease**: This department shows higher lengths of stay and readmission counts, indicating the complexity and chronic nature of respiratory illnesses. Refer to the [Department vs Length of Stay](#length-of-stay-by-department) image.
- **Surgery**: Surgical patients exhibit a broad range of stay lengths and readmission rates, depending on the type and severity of the surgery performed.


### Confirming the Pattern: Readmission and Length of Stay

1. **Readmission Count vs. Length of Stay**
   ![Readmission Count vs Length of Stay](images/Readmission_Count_vs_Length_of_Stay.png)

   - The box plot indicates a general trend where higher readmission counts are associated with longer lengths of stay. Patients with more frequent readmissions tend to have a higher median length of stay, especially noticeable beyond 10 readmissions.

2. **Cumulative Stay vs. Length of Stay**
   ![Cumulative Stay vs Length of Stay](images/Cumulative_Stay_vs_Length_of_Stay.png)

   - The scatter plot shows the distribution of cumulative stays in relation to individual lengths of stay. While there are some outliers, the data points suggest that patients with longer individual stays tend to accumulate more days in the hospital overall, reinforcing the pattern observed in the readmission count. Overall, The visualization reinforces the pattern observed in the statistical summary. Higher readmission counts are generally associated with longer lengths of stay.

### Implications

These insights imply that:

- **Higher Readmission and Length of Stay**: Certain categories, such as trauma admissions and patients with extreme severity of illness, consistently show higher readmission counts and longer lengths of stay. This suggests that these patient groups are particularly vulnerable and may benefit from more intensive post-discharge care and monitoring to reduce readmissions and hospital stay durations.
- **Focused Interventions**: Hospitals can implement targeted interventions for high-risk groups, such as trauma and severe illness patients, to manage their care more effectively. This could include enhanced discharge planning, follow-up care, and outpatient support to reduce the likelihood of readmission and shorten hospital stays.
- **Resource Allocation**: Understanding these patterns can help hospitals allocate resources more efficiently. Departments with higher readmission rates and longer stays may require additional staff, specialized equipment, or dedicated programs to manage patient care more effectively.


# Comprehensive Modelling Insight Report

This section presents an analysis of factors influencing patient length of stay in hospitals using various machine learning models. The models employed include Gradient Boosting, Random Forest, CatBoost, XGBoost, and Logistic Regression. The analysis highlights the most impactful features identified by each model.

#### Model Performance Summary

| Model              | Train Accuracy | Test Accuracy |
|--------------------|----------------|---------------|
| Gradient Boosting  | 41.93%         | 41.62%        |
| Random Forest      | 49.68%         | 42.19%        |
| CatBoost           | 46.23%         | 42.84%        |
| XGBoost            | 45.80%         | 42.41%        |
| Logistic Regression| 39.92%         | 40.10%        |


#### Key Features Influencing Length of Stay
The top features identified across different models provide valuable insights into the factors affecting patient length of stay:

1. **Visitors with Patient**:
   - This feature consistently showed a high impact across models, indicating that the number of visitors is significantly related to the length of stay. More visitors might be associated with better patient morale and support, potentially leading to longer stays.

2. **Ward Type (Q, P, S)**:
   - Different ward types play a crucial role in determining the length of stay. This might be due to varying levels of care and facilities available in different ward types.

3. **Admission Deposit**:
   - The amount of the admission deposit is a significant predictor. Higher deposits may correlate with longer stays due to the nature of the treatment required or the financial capability of the patients.

4. **Bed Grade**:
   - The grade of the bed, which likely reflects the quality and type of care received, is an important factor. Higher bed grades usually indicate more intensive care and longer stays.

5. **Available Extra Rooms in Hospital**:
   - The availability of extra rooms in the hospital also impacts the length of stay. Hospitals with more available rooms might be able to accommodate patients for longer periods.

6. **Type of Admission (Emergency, Trauma)**:
   - Emergency and trauma admissions are linked to longer stays, reflecting the severity and immediate need for intensive care in such cases.

7. **Severity of Illness (Minor, Extreme, Moderate)**:
   - The severity of the illness is a critical factor. More severe illnesses naturally lead to longer hospital stays due to the complexity and intensity of required medical interventions.

8. **Hospital Codes and City Codes**:
   - The specific hospital and city codes also play a role, likely reflecting differences in hospital policies, regional healthcare quality, and patient demographics.

#### Visualizations
Below are the feature importance visualizations from each model:

- **Gradient Boosting**:
  ![Gradient Boosting Feature Importances](images/gradient_boosting.png)
- **Random Forest**:
  ![Random Forest Feature Importances](images/random_forest.png)
- **CatBoost**:
  ![CatBoost Feature Importances](images/catboost.png)
- **XGBoost**:
  ![XGBoost Feature Importances](images/xgboost.png)
- **Logistic Regression**:
  ![Logistic Regression Feature Importances](images/logistic_regression.png)

#### Insights and Recommendations
1. **Resource Allocation**:
   - Hospitals should consider allocating resources based on the ward types and severity of illness to optimize patient care and potentially reduce unnecessary prolonged stays.
   
2. **Visitor Management**:
   - Developing policies around visitor management could indirectly influence the length of stay, as more visitors might be associated with better patient outcomes.

3. **Financial Planning**:
   - Understanding the financial implications of admission deposits can help in planning and managing hospital finances and patient billing systems.

4. **Tailored Care Plans**:
   - Personalized care plans based on the type of admission and severity of illness could enhance patient recovery and optimize the length of stay.

5. **Facility Improvements**:
   - Investing in hospital facilities, such as upgrading bed grades and ensuring adequate extra rooms, can improve patient care quality and management efficiency.

By focusing on these key areas, hospitals can better manage patient length of stay, improve patient outcomes, and optimize operational efficiency.

# Comprehensive Classification Report, Confusion Matrix, and ROC-Curve Analysis

This section presents an analysis of predictive modeling for patient length of stay using various machine learning models. The models evaluated include Random Forest, Gradient Boosting, CatBoost, and XGBoost. The performance of these models is assessed through classification reports, confusion matrices, and ROC-AUC curves.

### Random Forest

- **Confusion Matrix**: The confusion matrix (Figure 1) indicates that the model struggles with accurately predicting the length of stay for several classes, particularly classes 0, 3, and 4.
- **ROC-AUC Curves**: The ROC-AUC curves (Figure 2) demonstrate that the model has varying levels of performance across different classes, with AUC scores ranging from 0.68 to 0.93.

### Gradient Boosting

- **Confusion Matrix**: The confusion matrix (Figure 3) shows similar issues as Random Forest, with poor prediction accuracy for classes 4, 6, 7, and 9.
- **ROC-AUC Curves**: The ROC-AUC curves (Figure 4) display a range of AUC scores from 0.67 to 0.93, indicating varied performance across classes.

### CatBoost

- **Confusion Matrix**: The confusion matrix (Figure 5) reflects challenges in predicting classes 4, 6, and 7 accurately.
- **ROC-AUC Curves**: The ROC-AUC curves (Figure 6) show AUC scores from 0.69 to 0.93, indicating decent performance for most classes but still room for improvement.

### XGBoost

- **Confusion Matrix**: The confusion matrix (Figure 7) reveals difficulties in accurately predicting classes 4, 6, and 7.
- **ROC-AUC Curves**: The ROC-AUC curves (Figure 8) exhibit AUC scores from 0.70 to 0.93, suggesting reasonable performance for most classes.

## Analysis

### Classification Reports
The classification reports for all models show:
- **Precision and Recall**: Precision and recall scores vary significantly across different classes, with lower scores for certain classes indicating that the models are struggling to predict those accurately.
- **F1-Score**: The F1-scores are generally lower for classes 4, 6, and 7, suggesting that these classes are particularly challenging for the models.

### Confusion Matrices
The confusion matrices highlight:
- **Misclassifications**: High levels of misclassifications for certain classes, especially those with fewer instances in the dataset, suggest that the models may be overfitting to more frequent classes.
- **Diagonal Dominance**: Diagonal values (correct predictions) are not as dominant as desired, indicating that the models have room for improvement in accuracy.

### ROC-AUC Curves
The ROC-AUC curves reveal:
- **Class-Wise Performance**: The models perform well for certain classes with AUC scores above 0.80, while performance is lower for others, indicating the need for further model tuning or additional feature engineering.
- **Overall AUC**: Generally high AUC scores (above 0.70) for most classes suggest that the models have a reasonable ability to distinguish between different length-of-stay classes.

## Conclusion and Recommendations
- **Model Selection**: While all models exhibit reasonable performance, CatBoost and XGBoost show slightly better test accuracy and AUC scores, making them preferable for this task.
- **Feature Engineering**: Further feature engineering, particularly focusing on classes with lower performance, could help improve model accuracy.
- **Class Imbalance**: Addressing class imbalance through techniques like oversampling, undersampling, or using class weights could improve model performance for underrepresented classes.
- **Hyperparameter Tuning**: Additional hyperparameter tuning, especially for models like CatBoost and XGBoost, may yield further performance improvements.

By addressing these areas, the predictive accuracy and generalization capability of the models for patient length of stay can be enhanced, leading to more reliable predictions and better-informed healthcare management decisions.

### Figures

- **Figure 1**: Confusion Matrix for Random Forest
![Confusion Matrix RF](images/confusion_matrix_rf.png)
- **Figure 2**: ROC-AUC Curves for Random Forest
![ROC-AUC RF](images/roc_rf.png)
- **Figure 3**: Confusion Matrix for Gradient Boosting
![Confusion Matrix GB](images/confusion_matrix_gb.png)
- **Figure 4**: ROC-AUC Curves for Gradient Boosting
![ROC-AUC GB](images/roc_gb.png)
- **Figure 5**: Confusion Matrix for CatBoost
![Confusion Matrix CatBoost](images/confusion_matrix_catboost.png)
- **Figure 6**: ROC-AUC Curves for CatBoost
![ROC-AUC CatBoost](images/roc_catboost.png)
- **Figure 7**: Confusion Matrix for XGBoost
![Confusion Matrix XGBoost](images/confusion_matrix_xgboost.png)
- **Figure 8**: ROC-AUC Curves for XGBoost
![ROC-AUC XGBoost](images/roc_xgboost.png)

This comprehensive evaluation highlights the strengths and areas for improvement in the current models, paving the way for enhanced predictive analytics in patient length of stay.
