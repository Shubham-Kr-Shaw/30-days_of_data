





## Discuss 'Naive' in a Naive Bayes algorithm?

- The Naive Bayes Algorithm model is based on the Bayes Theorem. It describes the probability of an event. It is based on prior knowledge of conditions which might be related to that specific event.

## **Why is Naive Bayes naive?**

- Naive Bayes is a machine learning implementation of [Bayes Theorem](http://machinelearningspecialist.com/machine-learning-interview-questions-q6-bayes-theorem/).  It is a classification algorithm that predicts the probability of each data point belonging to a class and then classifies the point as the class with the highest probability.

- It is naive because while it uses conditional probability to make classifications, the algorithm simply assumes that all features of a class are independent.  This is considered naive because, in reality, it is not often the case.  The upside is that the math is simpler, the classifier runs quicker, and the results are often quite good for certain problems.

## What is conditional probability?

- conditional probability is a measure of the probability of an event occurring, given that another event (by assumption, presumption, assertion or evidence) has already occurred. If the event of interest is *A* and the event *B* is known or assumed to have occurred, "the conditional probability of *A* given *B*", or "the probability of *A* under the condition *B*", is usually written as P(*A*|*B*),or sometimes P*B*(*A*) or P(*A*/*B*). For example, the probability that any given person has a cough on any given day may be only 5%. But if we know or assume that the person is sick, then they are much more likely to be coughing. For example, the conditional probability that someone unwell is coughing might be 75%, in which case we would have that P(Cough) = 5% and P(Cough|Sick) = 75%.

## What is Bayes’ Theorem?

- Bayes’ Theorem gives us the probability of an event actually happening by combining the conditional probability given some result and the prior knowledge of an event happening.

- Conditional probability is the probability that something will happen, given that something has a occurred.  In other words, the conditional probability is the probability of X given a test result or P(X|Test).  For example, what is the probability an e-mail is spam given that my spam filter classified it as spam.

- The prior probability is based on previous experience or the percentage of previous samples.  For example, what is the probability that any email is spam.

- *Formally*

![img](http://machinelearningspecialist.com/wp-content/uploads/2017/07/bayes-300x78.png)

- - P(A|B) = Posterior probability = Probability of A given B happened
  - P(B|A) = Conditional probability = Probability of B happening if A is true
  - P(A) = Prior probability = Probability of A happening in general
  - P(B) = Evidence probability = Probability of getting a positive test

## What are the types of Naive Bayes Classifier?

There are several types of Naive Bayes classifiers.  Which one you use will depend on the features you are working with. 

- The different types are:
  - Gaussian NB – use when you have continuous feature values.  This classifier assumes each class is normally distributed.
  - MultiNomial NB – good for text classification.  This classifier treats each occurrence of a word as an event.
  - Bernoulli NB – use when you have multiple features that are assumed to be binary.  This classifier can be used for text classification but the features must be binary.  For text classification, the features can be set as a word is in the document or not in the document.

## What are the advantages and dis-advantages of Naive Bayes Classification?

*Advantages*

- Can successfully train on small data set.
- Good for text classification, good for multi class classification.
- Quick and simple calculation since it is naive.

*Disadvantages*

- Can’t learn the relationship among the features because assumes feature independence.
- Continuous feature data is assumed to be normally distributed.



## Which language is best for text analytic? R or Python?

- Python will more suitable for text analytic as it consists of a rich library known as pandas. It allows you to use high-level data analysis tools and data structures, while R doesn't offer this feature.



## Explain the steps for a Data analytics project?

- The following are important steps involved in an analytics project:
  - Understand the Business problem
  - Explore the data and study it carefully.
  - Prepare the data for modelling by finding missing values and transforming variables.
  - Start running the model and analyse the Big data result.
  - Validate the model with new data set.
  - Implement the model and track the result to analyse the performance of the model for a specific period.




## List out the libraries in Python used for Data Analysis and Scientific Computations.

- SciPy
- Pandas
- Matplotlib
- NumPy
- SKLearn
- Seaborn



