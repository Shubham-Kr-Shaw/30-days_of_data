## Which one is your favourite ML algorithm?
### or 
## Choose any ML algorithm which you know best?
- Answer of this question is compleatly of your choice but which ever you choose you should know each and every part of it.
- The follow up question will be on that perticular algorithm.
- Some ML algorithms is discussed below.

## What are the different type of Regression Algorithms?
- Linear Regression
- Logistic Regression
- Polynomial Regression
- Ridge Regression
- Lasso Regression
- Bayesian Linear Regression

## What is linerar regression?
- In simple words in linear regression we try to fit a linear straight line between feature(independent) and target(dependent) variable as a relationship. We use it when the target variables are contionus.
- Our aim is to keep the error(Root Mean Squared Error) minimum while fitting the line.

## What are the assumptions of linear regression?
- Linear relationship : There should be a linear and additive relationship between dependent (response) variable and independent (predictor) variable(s). A linear relationship suggests that a change in response Y due to one unit change in X¹ is constant, regardless of the value of X¹. An additive relationship suggests that the effect of X¹ on Y is independent of other variables.

- No or little multicollinearity : The independent variables should not be correlated. Absence of this phenomenon is known as multicollinearity.

- No auto-correlation : There should be no correlation between the residual (error) terms. Absence of this phenomenon is known as Autocorrelation.

- Homoscedasticity :The error terms must have constant variance. This phenomenon is known as homoskedasticity. The presence of non-constant variance is referred to heteroskedasticity.

- Multivariate normality : The error terms must be normally distributed.
#### How to deal with all this if it is not there will be discussed on some other day.

## What is Random Forest ?
- Random Forest or random decision forests are a learning method for classification, regression by making multiple decision tree using random samples from training data.

## What does random mean in Random forest?
- Random forest adds additional randomness to the model, while growing the trees. Instead of searching for the most important feature while splitting a node, it searches for the best feature among a random subset of features.

### What are the steps to follow while implementing Random Forest.
- Take the original dataset and take random sub-datasets.
- Implement decision tree on the random sub-datasets.
- As we get different predictions from different decision tree we need to take the result which is most relevent.
- For taking the most appropriate result we need to use different methods for different type of problems:
    - For classification we take prediction which has been given by maximum no of decision trees.
    - For regression as we have got a continous value we will take the average of the predictions given by the decision trees.

## What is KNN(K-Nearest Neighbor)?
- KNN is a supervised ML Algorithm that performes both classification and regression tasks using the numbers(K) of neighbors(Nearest).

## What is K in KNN?
'K' in KNN is a parameter that refers to the number of nearest neighbours to include in the majority of the voting process.

### Steps to implement KNN:
- Geting data.
- Defining K Neighbors.
- Calculating the neighbor's distance.
- Assigning new instace to majority of neighbors.

#### How to calculate distance.
- Euclidian Distance.
    - The Euclidean distance between two points in Euclidean space is the length of a line segment between the two points. It can be calculated from the Cartesian coordinates of the points using the Pythagorean theorem, therefore occasionally being called the Pythagorean distance.
- Manhatton distance.
    - The distance between two points measured along axes at right angles. In a plane with p1 at (x1, y1) and p2 at (x2, y2), it is |x1 - x2| + |y1 - y2|. 
    
     
# Notes of today's Project.

### Problem Statement
- To Track COVID-19 vaccination in the World, answer instantly to your questions:
- Which country is using what vaccine?
- In which country the vaccination programme is more advanced?
- Where are vaccinated more people per day? But in terms of percent from entire population ?

### Data set discription
- Data is collected daily from Our World in Data GitHub repository for covid-19, merged and uploaded.

#### Attribute Information:

- Country- this is the country for which the vaccination information is provided.

- Country ISO Code - ISO code for the country.

- Date - date for the data entry; for some of the dates we have only the daily vaccinations, for others, only the (cumulative) total.

- Total number of vaccinations - this is the absolute number of total immunizations in the country.

- Total number of people vaccinated - a person, depending on the immunization scheme, will receive one or more (typically 2) vaccines; at a certain moment, the number of vaccination might be larger than the number of people.

- Total number of people fully vaccinated - this is the number of people that received the entire set of immunization according to the immunization scheme (typically 2); at a certain moment in time, there might be a certain number of people that received one vaccine and another number (smaller) of people that received all vaccines in the scheme.

- Daily vaccinations (raw) - for a certain data entry, the number of vaccination for that date/country.

- Daily vaccinations - for a certain data entry, the number of vaccination for that date/country.

- Total vaccinations per hundred - ratio (in percent) between vaccination number and total population up to the date in the country.

- Total number of people vaccinated per hundred - ratio (in percent) between population immunized and total population up to the date in the country.

- Total number of people fully vaccinated per hundred - ratio (in percent) between population fully immunized and total population up to the date in the country.

- Number of vaccinations per day - number of daily vaccination for that day and country.

- Daily vaccinations per million - ratio (in ppm) between vaccination number and total population for the current date in the country.

- Vaccines used in the country - total number of vaccines used in the country (up to date).

- Source name - source of the information (national authority, international organization, local organization etc.).

- Source website - website of the source of information.


# Summery 

## Covaxin is used globally.
## In India Total Vaccination and People Vaccination rate is very high.
## India Secured 4th rank in Globally Total Vaccination Country list .
## India Secured 3rd rank in Globally Daily Vaccination Country list.
