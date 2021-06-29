### **1. What is the life cycle of the data science project?**

- Data Collection
- Exploratory Data Analysis
- Model Training and Testing
- Results Analysis from the models.

![EDA Interview Questions - Data Science Lifecycle](https://lh4.googleusercontent.com/YiovkqJWjoNhzyqwzl2wWxF0eBFWh6PqMPa3QujvUluNB7mn8VsXaP37Jri6z1VFcbm3vbgLVqimcdraMtDqgJPzpRpxyZDWUGlVneaJm3w61s04uSAdIRIG74aJkRtMTHzKxxCN)

### **2. What is the Differentiate between Univariate, Bivariate, and Multivariate analysis?**

- **Univariate** – When we analyze one variable at a time, it is called univariate data analysis. This analysis aims to describe the variable in question and find patterns that exist within it. Example: height of students
- **Bivariate** – Bivariate data involves two different variables. The analysis of this type of data deals with causes and relationships. The investigation determines the relationship between the two variables, where one of the variables is the target variable. Example: temperature and ice cream sales in the summer season.
- **Multivariate** – Analyzing three or more variables together is categorized under multivariate data analysis. It is similar to a bivariate but contains more than one dependent variable.
  Example: data for house price prediction

### **3. Mention the two kinds of target variables for predictive modeling.**

The two kinds of target variables are:

- ***Numerical/Continuous variable\*** – Variables whose values lie within a range, could be any value in that range and the time of prediction, values are not bound to be from the same range too.
  For example: Height of students – 5; 5.1; 6; 6.7; 7; 4.5; 5.11
  Here the range of the values is (4,7)
  And, the height of some new students can/cannot be any value from this range.
- ***Categorical variable\*** – [Variable](https://en.wikipedia.org/wiki/Variable_(research))s that can take on one of a limited, and usually fixed, number of possible values, assigning each individual or other unit of observation to a particular group on the basis of some [qualitative property](https://en.wikipedia.org/wiki/Qualitative_property).
  A categorical variable that can take on exactly two values is termed a [*binary variable*](https://en.wikipedia.org/wiki/Binary_variable) or a dichotomous variable. Categorical variables with more than two possible values are called polytomous variables
  For example: Exam Result: Pass, Fail (Binary categorical variable)
  The blood-type of a person: A, B, O, AB (polytomous categorical variable)

### **4. How to perform univariate analysis for numerical and categorical variables?**

- ***For the Numerical variables:\***
  One can plot a Box and Whiskers plot and KDE plot to better understand the data; below is an example of the Age column plotted using both box and KDE plot.

> ![EDA Interview Questions - Univariate Analysis for Numerical Variable](https://lh6.googleusercontent.com/VkaSw0i8AZ4clzBryU5ynMyJdM9tVTzNSQKvtvPB_DAifxuZt5Y-axc2djX8ZYnbx6NRAfulDQDvcUWiHOLcXfpCSj5SQXa8QevNtoWH1CeOb1E9bC2VYdaopTp4B0vjQS0StzSY)
>
> Box plot and KDE both show that an average population age lies between 25yrs to 50 yrs roughly, and the mean of the population is 38yrs. The left skewness in the KDE plot shows that more population was between 20 and 30 years and very few aged people were in the sample, which could be verified from the box plot too, as the box is aligned more towards the Q1 and not evenly distributed.

 

- ***For the Categorical variables:\***
  Bar plots and Pie Charts are a great way to analyze categorical variables to understand the categorical data. The two plots represent the number (in a bar chart) and proportion (in a pie chart) of individuals opting for Course_types

> ![EDA Interview Questions Univariate Analysis for Categorical Variable](https://lh6.googleusercontent.com/xlnAwGUVydq8OUsgik8AzyjDIDYzAS65hQUwebiWSLrxi1Uhke0obYIAixiyALjSwGO5lq_G-3aAI2-uELTzIdeoJMmxOl4QDZ-dw3yEmnnlVfOwuY5sUV9Vqol8yLGA4HPd9ChA)
>
> Here, the Barplot and Pie chart shows that “Course” Course_Type was highest in number with 51.3 % people subscribing to such courses, followed by “Program” Course_Type, with the least number of “Degree” Course_Type with only 0.3% subscribing to such courses.

 

### **5. How to perform Bivariate analysis for Numerical-numerical, Categorical-Categorical, and Numerical-Categorical variables?**

Univariate analysis is the analysis of one(“uni”) variable and Bivariate Analysis is the analysis of exactly two variables and is one of the simplest forms of statistical analysis, used to find out if there is a relationship between two sets of values.

Though Bivariate analysis can be performed for any two sets of variables, Bivariate analysis is performed using an independent variable and the dependent variable.

- ***Numerical-Numerical\*** – Here, one of the numerical variables is the target variable and the other one is any other independent numerical variable. A Scatter plot is a great way for understanding numerical-numerical variable data relationships. In the example shown, sales is the target numerical variable plotted on the y-axis against user-traffic numerical variables on the x-axis.

> ![bivariate analysis](https://lh4.googleusercontent.com/lsroHGvCXrqBWD7RCGCVZOjumfGE80XXG8hygcJeFHQPXQD6bnXZNXrRI6QsS7nRz1hrOjiVZOdG5AKM4ZinkKDJB-VoK9krWld2YnoXxP5zUrtoNwlHCoLXH0jFhkhpBQRy-60Z)
>
> The scatter plot helps us in understanding that User_Traffic is increasing linearly as the Sales going up, or we can also say, as User_traffic increases the sales also increase linearly.

 

- ***Categorical-Categorical\*** – One of the Categorical variables is the target variable and another one can be an independent categorical variable. In the example below, the target variable is about default next month represented by either 0 or 1 against the education categorical independent variable.

> ![Categorical-Categorical](https://lh6.googleusercontent.com/XTM-Dbhztt_nWLUjReKkJ78Cj1TQj8Rz787pnZgCGdi5ff5R0nDlI7p0CMw38a44hbb8LV5VuY4r-YLBD7yRVOVqBK6vxK7n9lpSb8ZSM56iARDWdfcDXbp77S4EgoX2DGkrim55)
>
> ![Categorical-Categorical default payment](https://lh6.googleusercontent.com/NyOays-fejehoIAKIJo05Up7nD_KKyV0euTmuSdJpqfk_K1Idt4cP196wfFClV5kaUacT8rDMDCItcgL5dhvYXGPj1UFq4NJCC7IFmKXr-DyrfYxbotUWjQJzrQgXeNijhUI5N7T)
>
> The Bivariate for categorical and categorical variables can easily be done with the help of double bar or stacked bar charts. In the above example, we can see how defaulters( represented by 1: orange color) are highest in number for High School then University and then for Others category even when they are so less in number.

- ***Numerical-Categorical\*** – Here, the target variable is either categorical or numerical, and in such case, bar plots or strip plots are a great way of understanding the data. Below is an example for a bar and strip plot where sales which is the numerical variable(target) is on the y-axis and course_domain is the categorical variable represented on the x-axis.

> ![Numerical-Categorical](https://lh5.googleusercontent.com/aMLOpR3PNpFM8GDrQhDr2k753ISRg-oryx3K4MdjMfdZRPZPyGkoDj9QH_PCrY9bbVb4mpuNaA3Z3eDXM4CGVFvDYHQ2SFkZw27HxR6_4B9CPZW3AhGfjx26ELG292f9PCS_OI-y)
>
> Here, Bar Plot helps in understanding that sales for “Business” course_domain give the highest sales followed by Finance, the Development and the least sales from Software course_domain. The business gives the highest sales, and the strip plot corresponding to the same helps in understanding the minimum value of sale for this category is quite high if compared with others and maximum sales value is low than others, but at last, gives the most sales.

 

### **6. What are the different tests that are used for verifying analysis/hypothesis for numerical-numerical, categorical-categorical, and numerical-categorical variables?**

- For ***numerical-numerical\*** data, the correlation matrix is used for understanding how much are independent variables correlated with the target variable.

> ![statistical tests](https://lh6.googleusercontent.com/G3aCnuLwzfOsK4tgPXOXpnHw9B4325is11WmZSZolIAjozNAA7kWoriyR7NM1oWjYPrvO8-A72teTqd7aQ-TkVW4ZXNtyZwC6KETaZ1yDMrzUWrn6uxcIC1h5ZhvO7ZGvl-vuQPM)
>
> 

- For ***Categorical-Numerical\*** variable testing, the T-test or Z-test is mostly used depending upon whether the number of observations is below(Z-test) or above 30(T-test). And, if in the category column, the number of categories is more the Anova test is preferred over T/Z-test.
  These tests are performed using p values and further helping in accepting or rejecting the null hypothesis made for the test columns.
- For ***Categorical-Categorical\*** variables, the chi sq test is used. There are two types of chi-square tests.
  Chi-square *goodness of fit test* determines if [sample](https://www.statisticshowto.com/sample/) data matches a [population](https://www.statisticshowto.com/what-is-a-population/).
  A *chi-square test for independence* tests to see whether distributions of [categorical variables](https://www.statisticshowto.com/what-is-a-categorical-variable/) differ from each other.
  A *very small chi-square test statistic* means that your observed data fits your expected data extremely well. In other words, there is a relationship. A *very large chi-square test statistic* means that the data does not fit very well. In other words, there isn’t a relationship.



***Note:\*** If the p-value ≤ 0.05, that indicates strong evidence against the null hypothesis; so you reject the null hypothesis. And if the p-value > 0.05, indicates weak evidence against the null hypothesis, so you accept the null hypothesis.

 



For more understanding of tests, one should be thoroughly familiar with basic statistics concepts.

 

### **7. During the data preprocessing step, how should one treat missing/null values?** **How will you deal with them?**

- **There are three types of missing data:**

1. ***MCAR**:* Missing Completely At Random. It is the highest level of randomness. This means that the variable with the missing values is not dependent on any other variable/feature values. An example of MCAR is a weighing scale that ran out of batteries. Some of the data will be missing simply because of bad luck.
2. ***MAR:*** Missing At Random. This means that the missing values in any column/feature are dependent on other feature values. For example, when placed on a soft surface, a weighing scale may produce more missing values than when placed on a hard surface. Such data are thus not MCAR. If, however, we know the surface type and if we can assume MCAR *within* the type of surface, then the data are MAR.
3. ***MNAR:*** Missing Not At Random. Missing not at random data is a more serious issue and in this case, it is advisable to check the data gathering process further and understand the reason behind missing data. For example, the weighing scale mechanism may wear out over time, producing more missing data as time progresses, but we may fail to note this. If the heavier objects are measured later in time, then we obtain a distribution of the measurements that will be distorted. MNAR includes the possibility that the scale produces more missing values for the heavier objects (as above). Another example, if most people refuse to answer some particular questions, what was the reason? Was it an unclear question or some other issue? This helps in making better business decisions and saves time to do modeling as a basic issue might lie here.

- Now that we have seen what type of missing data exists in our dataset, we should check what percentage of missing information exists for features.
- If the missing data type is Missing completely at random, then the missing percentage of even 20 can be ignored, but if it is the other two types of missing data, missing values should not be ignored.
- If missing data is MCAR with a high percentage value, they are advised to be dropped and not to be included in the modeling part. Also, if missing data is MAR with a high percentage they can be dropped, but if the percentage is low in MAR then they shouldn’t be dropped. Features with a missing percentage of more than 10% are mostly advisable not to be included in the modeling section.
- Now that unnecessary features have been dropped or ignored, the features still having missing values should be treated using Imputation. Imputation is the process of filling the missing data by some statistical methods. Imputation is useful as it replaces the missing data with an estimated value based on other available information.
- If the missing values in a column or feature are numerical, the values can be imputed by the mean of the complete cases of the variable. Mean can be replaced by median if the feature is suspected to have outliers. For a categorical feature, the missing values could be replaced by the mode of the column.

### 

### **8. What is an outlier and how to identify them?**

An **outlier** is an observation point that is distant from others. They sometimes represent errors in measurement, bad data collection, or simply show variables not considered when collecting the data or can be a part of the data distribution as well. And hence they might skew the results and give insights accordingly.
There is no one method to detect outliers as every dataset is different. One thing which should be practiced in detecting outliers is that you(data analyst) can inspect the unfiltered, basic observations and decide whether a value is an outlier or not based on the domain knowledge.

After performing the above step, one can understand the data and look at outliers using these two methods:

> ![Outlier](https://lh4.googleusercontent.com/jjPQ5oVztYOIX9_Vo3RgqbzuTqM1CK6rPU_qC0OEvfxiLjeP5S0F_SKpHHI3AOp471hlSN6JZD23V7R-Dtjx6284GI9CGYjaHCRLbe8ImmvVoD4feCCGGqKEPDSMSXUBGNkAWU5x)
>
> 

 

 

> ![Scatter plot](https://lh6.googleusercontent.com/G4U_01a7-5iLqqyJ0avXGUfrkbdD-T0MEDVrPtR70y3odoHN_UsS0vf7BuyvNF3OFkTBL6JVR1WD39Adat8c1UtKgf3i0FxzaGeeG4G_HWpTO6MziPP1sBquofd2Em2eeD_runoi)
>
> 

Outliers can be dropped only if it is a garbage value. Example: height of an adult = 0 ft. This cannot be true, as the height cannot be a string value. In this case, outliers can be removed. If the outliers have extreme values, they can be removed. For example, if all the data points are clustered between zero to 10, but one point lies at 100, then we can remove this point. If you cannot drop outliers, you can normalize the data. This way, the extreme data points are pulled to a similar range.

### 

### **9. How can the data be normalized?**

Data can be normalized by either transforming the data or by scaling the data down in a particular range.

- ***Transformation\* –** If the data is left-skewed, log transformation is the best way to make them behave in the normal distribution, and if the data is right-skewed, exponential transformation helps in transforming them into a normal distribution.

- *Scaling* – 

  There are two scalers used on a wide base

  - Normalization

     

    (Min-Max Scaler): This scales down the data between 0 and 1 range where minimum value corresponds to 0 and maximum was 1.

    > A value is normalized as follows:y = (x – min) / (max – min), where the minimum and maximum values pertain to the value x being normalized

- - Standardization (Standard Scaler): This scaler helps in making a normal distribution in standard normal distribution where the mean is represented by 0 and the standard deviation is represented by 1.

> A value is standardized as follows: y = (x – mean) / standard_deviation

 
