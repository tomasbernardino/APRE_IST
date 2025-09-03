# Homework I
Consider the diabetes.arff dataset, comprising 8 biological
features to classify 768 patients into 2 classes (normal, diabetes).

**1.** ANOVA is a statistical test that can be used to assess the discriminative power of a
single input variable. Using f_classif from sklearn, identify the input variables with the
worst and best discriminative power. Plot their class-conditional probability density
functions.

**2.** Using a stratified 80-20 training-testing split with a fixed seed (random_state=1),
assess in a single plot both the training and testing accuracies of a decision tree with
minimum sample split in and the remaining parameters as default.
Note that split thresholding of numeric variables in decision trees is nondeterministic in sklearn, hence you may opt to average the results using 10 runs per
parameterization.

**3.** Critically analyze these results, including the generalization capacity across settings.

**4.** To deploy the predictor, a healthcare provider opted to learn a single decision tree
(random_state=1) using all available data and ensuring that the maximum depth would be 3
in order to avoid overfitting risks.
- i. Plot the decision tree.
- ii. Explain what characterizes diabetes by identifying the conditional associations
together with their posterior probabilities.