# Credit-Score-Classification
 ##Given a person’s credit-related information, build a machine learning model that can classify the credit score into *Good*, *Standard* and *Poor*
.There were two parts to the above task:
- **Exploratory Data Analysis**
- **Model Building and Training**

## Exploratory Data Analysis

The first step of EDA was Data Preprocessing, which included-
- Dropping null values
- Dropping columns that are not relevant to prediction
- Removing duplicate entries

The next step was **Data Visualisation**, which included plotting histograms of the numerical features and then plotting a heatmap of the correlation matrix.

After this, the numerical variables in string format were converted to *integer* and *float*.
Then, columns with mostly corrupted entries were removed.
**Outlier Detection** included removing values that were outside three standard deviations of the mean.
**Data Imbalance** was handled by oversampling the input values of *Good* and *Poor* labels to match that of *Standard* labels.
The next step was **One Hot Encoding** and **Scaling**, which involved converting the categorical attributes to numerical attributes, and standardizing the numerical attributes to make the training process stable.

## Model Building and Training
 
 The dataset was divided into training and testing sets in the ratio 7:3.
 Two classifiers, namely *Random Forest* and *Decision Tree* were built to train the dataset.
 
 Their results are shown as follows:
 ### Random Forest
 Accuracy : 0.87
 Precision : 0.88
 Recall : 0.87
 
 ### Decision Tree
 Accuracy : 0.87
 Precision : 0.87
 Recall : 0.87
