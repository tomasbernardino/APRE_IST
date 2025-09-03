# Homework IV
Consider the accounts.csv dataset. This dataset contains account details
of bank clients, and the target variable y is binary (‘has the client subscribed a term deposit?’).
Select the first 8 features and remove duplicates and null values.



**1.** Normalize the data using MinMaxScaler:
- **a.** Using sklearn, apply k-means clustering (without targets) on the normalized
data with k={2,3,4,5,6,7,8}, max_iter=500 and random_state=42. Plot the
different sum of squared errors (SSE) using the _inertia attribute of k-means
according to the number of clusters.
- **b.** According to the previous plot, how many underlying customer segments
(clusters) should there be? Explain based on the trade-off between the clusters and
inertia
- **c.** Would k-modes be a better clustering approach? Explain why based on the
dataset features.

**2.** Normalize the data using MinMaxScaler:
- **a.** Apply PCA to the data. How much variability is explained by the top 2
components?
- **b.** Apply k-means clustering with k=3 and random_state=42 (all other
arguments as default) and use the original 8 features. Next, provide a scatterplot
according to the first 2 principal components. Can we clearly separate the clusters?
Justify.
- **c.** Plot the cluster conditional features of the frequencies of “job” and ”education”
according to the clusters obtained in the previous question (2b.). Use sns.displot
(see Data Exploration notebook), with multiple="dodge", stat='density',
shrink=0.8 and common_norm=False. Describe the main differences between the
clusters in no more than half a page.