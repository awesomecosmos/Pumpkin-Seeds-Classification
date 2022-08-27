# Pumpkin Seeds Classification

## Project Synopsis

In this research project, I perform an extensive algorithm and dataset split analysis in order to determine the best possible combination of algorithm(s) and dataset split which yields the most accurate classification results. For this purpose, a dataset containing morphological measurements of Turkish pumpkin seeds is used, along with 10 algorithms, and 4 dataset splits. Detailed analysis is performed and described in this research, and concluded with the best inferred algorithm and dataset split combination.

The dataset used in this research is the ‘Pumpkin Seeds’ dataset, available from [Kaggle](https://www.kaggle.com/datasets/muratkokludataset/pumpkin-seeds-dataset). This dataset is from a 2021 study on two species of pumpkin seeds, and their morphological features. The dataset comprises of 2500 records of the morphological features of both types of pumpkin seeds (cercevelik, urgup sivirsi). The values of the morphology of the seeds were obtained using 2-dimensional image processing techniques in [Koklu et al., 2021](https://link.springer.com/article/10.1007/s10722-021-01226-0).

<img src="datafiles/pumpkin_seeds.jpg" width="272" height="432">

## Classification

The classification of pumpkin seeds is performed using [WEKA software](https://www.cs.waikato.ac.nz/ml/index.html), which is a graphical software used for performing classifications. The results obtained from the classification schemes were manually inputted into a CSV. We will read the CSV of obtained results in the next section.

The aim of this research is to compare different classification algorithms and their efficiency in predicting the class of pumpkin seed in the following dataset scenarios:
- data split into training/testing split of 60%/40%.
- data split into training/testing split of 80%/20%.
- data split according to 5-fold cross validation.
- data split according to 10-fold cross validation.

The following data mining techniques were used to evaluate the performance of the algorithms on the aforementioned data train/test splits:
- Decision Stump: algorithm returning a single-level decision tree to make a prediction based on the value of a single attribute.
- Decision Table: algorithm returning set of rules to classify the class attribute.
- IBk (k-NN): algorithm for k-nearest neighbors classification scheme. 
- OneR: algorithm returning a single-level decision tree to make a prediction based on the value of a single attribute.
- C4.5 (J48) pruned: algorithm returning a pruned decision tree for classifying the attributes.
- C4.5 (J48) unpruned: algorithm returning an unpruned decision tree for classifying the attributes.
- Logistic Regression: linear regression algorithm to classify instances according to regressions for each class.
- k-Star: algorithm for instance-based classification using a distance function, e.g Euclidean distance function.
- Naive Bayes: algorithm based on Bayes' rule, assuming independent probabilities of attributes. 
- SMO: algorithm using a support vector classifier to train the attributes.
