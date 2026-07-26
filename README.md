# Project Title

### Capstone Project - Mental Illness Risk prediction

### ***GIT HUB REPO link***

Please see the notebook link below : https://github.com/chandan-banerjee/capstone_draft_mod20/blob/main/capstone_analysis_with_feature_engg.ipynb

# Executive summary

1. This project develops an interpretable machine learning framework that evaluates clinical and behavioral data to predict the risk of mental health conditions. By identifying high-risk individuals early, this tool empowers clinicians and patients to implement proactive, personalized interventions before acute crises occur

2. At the sametime this framework should NOT miss any low/medium RISK patients who can develop mental illness in future

3. Evaluation Metrics: Evaluated primarily on Recall, F1-Score, and AUC-ROC to minimize false negatives( MAXIMIZE recall ) and ensure maximum safety in medical triage.

4. Mental Risk Prediction is a multi class classification project where a patient can be categorized as 'Low Risk', 'Medium Risk' or 'High Risk' depending on their socioeconomic factors , clinical factors & past treatment/medical history.

# Rationale
Why should anyone care about this question?

1. **For Patients:** Shifts the focus toward prevention rather than just symptom management. Early risk detection allows individuals to seek support before conditions escalate, improving long-term quality of life

2. **For Clinicians:** Acts as a powerful clinical decision-support tool. By automatically analyzing vast datasets like Electronic Health Records, algorithms help doctors identify subtle warning signs that might be missed during brief routine checkups

3. Identifying mental illness risk via machine learning transforms psychiatric care from reactive to proactive.

# Research Question
What are you trying to answer?

### How can I identify and predict Mental Health Risk factors which is a serious global challenge ? The  conditions like  Anxiety and Depression are the most common disorders globally and saw a massive surge in prevalence over the past three decades

# Data Sources
What data will you use to answer you question?

### I used Kaggle data source: https://www.kaggle.com/datasets/guriya79/mental-health-disorder

# Methodology
What methods are you using to answer the question?

### Class imbalance analysis, PCA , Correlation Matrix analysis, Encoding input features, target encoding (as appropriate), different multi-class classification model comparison, ROC-AUC, Recall & F1 score comparison  to see which algorithm produces better results for this Use Case .

# Results
What did your research find?

- This UseCase is on mental illness. I don't see any missing medical/clinical information for each patient in the given dataset. This is good in one way that I don'tneed to  use mean/median/mode or any other technique to fill-in the NULLS. The mdeical/clinical fators are very specific to a person, should not be generalized. 
- Incontrast I see data is noisy like for example, one member's anxiety_score,depression_score,stress_level are 4,4,5 respectively. If we feed raw data with less variance model will not learn patterns correctly and might show high accuracy score during training, which is incorrect.
- Mental health risks are rarely the result of a single isolated factor, but rather combinations of lifestyle and environment. So feature enginnering is an important step
- Transforming this raw data into meaningful features highlights hidden patterns, model accuracy, and reduces dimensionality so machine learning algorithms can better capture complex psychological and lifestyle interactions.
- Generating new features ( derived columns/feature ) uncover hidden correlations that raw features miss.
- Engineer features that highlight anomalies (like combining multiple high stress and anxiety indicators) to help models better delineate at-risk individuals.
- Data skewness observed. This needs to be handled by logrithmic transformation before feeding into an algorithm.
- Target class imbalance observed. Use/choose proper algorithm.
- PCA analysis indicates both categorical & numerical features play important role
- To find initial base model I used four classifiers, namely LogisticRegression,DecisionTree, KNearestNeighbor, SupportVectorMachine
- From overall performace(Train/Test time) and recall/precisionF1-score perspective I will take LogisticRegression as my base model & look for other algorithm that can handle class imbalance & non linear relationships in a better way

# Next steps
What suggestions do you have for next steps?

Will be filled up later during final submission

# Outline of project

Will be filled up later during final submission


# Contact and Further Information

Will be filled up later during final submission