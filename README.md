# Parkinson's-Disease-Prediction

### Overview
* Created a tool for early detection of Parkinson's disease
* (To begin with, the dataset was aggregated by Max Little of the University of Oxofrd, in collab with the National Centre for Voice and Speech, Denver, Colorado, USA, who recorded the speech signals)
* The same dataset was found and downloaded from uci repository for Data Science projects.
* Optimized Base and Ensemble Learner Algorithms to build a model
* Built a client facing API using fastapi and colabcode

### Code and Resources used
* Python version : Python 3.7
* Packages : pandas, numpy, matplotlib, seaborn, sklearn, pickle, fastapi, colabcode

### Project Walk-through
* Dataset : Dataset was read using pandas library.
* Domain Knowledge : Each column variables recorded various aspects of voice (linear and nonlinear).
* Data Cleaning : Data was checked for null values.
* As the data collected was scrupulously monitored, only exclusive variables are gathered with no null values
* Scaling : The input float values, as the scales of different variables are widely spread and ununiform, were scaled.
* The Split : The dataset was divided - predictor(X) and target variable(y). Also, train_test_split was implemented.
* Base Models : Base Regression Classifiers, Support Vector Machines, Decision Tree and KNearestClassifier were implemented. Hyperparameter tuning improvised the model.
* Ensemble Models : Random Forest, and Boosting Algorithms - AdaBoostClassifier, GradientBoostingClassifier, XGBClassifier - were also used, to train the model.
* Inference : XGBClassifier gave a maximum accuracy for correct prediction of patients' records with utmost ability to categorize the patient.
* Deployment : The model was deployed using fastapi and colabcode, with the aid of pickle and pydantic.
