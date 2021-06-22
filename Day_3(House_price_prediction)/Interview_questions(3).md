





## What is Decision Tree algorithm?

- A decision tree is a popular supervised machine learning algorithm. It is mainly used for Regression and Classification. 
- It allows breaks down a dataset into smaller subsets.
- The decision tree can able to handle both categorical and numerical data.
- A decision tree is a tree in which every node specifies a test of some attribute of the data and each branch descending from that node corresponds to one of the possible values for this attribute.

## To which kind of problems are decision trees most suitable?
- Decision trees are most suitable for tabular data.
- The outputs are discrete.
- Explanations for decisions are required.
- The training data may contain errors.
- The training data may contain missing attribute values.

## On what basis is an attribute selected in the decision tree for choosing it as a node?

- Attribute selection is done using Information Gain in decision trees. The attribute with maximum information gain is selected.

## What is Information Gain? What are its disadvantages?

- Information gain is the reduction in entropy due to the selection of an attribute. 
- Information gain ratio biases the decision tree *against* considering attributes with a large number of distinct values which might lead to overfitting. 
- In order to solve this problem, information gain ratio is used.

## What is the inductive bias of decision trees?

- Shorter trees are preferred over longer trees. Trees that place high information gain attributes close to the root are preferred over those that do not.

## How does a decision tree handle continuous attributes?

- By converting continuous attributes to a threshold-based Boolean attribute. The threshold is decided by maximising the information gain.

## How does a decision tree handle missing attribute values?

- One way to assign the most common value of that attribute to the missing attribute value. The other way is to assign a probability to each of the possible values of the attribute based on other samples.

## What are the different types of nodes in Decision Trees.

- The Decision Tree consists of the following different types of nodes:
  - **1. Root node:** It is the top-most node of the Tree from where the Tree starts.
  - **2. Decision nodes:** One or more Decision nodes that result in the splitting of data into multiple data segments and our main goal is to have the children nodes with maximum homogeneity or purity.
  - **3. Leaf nodes:** These nodes represent the data section having the highest homogeneity.

##  What Pruning in Decision Trees? Why be we do it?

- After we create a Decision Tree we observe that most of the time the leaf nodes have very high homogeneity i.e., properly classified data. However, this also leads to overfitting. Moreover, if enough partitioning is not carried out then it would lead to underfitting.

- Hence the major challenge that arises is to find the optimal trees which result in the appropriate classification having acceptable accuracy. So to cater to those problems we first make the decision tree and then use the error rates to appropriately prune the trees.

## **What do you understand by Pruning in a Decision Tree?**

When we remove sub-nodes of a Decision node, this process is called pruning or the opposite process of splitting. The two techniques which are widely used for pruning are- Post and Pre Pruning.

**Post Pruning:**

- This type of pruning is used after the construction of the Decision Tree.
- This technique is used when the Decision Tree will have a very large depth and will show the overfitting of the model.
- It is also known as backward pruning.
- This technique is used when we have an infinitely grown Decision Tree.

**Pre Pruning:**

- This technique is used before the construction of the Decision Tree.
- Pre-Pruning can be done using Hyperparameter tuning.
- Overcome the overfitting issue.

## **List down some popular algorithms used for deriving Decision Trees along with their attribute selection measures.**

- Some of the popular algorithms used for constructing decision trees are:
  - **1.** **ID3 (Iterative Dichotomiser):** Uses Information Gain as attribute selection measure.
  - **2.** **C4.5 (Successor of ID3):**  Uses Gain Ratio as attribute selection measure.
  - **3. CART (Classification and Regression Trees)** – Uses Gini Index as attribute selection measure.

## What are the advantages of the Decision Trees?

**1. Clear Visualization:** This algorithm is simple to understand, interpret and visualize as the idea is mostly used in our daily lives. The output of a Decision Tree can be easily interpreted by humans.

**2. Simple and easy to understand:** Decision Tree works in the same manner as simple if-else statements which are very easy to understand.

**3.** This can be used for both classification and regression problems.

**4.** Decision Trees can handle both continuous and categorical variables.

**5. No feature scaling required:** There is no requirement of feature scaling techniques such as standardisation and normalization in the case of Decision Tree as it uses a rule-based approach instead of calculation of distances.

**6. Handles nonlinear parameters efficiently:** Unlike curve-based algorithms, the performance of decision trees can’t be affected by the Non-linear parameters. So, if there is high non-linearity present between the independent variables, Decision Trees may outperform as compared to other curve-based algorithms.

**7.** Decision Tree can automatically handle missing values.

**8.** Decision Tree handles the outliers automatically, hence they are usually robust to outliers.

**9. Less Training Period:** The training period of decision trees is less as compared to ensemble techniques like Random Forest because it generates only one Tree unlike the forest of trees in the Random Forest.

## What are the disadvantages of the Decision Trees?

**1. Overfitting:** This is the major problem associated with the Decision Trees. It generally leads to overfitting of the data which ultimately leads to wrong predictions for testing data points. it keeps generating new nodes in order to fit the data including even noisy data and ultimately the Tree becomes too complex to interpret. In this way, it loses its generalization capabilities. Therefore, it performs well on the training dataset but starts making a lot of mistakes on the test dataset.

**2. High variance:** As mentioned, a Decision Tree generally leads to the overfitting of data. Due to the overfitting, there is more likely a chance of high variance in the output which leads to many errors in the final predictions and shows high inaccuracy in the results. So, in order to achieve zero bias (overfitting), it leads to high variance due to the bias-variance tradeoff.

**3. Unstable:** When we add new data points it can lead to regeneration of the overall Tree. Therefore, all nodes need to be recalculated and reconstructed.

**4. Not suitable for large datasets:** If the data size is large, then one single Tree may grow complex and lead to overfitting. So in this case, we should use Random Forest instead, an ensemble technique of a single Decision Tree.



# Notes of today's Project.

## House Price Prediction Using Multiple Linear Regression

### Problem Statement
- Consider a real estate company that has a dataset containing the prices of properties in the Delhi region. It wishes to use the data to optimise the sale prices of the properties based on important factors such as area, bedrooms, parking, etc.

- To identify the variables affecting house prices, e.g. area, number of rooms, bathrooms, etc.

- To create a linear model that quantitatively relates house prices with variables such as number of rooms, area, number of bathrooms, etc.

- To know the accuracy of the model, i.e. how well these variables can predict house prices.

### Data set description
- Data is collected from https://www.kaggle.com/ashydv/housing-dataset .

