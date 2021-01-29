# Data-Preprocessing

Data Preprocessing tools 


a) Taking care of missing data
Missing data can be replaced by mean technique, median technique or mode , prediction technique, Deletion technique (large data set and only <1% missing data)

In most cases we use mean - If there are no drastic outliers that can change the performance of model

In case of outliers - use mediane 

Need to use Impute module from sklearn and SimpleImputer class

b) Encoding the categorical variables - Independent and dependent variables

Need to use compose module and ColumnTransformer class

simple inputter class from sklearn (scikit learn) is used to encode categorical variables

OneHotEncoder from preprocessing module - To encode into a vector i.e. Country - IND (1,0,0), aus (0,1,0), us(0,0,1) - 3 columns will be created  
LabelEncoder from preprocessing module - To encode a categorical variable to 0,1 i.e. Yes to 1 and No to 0
c)

Split the dataset into training and test sets - train the model to understand the correlation b/w variables in the dataset
test - to test the performance of the model

from sklearn.model_Selection import train_test_Split

If the model is trained too well i.e. it fits the training data better but doesn't perform well on test set - overfitting
vice versa is underfitting

Feature scaling - scales all the features to make sure they are on the right scale so as to make sure that one feature doesn't dominate the other


Do we need to do Feature scaling before splitting the data into training and test sets or after ?
>>> We HAVE to do it after because 
feature scaling will get the standard deviation and mean of the features, if we do it before the split then it will get these values for both training and tes
and there is no point of doing that we don't know the performance of model on test set
Instead 







