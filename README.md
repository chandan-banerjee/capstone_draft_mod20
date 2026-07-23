### Project Title

**Author**

#### Executive summary

#### Rationale
Why should anyone care about this question?

#### Research Question
What are you trying to answer?

#### Data Sources
What data will you use to answer you question?
I will use Kaggle data source. https://www.kaggle.com/datasets/guriya79/mental-health-disorder

#### Methodology
What methods are you using to answer the question?

#### Results
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

#### Next steps
What suggestions do you have for next steps?

#### Outline of project

- [Link to notebook 1]()
- [Link to notebook 2]()
- [Link to notebook 3]()


##### Contact and Further Information