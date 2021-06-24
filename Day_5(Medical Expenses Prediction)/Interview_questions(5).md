



## What does SVM stands for?

- Support vector machines

## What is SVM?

- Support vector machines is a supervised machine learning algorithm which works both on classification and regression problems. It tries to classify data by finding a hyperplane that maximizes the margin between the classes in the training data. Hence, SVM is an example of a large margin classifier.
- The basic idea of support vector machines:
  - Optimal hyperplane for linearly separable patterns
  - Extend to patterns that are not linearly separable by transformations of original data to map into new space(i.e the kernel trick)

## Explain SVM to a non-technical person.

- Suppose you have to construct a bidirectional road. Now you have to make a dividing line. The optimal approach would be to make margins on the sides and draw an equidistant line from both the margins.
- This is exactly how SVM tries to classify points by finding an optimal centre line technically called as hyper plane.

## 3. What is the geometric intuition behind SVM?

- If you are asked to classify two different classes. There can be multiple hyperplanes which can be drawn.

  ![a.png](https://miro.medium.com/max/469/0*j6b6qNc-E0RfBxFj)

- SVM chooses the hyperplane which separates the data points as widely as possible. SVM draws a hyperplane parallel to the actual hyperplane intersecting with the first point of class A (also known as Support Vectors) and another hyperplane parallel to the actual hyperplane intersecting with the first point of class B. SVM tries to maximize these margins. Eventually, this margin maximization improves the model’s accuracy on unseen data.

##  How would explain Convex Hull in light of SVMs?

- We simply build a convex hull for class A and class B and draw a perpendicular on the shortest distance between the closest points of both these hulls.

  ![a.png](https://miro.medium.com/max/338/0*0f3JsP3NsoWhYwKs)

## What do know about Hard Margin SVM and Soft Margin SVM?

- Explanation: If a point Xi satisfies the equation ***Yi(WT\*Xi +b) ≥ 1,\*** then Xi is correctly classified else incorrectly classified. So we can see that if the points are linearly separable then only our hyperplane is able to distinguish between them and if any outlier is introduced then it is not able to separate them. So these type of SVM is called ***hard margin SVM\*** *(since we have very strict constraints to correctly classify each and every data point).*

- To overcome this, we introduce a term ***( ξ )\*** (pronounced as Zeta)

  ![a.png](https://miro.medium.com/max/183/0*Mimj5tNTj0RoCpRv)

  *if ξi= 0, the points can be considered as correctly classified.*

  *if ξi> 0 , Incorrectly classified points.*
## What is Hinge Loss?

- Hinge Loss is a loss function which penalises the SVM model for inaccurate predictions.
- If ***Yi(WT\*Xi +b) ≥ 1\***, hinge loss is ‘**0**’ i.e the points are correctly classified. When  ***Yi(WT\*Xi +b)\* < 1**, then hinge loss increases massively.

- As ***Yi(WT\*Xi +b)\*** increases with every misclassified point, the upper bound of hinge loss {**1- \*Yi(WT\*Xi +b)\***} also increases exponentially.

- Hence, the points that are farther away from the decision margins have a greater loss value, thus penalising those points.

  ![a.png](https://miro.medium.com/max/273/0*ZnoTexvPg-6hGTHB)

  We can formulate hinge loss as **max[0, 1- \*Yi(WT\*Xi +b)\*]**

## Explain the Dual form of SVM formulation?

- The aim of the Soft Margin formulation is to minimize

  ![a.png](https://miro.medium.com/max/131/0*ijBJ9cN63ydw0Nsv)

  subject to

  ![a.png](https://miro.medium.com/max/431/0*W1bCbvkRYDZjtoMU)

- This is also known as the primal form of SVM.

- The duality theory provides a convenient way to deal with the constraints. The dual optimization problem can be written in terms of dot products, thereby making it possible to use kernel functions.

- It is possible to express a different but closely related problem, called its dual problem. The solution to the dual problem typically gives a lower bound to the solution of the primal problem, but under some conditions, it can even have the same solutions as the primal problem. Luckily, the SVM problem happens to meet these conditions, so you can choose to solve the primal problem or the dual problem; both will have the same solution.

  ![a.png](https://miro.medium.com/max/1000/0*d7YVJ-Pb3dj2m-8f)

## What’s the “kernel trick” and how is it useful?

- Earlier we have discussed applying SVM on linearly separable data but it is very rare to get such data. Here, kernel trick plays a huge role. The idea is to map the non-linear separable data-set into a higher dimensional space where we can find a hyperplane that can separate the samples.

  ![a.png](https://miro.medium.com/max/838/0*ZnINGVLyQZfrcZYG)

- It reduces the complexity of finding the mapping function. So, **Kernel function defines the inner product in the transformed space.** Application of the kernel trick is not limited to the SVM algorithm. Any computations involving the dot products (x, y) can utilize the kernel trick.

## Should you use the primal or the dual form of the SVM problem to train a model on a training set with millions of instances and hundreds of features?**

- This question applies only to linear SVMs since kernelized can only use the dual form. The computational complexity of the primal form of the SVM problem is proportional to the number of training instances m, while the computational complexity of the dual form is proportional to a number between m² and m³. So, if there are millions of instances, you should use the primal form, because the dual form will be much too slow.

## Explain about SVM Regression?

- The Support Vector Regression (SVR) uses the same principles as the SVM for classification, with only a few minor differences. First of all, because the output is a real number it becomes very difficult to predict the information at hand, which has infinite possibilities. In the case of regression, a margin of tolerance (epsilon) is set in approximation to the SVM

  ![img](https://miro.medium.com/max/458/0*eXs0bEy10djpwu7d)

## Give some situations where you will use an SVM over a RandomForest Machine Learning algorithm.

  - The main reason to use an SVM instead is that the problem might not be linearly separable. In that case, we will have to use an SVM with a non-linear kernel (e.g. RBF).

  - Another related reason to use SVMs is if you are in a higher-dimensional space. For example, SVMs have been reported to work better for text classification.

## SVM being a large margin classifier, is it influenced by outliers?

- Yes, if C is large, otherwise not.

## In SVM, what is the angle between the decision boundary and theta?

- Decision boundary is a plane having equation Theta1*x1+Theta2*x2+……+c = 0, so as per the property of a plane, it’s coefficients vector is normal to the plane. Hence, the Theta vector is perpendicular to the decision boundary.

## Can we apply the kernel trick to logistic regression? Why is it not used in practice then?

  1. Logistic Regression is computationally more expensive than SVM — O(N³) vs O(N²k) where k is the number of support vectors.
  2. The classifier in SVM is designed such that it is defined only in terms of the support vectors, whereas in Logistic Regression, the classifier is defined over all the points and not just the support vectors. This allows SVMs to enjoy some natural speed-ups (in terms of efficient code-writing) that is hard to achieve for Logistic Regression.

## What is the difference between logistic regression and SVM without a kernel?

- They differ only in the implementation . SVM is much more efficient and has good optimization packages.



## Does SVM give any probabilistic output?

- SVMs do not directly provide probability estimates, these are calculated using an expensive five-fold cross-validation
