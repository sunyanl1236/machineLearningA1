## Github Repo URL
https://github.com/sunyanl1236/machineLearningA1.git

## Description
IDE: Visual Studio Code
Extension: Python, Vetur

Use the [scikit-learn](https://scikit-learn.org/stable/) machine learning framework to experiment with different machine learning algorithms and different datasets.

Dataset 1 contains images of the 26 uppercase letters [A - Z].
Dataset 2 contains images of 10 Greek letters.
Both datasets are about the classification of black & white images of size 32 × 32 that represent a character. 

Each dataset is in .csv format, where each row is a data instance. Each instance is composed of 1024 binary features followed by its class (the index). 

Each dataset contains 3 splits:
* training: to be used for training your models.
* validation: to be used for validating/experimenting with your models.
* test: to be used to report your final output.

## Task
For each dataset, write the necessary code to:
1. Plot the distribution of the number of the instances in each class.
```
For dataset 1, change select_lang="English" in block #2
Run block #1, #2, #3, #4
```
```
For dataset 2, change select_lang="Greek" in block #2
Run block #1, #2, #3, #4
```

2. Run 6 different ML models:
(a) GNB: a Gaussian Naive Bayes Classifier, with default parameter values.
```
For dataset 1, change select_lang="English" in block #2
Run block #1, #2, #3, #5

It will generate a GNB-DS1.csv file that contains the output classification, a plot confusion matrix, and performance of this dataset such as the precision, recall, and f1-measure for each class, the accuracy, macro-average f1 and weighted-average f1 of the model
```
```
For dataset 2, change select_lang="Greek" in block #2
Run block #1, #2, #3, #5

It will generate a GNB-DS2.csv file that contains the output classification, a plot confusion matrix, and performance of this dataset such as the precision, recall, and f1-measure for each class, the accuracy, macro-average f1 and weighted-average f1 of the model
```

(b) Base-DT: a baseline Decision Tree using entropy as decision criterion and using default values values for the rest of the parameters.
```
For dataset 1, change select_lang="English" in block #2
Run block #1, #2, #3, #6

It will generate a Base-DT-DS1.csv file that contains the output classification, a plot confusion matrix, and performance of this dataset such as the precision, recall, and f1-measure for each class, the accuracy, macro-average f1 and weighted-average f1 of the model
```
```
For dataset 2, change select_lang="Greek" in block #2
Run block #1, #2, #3, #6

It will generate a Base-DT-DS2.csv file that contains the output classification, a plot confusion matrix, and performance of this dataset such as the precision, recall, and f1-measure for each class, the accuracy, macro-average f1 and weighted-average f1 of the model
```

(c) Best-DT: a better performing Decision Tree found by performing grid search to find the best combination of hyper-parameters. For this, you need to experiment with the following parameter values:
* splitting criterion: gini and entropy
* maximum depth of the tree: 10 and no maximum
* minimum number of samples to split an internal node: experiment with values of your choice
* minimum impurity decrease: experiment with values of your choice
* class weight: None and balanced

```
For dataset 1, change select_lang="English" in block #2
Run block #1, #2, #3, #7

It will generate a Best-DT-DS1.csv file that contains the output classification, a plot confusion matrix, and performance of this dataset such as the precision, recall, and f1-measure for each class, the accuracy, macro-average f1 and weighted-average f1 of the model
```
```
For dataset 2, change select_lang="Greek" in block #2
Run block #1, #2, #3, #7

It will generate a Best-DT-DS2.csv file that contains the output classification, a plot confusion matrix, and performance of this dataset such as the precision, recall, and f1-measure for each class, the accuracy, macro-average f1 and weighted-average f1 of the model
```

(d) PER: a Perceptron, with default parameter values.

```
For dataset 1, change select_lang="English" in block #2
Run block #1, #2, #3, #8

It will generate a PER-DS1.csv file that contains the output classification, a plot confusion matrix, and performance of this dataset such as the precision, recall, and f1-measure for each class, the accuracy, macro-average f1 and weighted-average f1 of the model
```
```
For dataset 2, change select_lang="Greek" in block #2
Run block #1, #2, #3, #8

It will generate a PER-DS2.csv file that contains the output classification, a plot confusion matrix, and performance of this dataset such as the precision, recall, and f1-measure for each class, the accuracy, macro-average f1 and weighted-average f1 of the model
```

(e) Base-MLP: a baseline Multi-Layered Perceptron with 1 hidden layer of100 neurons, sigmoid/logistic as activation function, stochastic gradient descent, and default values for the rest of the parameters.

```
For dataset 1, change select_lang="English" in block #2
Run block #1, #2, #3, #9

It will generate a Base-MLP-DS1.csv file that contains the output classification, a plot confusion matrix, and performance of this dataset such as the precision, recall, and f1-measure for each class, the accuracy, macro-average f1 and weighted-average f1 of the model
```
```
For dataset 2, change select_lang="Greek" in block #2
Run block #1, #2, #3, #9

It will generate a Base-MLP-DS2.csv file that contains the output classification, a plot confusion matrix, and performance of this dataset such as the precision, recall, and f1-measure for each class, the accuracy, macro-average f1 and weighted-average f1 of the model
```

(f) Best-MLP: a better performing Multi-Layered Perceptron found by performing grid search to find the best combination of hyper-parameters. For this, you need to experiment with the following parameter values:
* activation function: sigmoid, tanh, relu and identity
* 2 network architectures of your choice: for eg 2 hidden layers with 30+50 nodes, 3 hidden layers with 10+10
* solver: Adam and stochastic gradient descent

```
For dataset 1, change select_lang="English" in block #2
Run block #1, #2, #3, #10

It will generate a Best-MLP-DS1.csv file that contains the output classification, a plot confusion matrix, and performance of this dataset such as the precision, recall, and f1-measure for each class, the accuracy, macro-average f1 and weighted-average f1 of the model
```
```
For dataset 2, change select_lang="Greek" in block #2
Run block #1, #2, #3, #10

It will generate a Best-MLP-DS2.csv file that contains the output classification, a plot confusion matrix, and performance of this dataset such as the precision, recall, and f1-measure for each class, the accuracy, macro-average f1 and weighted-average f1 of the model
```

