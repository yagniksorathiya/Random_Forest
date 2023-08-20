# Random_Forest

## Problem Statement

**Company Data :**

A cloth manufacturing company is interested to know about the segment or attributes causes high sale. 

Approach - A Random Forest can be built with target variable Sales (we will first convert it in categorical variable) & all other variable will be independent in the analysis.  

**Fraud check :**

Use Random Forest to prepare a model on fraud data 

treating those who have taxable_income <= 30000 as "Risky" and others are "Good"

# ➳ Random Forest Algorithm

![Random-Forest-Algorithm](https://github.com/yagniksorathiya/Random_Forest/assets/129974278/868cee54-813e-429e-86d9-7d8622567cfd)

Random Forest is a popular machine learning algorithm that belongs to the supervised learning technique. It can be used for both Classification and Regression problems in ML. It is based on the concept of **ensemble learning**, which is a process of combining multiple classifiers to solve a complex problem and to improve the performance of the model.

As the name suggests, **"Random Forest is a classifier that contains a number of decision trees on various subsets of the given dataset and takes the average to improve the predictive accuracy of that dataset."** Instead of relying on one decision tree, the random forest takes the prediction from each tree and based on the majority votes of predictions, and it predicts the final output.

**The greater number of trees in the forest leads to higher accuracy and prevents the problem of overfitting.** 

The below diagram explains the working of the Random Forest algorithm:

![Ensemble-of-decision-trees](https://github.com/yagniksorathiya/Random_Forest/assets/129974278/230844ef-da48-46b8-910c-a1697f7be646)

      **NOTE: Majority voting for classification and averaging for regression.**


## ↳ Assumptions for Random Forest

Since the random forest combines multiple trees to predict the class of the dataset, it is possible that some decision trees may predict the correct output, while others may not. But together, all the trees predict the correct output. Therefore, below are two assumptions for a better Random forest classifier:

+ There should be some actual values in the feature variable of the dataset so that the classifier can predict accurate results rather than a guessed result.

+ The predictions from each tree must have very low correlations.

## ↳ Why use Random Forest?

Below are some points that explain why we should use the Random Forest algorithm:

+ It takes less training time as compared to other algorithms.

+ It predicts output with high accuracy, even for the large dataset it runs efficiently.

+ It can also maintain accuracy when a large proportion of data is missing.

## ↳ How does Random Forest algorithm work?

Random Forest works in two-phase first is to create the random forest by combining N decision tree, and second is to make predictions for each tree created in the first phase.

The Working process can be explained in the below steps and diagram:

**Step-1:** Select random K data points from the training set.

**Step-2:** Build the decision trees associated with the selected data points (Subsets).

**Step-3:** Choose the number N for decision trees that you want to build.

**Step-4:** Repeat Step 1 & 2.

**Step-5:** For new data points, find the predictions of each decision tree, and assign the new data points to the category that wins the majority votes. 

## ↳ Advantages of Random Forest

+ Random Forest is capable of performing both Classification and Regression tasks.

+ It is capable of handling large datasets with high dimensionality.

+ It enhances the accuracy of the model and prevents the overfitting issue.

## ↳ Disadvantages of Random Forest

+ Although random forest can be used for both classification and regression tasks, it is not more suitable for Regression tasks.

# ➳ Ensemble learning techniques

**Bagging :**

Bagging, an ensemble technique is known by the name Bootstrap Aggregation. Bagging chooses a randomized subset from the data set. Then Original Data is randomly selected and is given parallelly to different models(weak learners or base learners) but with replacement. Replacement means there is a high possibility that the data sample could be repeated. This is called row sampling and when this step is done with replacement is called bootstrap. After this, each model is trained for generating results. Then results are combined and majority voting is done to generate the final output. This is known as aggregation.  

**Boosting :**

Boosting is an ensemble learning technique that random forest use. Like bagging boosting combines weak learners to get the final outcome. Unlike the bagging process boosting follow the sequential process.In which we have sequential learners where every model learns from the mistakes of the previous model and corrects them as shown in fig.

**Boosting techniques :**

+ Gradient Boosting

+ AdaBoost algorithm (Adaptive Boosting)

+ XGBoost

![bagging   boosting](https://github.com/yagniksorathiya/Random_Forest/assets/129974278/70db28f4-7b51-4db0-886a-e010bb521e3a)

## ↳ Understanding these techniques with a real-life analogy

**Bagging :**

Suppose after interviewing a candidate four interviewers gave their feedback parallelly and three selected the candidate and one rejected it. So we can say that candidate is selected(majority wins!!). So this will follow the bagging technique.

**Boosting :**

But if the first interviewer is giving his outcome and forwarding the feedback to the second interviewer and the second interviewer learning from the feedback of the first interviewer and so on.

**Pros of Random forest Algorithm :**

+ The random forest algorithm can be used to solve both classification and regression problems.

+ The performance of a random forest algorithm is better than other algorithms on small datasets which may contain outliers.

+ Random Forest also has low variance which means that it usually generates similar predictions for different instances (samples) from the same class.

**Cons of Random forest Algorithm :**

+ The random forest algorithm suffers from overfitting

+ It is computationally expensive. It can take up to 100 times more computation time than gradient-boosted trees (GBT) when it comes to the training process.


      **Note: To better understand the Random Forest Algorithm, you should have knowledge of the Decision Tree Algorithm.**    
