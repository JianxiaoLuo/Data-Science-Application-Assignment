# Data-Science-Application-Assignment
## Introduction
It is assignments and project of my course GNG5126 Data Science Application.

The first assignment is about classification, we mainly use NLTK and sklearn libraries. 

The second assignment is about clustering. 

You can see the assignment requirements in PDFs.

## Assignment1 Text Classification

### Overview
The goal of our program is to classify the word from seven different authors after training. Our code contains two main parts. First, we select validate books, do several steps of data preparing and preprocessing to get it ready for our models. The second part is to do transform, training and testing.

### Environment
Python version: 3.X

Develop platform: Google Colab


### Prerequisite
The libraries we used include: nltk, sklearn, numpy, matplotlib.pyplot, pandas, spacy, seaborn.

If you use Colab to run the code, it is not necessary for you to install the external libraries yourself.

### How to run
Our code [GNG Data Science assignment1.ipynb](https://colab.research.google.com/drive/1Bum4VCEGecAxzIqrzdz99ze-OZovQbJf#scrollTo=qjM-R-vAPUpP&uniqifier=6) was developed on Google Colab, so it is easy to open it through Colab and run the code cell sequently.


You can also open and run the code through jupyter notebook or jupyterLab.


In the function ` main() `, there are several key execute parameters you can modify:
``` Python
    ########### EXECUTE ################
    train_list = ['svm']
    n = nlp_1(documents, shuffle=1)
    n.transform(type='2-gram', tf_idf=False)
```
In the `train_list`, you can add the one or more algorithms you want to play with. The parameters are `'decision tree'`, `'svm'`, `'linear regression'`, `'mlp'`, `'gaussian naive bayes'` and `'knn'`. Decision tree is the defalt algorithm.

In the parameters of `n.transform(type=  , tf_idf=  )`, you can define the type of transform. The parameters of `type` are `'bow'`, `'3-gram'` and `'2-gram'`. The parameter of `'tf_idf` is boolean(True or False), which define whether it will do tf-idf or not. BOW and tf-idf False is the defalt parameter.


## Assignment2 Text Clustering

### Overview
The program is to do the Doc2Vec transformation and clustering. It contains seven functions.

`def preprocess()`-- It does the preprocessing and returns a dictionary of documents and labels.
`def doc2vec(docs, model=1)`-- It is the function to do Doc2Vec transformation, the argument docs are the list of documents and the model argument is to see if we train a model or load a pre-trained model.
`def kmeans(infered_vectors_list)`, `def em(infered_vectors_list)` and `def agg(infered_vectors_list)` are the functions to do clustering algorithms. The input of them is the transformed vector of documents.
`def kappa(pred_label_kmeans, pred_label_em, pred_label_agg, true_labels)` and `def silhouette(infered_vectors_list, pred_label_kmeans, pred_label_em, pred_label_agg)` are to do the Kappa score and Silhouette score evaluation.
The last code cell is the main part of the program. It calls those functions and does visualization. 
 
### How to run
It is the environment on Colab, so you just need to run the code cells in sequence. After you run the last code cell, you will see the result. Named as ‘Part C’.’


