Predicting the Likelihood of Acute Myocardial Infarction (AMI) Diagnosis in ICU Patients Using Machine Learning Approaches

Through this research, we aim to advance the field by providing interpretable and effective models
that can assist clinicians in identifying high-risk patients early. This approach has the potential to
enable timely interventions, reduce diagnostic errors, and ultimately improve patient outcomes in
ICU settings.

Data Description

The Medical Information Mart for Intensive Care III (MIMIC-III) database is a publicly available
critical care dataset that contains comprehensive information on over 40,000 ICU admissions at
the Beth Israel Deaconess Medical Center between 2001 and 2012. The database integrates
diverse types of data, enabling researchers to conduct detailed analyses of ICU patient outcomes
and healthcare processes. Key components of the dataset are shown as follows:

• DIAGNOSES_ICD: Includes International Classification of Diseases (ICD) codes for
primary and secondary diagnoses.

• PROCEDURES_ICD: Contains ICD codes for medical procedures performed during ICU
stays.

• PATIENTS: Provides demographic information such as age, gender, and ethnicity.

• ADMISSIONS: Captures admission-specific details, including admission and discharge
times, admission type, and insurance information.

• LABEVENTS: Contains laboratory test results linked to patient admissions, including test
names, results, and timestamps.

• Lab_Item_Codes.txt: Offers descriptions or categories of laboratory items, aiding in the
interpretation of lab test results.

• Error-Prone Codes: Lists diagnosis codes associated with outcomes that are prone to
errors in recognition or treatment.

The MIMIC-III dataset is particularly suited for AMI prediction due to its inclusion of rich temporal
data, such as lab results, diagnostic codes, and treatment procedures. By analyzing trends and
patterns within this data, ML models can identify early indicators of AMI risk. The inclusion of
demographic and admission details further enables stratification of risk based on patient-specific
factors.

Conclusion

This project on early prediction of acute myocardial infarction (AMI) has demonstrated the
effectiveness of advanced machine learning models, particularly XGBoost and Histogram
Gradient Boosting, in predicting AMI risk. Both models outperformed Random Forest in terms of
overall predictive ability, with Histogram Gradient Boosting achieving the highest Area Under the
Curve (AUC) of 0.96, indicating superior discrimination between classes. Both XGBoost and
Histogram Gradient Boosting exhibited nearly identical accuracy rates of approximately 0.88,
showcasing its potential as a strong predictive tool. Random Forest, while demonstrating high
specificity (0.97), struggled with limited sensitivity (0.51), undermining its utility in effectively
detecting AMI cases.

From a clinical perspective, the results emphasize the need for careful model selection based on
the diagnostic priorities of healthcare providers. For tasks that require a balance between correctly
identifying both AMI and non-AMI cases, XGBoost and Histogram Gradient Boosting are ideal. In
settings where ruling out non-MI cases is critical, Histogram Gradient Boosting or Random Forest
may offer significant value. Furthermore, these models offer valuable insights into the underlying
factors contributing to AMI risk, such as key biomarkers like Creatine Kinase (CK), age, glucose
levels, fibrinogen, and other clinical parameters. These factors provide a foundation for future
research aimed at refining AMI prediction models and exploring new strategies for prevention and
treatment optimization.

Looking ahead, future work could explore the potential of combining these models through
ensemble methods to further enhance predictive performance. By incorporating multiple models,
we could potentially improve overall accuracy and reliability, making early AMI prediction more
robust and clinically actionable. There is still room to apply the LSTM deep learning model to the
time series sequential data. However, tree-based and ensemble models also perform well in
predicting the diagnosis, with less complexity in layers and computation. Additionally, XGBoost
offers greater interpretability through feature importance extraction.
