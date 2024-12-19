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
5
• Error-Prone Codes: Lists diagnosis codes associated with outcomes that are prone to
errors in recognition or treatment.

The MIMIC-III dataset is particularly suited for AMI prediction due to its inclusion of rich temporal
data, such as lab results, diagnostic codes, and treatment procedures. By analyzing trends and
patterns within this data, ML models can identify early indicators of AMI risk. The inclusion of
demographic and admission details further enables stratification of risk based on patient-specific
factors
