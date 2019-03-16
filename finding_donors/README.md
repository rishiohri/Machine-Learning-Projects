# Finding Donors for CharityML
### Supervised Learning Project

In this project, I worked on several supervised algorithms of my choice to accurately model individual's income using data collected from the 1994 U.S. Census. I chose the best candidate algorithm from preliminary results and further optimized this algorithm to best model the data. The goal of this implementation was to construct a model that accurately predicts whether an individual makes more than $50,000. This sort of task can arise in a non-profit setting, where organizations survive on donations. Understanding an individual's income can help a non-profit better understand how large of a donation to request, or whether or not they should reach out to begin with. While it can be difficult to determine an individual's general income bracket directly from public sources, we can (as we will see) infer this value from other publically available features. The dataset for this project originates from the UCI Machine Learning Repository.

In this project I learned and applied the following:

- Data Exploration
  - Used pandas librbary to read a csv file
  - Performed feature set exploration
- Data Preprocessing
  - Determined the skewed features
  - Applied log-transform on the skewed features
  - Normalized the numerical features. Scaled the features using MinMaxScaler from sklearn.preprocessing
  - Use pandas.get_dummies() to perform one-hot encoding on the 'features_log_minmax_transform' data.
  - Shuffle and split the data using train_test_split from sklearn.cross_validation
- Evaluating Model Performance
  - Found True Positives, False Positives, and False Negatives for naive model
  - Calculated Precision, Recall, Accuracy and F-beta score
  - Discussed and implemented three models - Gaussian Naive Bayes, Decision Trees and AdaBoost Classifier
  - Calculated the F1 score and accuracy for all the three models
- Model Selection
  - Compared the performace of three models
  - Fine tuned the chosen model using GridSearchCV
  - Found an optimized model
- Extracted feature importance and performed feature selection
  - Discussed effects of feature selection
