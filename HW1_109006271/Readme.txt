This dataset [1] is the result of a chemical analysis of wines grown in the same
region in Italy but derived from three different cultivars. The analysis determined the
quantities of 13 constituents found in each of the three types of wines.
That is, there are 3 types of wines and 13 different features of each instance. In
this problem, you will implement the Maximum A Posteriori probability (MAP) of the
classifier for 60 instances with their features.

There are a total 483 instances in wine.csv. The first column is the label (0, 1, 2)
of type and other columns are the detailed values of each feature. Information of each
feature:
1. Alcohol
2. Malic acid
3. Ash
4. Alcalinity of ash
5. Magnesium
6. Total phenols
7. Flavanoids
8. Non Flavonoid phenols
9. Proanthocyanins
10. Color intensity
11. Hue
12. OD280/OD315 of diluted wines
13. Proline

Assume that all the features are independent and the distribution of them is Gaussian
distribution.


1. Please split wine.csv into training data and test data. When splitting, please
randomly select 20 instances of each category as testing data. Then save the training
dataset as train.csv and testing dataset as test.csv. (423 instances for training and 60
instances for testing.)

2.To evaluate the posterior probabilities, you need to learn likelihood functions
and prior distribution from the training dataset. Then, you should calculate the
accuracy rate of the MAP detector by comparing to the label of each instance in the
test data. Note that the accuracy rate will be different depending on the random
result of splitting data, but it should exceed 90% overall. (Please screenshot the
result and add corresponding comments in your code to describe how you obtain
the posterior probability in your report.)

3.  Please plot the PCA visualized result of testing data and briefly describe the
role of PCA and how it works in your report. (You can directly use the built-in PCA
function to get visualized result.)

4. Please discuss the effect of prior distribution on the posterior probabilities in
your report.

5. The confusion matrix can help us understand the performance of the
classifier on different categories. Please calculate and plot the confusion matrix for
your test data and briefly discuss your results in your report. An example of
confusion matrix visualization result is shown in Fig.1. (You can directly use the
built-in function to calculate and plot confusion matrix.)