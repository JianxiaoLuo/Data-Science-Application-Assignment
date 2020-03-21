# Data-Science-Application-Assignment
It is the assignments of my course Data Science Application.

# Assignment1 Text Classification

## Overview
The goal of our program is to classify the word from seven different authors after training. Our code contains two main parts. First, we select validate books, do several steps of data preparing and preprocessing to get it ready for our models. The second part is to do transform, training and testing.

## Environment
Python version: 3.X

Develop platform: Google Colab


## Prerequisite
The libraries we used include: nltk, sklearn, numpy, matplotlib.pyplot, pandas, spacy, seaborn.

If you use Colab to run the code, it is not necessary for you to install the external libraries yourself.

## How to run
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

