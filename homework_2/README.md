# Homework II
Consider the heart-disease.csv dataset.
Using sklearn, apply a 5-fold stratified cross-validation with shuffling (random_state=0) for the
assessment of predictive models along this section.


**1.** Compare the performance of a 𝑘𝑁𝑁 with 𝑘 = 5 and a naïve Bayes with Gaussian assumption (consider all remaining parameters as default):
- **a.** Plot two boxplots with the fold accuracies for each classifier. Is there one
more stable than the other regarding performance? Why do you think that is the
case? Explain.

- **b.** Report the accuracy of both models, this time scaling the data with a
Min-Max scaler before training the models. Explain the impact that this
preprocessing step has on the performance of each model, providing an
explanation for the results.
- **c.** Using scipy, test the hypothesis “the 𝑘𝑁𝑁 model is statistically superior to
naïve Bayes regarding accuracy”, asserting whether it is true.

**2.** Using a 80-20 train-test split, vary the number of neighbors of a 𝑘𝑁𝑁 classifier using
𝑘 = {1, 5, 10, 20, 30}. Additionally, for each 𝑘, train one classifier using uniform weights
and distance weights.
- **a.** Plot the train and test accuracy for each model.
- **b.** Explain the impact of increasing the neighbors on the generalization ability of
the models.

**3.** Considering the unique properties of the heart-disease.csv dataset, identify two
possible difficulties of the naïve Bayes model used in the previous exercises when learning
from the given dataset.