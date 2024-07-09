# A/B Testing with Customer Data
This Jupyter Notebook conducts A/B testing on a customer dataset to compare the conversion rates between an exposed group and a control group.


## **Content Summary**

**Libraries:** Imports necessary libraries for data manipulation, statistical analysis, visualization, and logistic regression.

**Data Loading:** Reads the CSV file named "AdSmartABdata - AdSmartABdata.csv" and stores it in a Pandas DataFrame.

**Data Cleaning:**
* Checks for duplicates and missing values. 
* Filters out users who did not interact (yes=0 and no=0). 
* Splits the data into exposed and control groups based on the "experiment" variable.


**Data Analysis:**
* Calculates the conversion rate for each group.
* Performs a Z-test to compare the conversion rates between the groups and reports the p-value.
* Creates a sampling distribution under the null hypothesis.
* Calculates and displays the 90% confidence interval for the difference in conversion rates.
  
**Logistic Regression:**
* Creates dummy variables for the experiment variable.
* Fits a logistic regression model to predict the conversion rate based on the exposure group.
* Prints the model summary.
