
# Interview Questions and answers:-


## What is machine learning?
- Machine learning is a branch of AI focused on building applications that learn from data and improve their accuracy over time without being programmed to do so. 

## What is the relation between Al, ML & DL?

![img](https://www.aimlmarketplace.com/images/Startup-images-1/difference-between-ai-ml-dl.png)



## What are the different types of machine learning ? Explain each of them.
- These are three types of machine learning: supervised learning, unsupervised learning, and reinforcement learning.

  - **Supervised Learning** is one of the most basic types of machine learning. In this type, the machine learning algorithm is trained on labelled data.

  - **Unsupervised machine learning** holds the advantage of being able to work with unlabelled data. This means that human labour is not required to make the dataset machine-readable, allowing much larger datasets to be worked on by the program.

  - **Reinforcement Learning** directly takes inspiration from how human beings learn from data in their lives. It features an algorithm that improves upon itself and learns from new situations using a trial-and-error method. Favourable outputs are encouraged or ‘reinforced’, and non-favourable outputs are discouraged or ‘punished’.

  - ##### The followup question can be from any of the 3 types.
  
    
  


## What is machine learning algorithms?
- Machine learning algorithms are programs (maths and logic) that adjust themselves to perform better as they are exposed to more data. The “learning” part of machine learning means that those programs change how they process data over time, much as humans change how they process data by learning.
- In machine learning, algorithms are 'trained' to find patterns and features in massive amounts of data in order to make decisions and predictions based on new data. The better the algorithm, the more accurate the decisions and predictions will become as it processes more data.

##  What are the differences between supervised and unsupervised learning?

|                     Supervised Learning                      |                    Unsupervised Learning                     |
| :----------------------------------------------------------: | :----------------------------------------------------------: |
|            Uses known and labelled data as input.            |                Uses unlabelled data as input.                |
|        Supervised learning has a feedback mechanism.         |       Unsupervised learning has no feedback mechanism.       |
| The most commonly used supervised learning algorithms are decision trees, logistic regression, and support vector machine. | The most commonly used unsupervised learning algorithms are k-means clustering, hierarchical clustering, and apriori algorithm. |



### Tomorrow we will see some algorithm specific questions on supervised learning.

### Please post your questions in the comment section, I will answer it, tomorrow.


### There are lots of basic and advance questions are there which will be coming up, stay tuned.



# Notes of today's Project.
## Breast Cancer type prediction.

### Problem Statement

- We have the dataset of the patients with breast cancer, With it's analysis we can predict and diagnose patients, and generate the report which will show which type of breast cancer they are suffering from and also recommend the immediate actions to be taken on the basis of their cancer type.


### Data set description
- Download dataset from https://www.kaggle.com/uciml/breast-cancer-wisconsin-data
  
#### Attribute Information:

- ID number
- Diagnosis (M = malignant, B = benign)

- Ten real-valued features are computed for each cell nucleus:
  - Radius (mean of distances from centre to points on the perimeter)
  - Texture (standard deviation of Gray-scale values)
  - Perimeter
  - Area
  - Smoothness (local variation in radius lengths)
  - Compactness (perimeter^2 / area - 1.0)
  - Concavity (severity of concave portions of the contour)
  - Concave points (number of concave portions of the contour)
  - Symmetry
  - Fractal dimension ("coastline approximation" - 1)

- The mean, standard error and "worst" or largest (mean of the three largest values) of these features were computed for each image,resulting in 30 features. For instance, field 3 is Mean Radius, field 13 is Radius SE, field 23 is Worst Radius.

- All feature values are recorded with four significant digits.

- Missing attribute values: none

- Class distribution: 357 benign, 212 malignant
