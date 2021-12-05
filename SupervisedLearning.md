Main use: To classify the target feature based on independent features.
How is it different from Unsupervised Learning: Data is labeled and that is target feature.
What labeled data looks like: Target feature can be binary or multi-values or multi-categories.

General Work Flow:
1. Data Preparation
Data assessment, data cleaning, data reprocessing
Feature Engineering, Feature Selection
3. Modeling
Building, Training, Evaluation, Tuning

Supervised Learning Models: For Classification and Continous Value Prediction
Note. Most model could handle both tasks, but some cannot. E.g. Linear regression is for continous value prediction only, to classify, use Logistic Regression.
Also, Naive Bayes is for classification only, not for continoue value prediction.
**********************************************************************************************************************************************************************
1. Decision Tree
What?
A Trie like structure that contains a seris of questions to direct from 1st question to the last question that leads to a final result.
How to construct the tree?
The feature that split the most data should be at higher level.
To determin which feature split the most data, use Entropy to measure. [Entropy] is how mixed is target feature. The model should compare between features and find those lower the Entropy the most. 
E.g.
A B Target
+ +   0
+ -   0
- -   1
- +   1
In this case, A could reduce the most Entropy when the value of A is different. So the top decision should be asking what is the value of A.

Some common problems of DT:
1. Underfitting - Not very good model when data is small. Not enough information to build a reliable tree.
2. Overfitting - Trie could become too big/too deep that not perform well on new dataset. Should lower the variance or lower the depth of the tree. 
Solution: Lower variance could lower the impact of noise in the training data. Lower the depth of the tree could eliminate the unimportant factors at decision making. 
**********************************************************************************************************************************************************************
2. Naive Bayes
What? 
A probability-based model that uses Bayes probability formula to estimate the likehood of of outcome.
'Naive' means the model has assumed that features are not correlted and independant, which is probabily False in the real world. Therefore, we say it is Naive in reality.
How?
Training the model = finding the values that can be plugged in the Bayes formula.
P(B|A) = P(A|B) * P(B) / P(A)

**********************************************************************************************************************************************************************
3. KNN - K nearest neighbors
**********************************************************************************************************************************************************************
5. SVM
**********************************************************************************************************************************************************************
6. Logistic Regression
**********************************************************************************************************************************************************************
7. Linear Regression
**********************************************************************************************************************************************************************
8. NN / CNN / RNN
