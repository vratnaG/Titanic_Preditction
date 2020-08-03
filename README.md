# Titanic_Preditction

Kaggle titanic dataset taken and predict the survival of the passenger.

# Dataset Description

Data Dictionary
Variable Definition Key
survival Survival 0 = No, 1 = Yes
pclass Ticket class 1 = 1st, 2 = 2nd, 3 = 3rd
sex Sex
Age Age in years
sibsp # of siblings / spouses aboard the Titanic
parch # of parents / children aboard the Titanic
ticket Ticket number
fare Passenger fare
cabin Cabin number
embarked Port of Embarkation C = Cherbourg, Q = Queenstown, S = Southampton

# Methodology

**Data Filling:** Embarked: max occurrence value fill in place of Nan Fare: Mean filling value. Cabin: Nan fill as No. Which have cabin number replaced as yes Age: fill based on feature-based Parch, Sibsp, Sex, Embarked and Pclass and remain filled by mean.

**Preprocessing:** Label encoder use for object. Apply PCA and 6 max variations respectively select as a feature for traning.

**Classifier:** Stacked classifier is used where estimeter are Random Forest, Grandient Boosting and Logistic regression. For final estimeter used Logistic regression.
