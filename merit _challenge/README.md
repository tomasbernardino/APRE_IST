# Challenge for “Merit Prize” 2024/2025
Consider the breast_cancer dataset
data = datasets.load_breast_cancer() with binary target variable y=‘malignant’. Split it 70% for training and 30% for testing.

**1.** Perform logistic regression and indicate the accuracy.

**2.** Perform EM clustering on the training data set with different number k of clusters. Evaluate
the quality of the clusterings using Silhouette. Is the number of clusters correlated with the
quality of clustering? Which is the optimal k?

**3.** Map the test set into probability values of the k-clusters. If you have a data point represented
by a vector of dimension d, you will map it into a vector of dimension:
prob=em_model.predict_proba(X).

**4.**  Perform logistic regression on the mapped data set with the labels of the original test set.
Indicate now the accuracy. Is there a relation between the number of clusters, the cluster
evaluation and the accuracy of the logistic regression model?

**5.** Train an RBF network using the clustering with optimal k from 2).

**6.** Discuss your findings on a (up to) 5 page document.