# ICU
Background: The APACHE IV system is one of the ICU scoring systems used to predict mortality rate of ICU patients who are admitted within 24 hours. 

Objective: 
We are given a set of APACHE IV data (91713 rows and 185 columns) and a data dictionary that contains description of the features used in the APACHE IV data. From here, we will train a ML model to predict mortality rate of ICU patients.

# Methodology:
1) Inspect raw data, identify missing values, and perform data cleaning.
2) Perform EDA (Univariate & Bivariate Analysis) on cleaned data. 
3) Perform One-Hot Encoding on categorical features.
4) Train 5 classification models using the training set: DummyClassifier, LogisticRegression, DecisionTreeClassifier, RandomForestClassifier, KNeighborsClassifier. For each model, calculate the ROC AUC scores and confusion matrix using the predictions and actual target data from test set.

Technical skills: Pandas, Matplotlib, Seaborn, Missingno, EDA, one-hot-encoding, data visualization, Scikit-learn (Sklearn)

# Conclusion:
The models lacked performance, with the best model (Decision Tree Classifier) only managed 0.519 in ROC-AUC score. The results reflected a lack of understanding in how APACHE IV scoring works and thus the selected features underperformed in mortality prediction.  

# Ideas for improvement and rework:
- Recalibrate the ML model based on APACHE II system, see [APACHE II system](https://en.wikipedia.org/wiki/APACHE_II)
- Recalibrate the ML model based on the following research paper 
"The Ability of the Acute Physiology and Chronic Health Evaluation (APACHE) IV Score to Predict Mortality in a Single Tertiary Hospital" (https://www.ncbi.nlm.nih.gov/pmc/articles/PMC6786733/)

# Useful reading:
1) APACHE II system: https://en.wikipedia.org/wiki/APACHE_II
