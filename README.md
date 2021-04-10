# Multiclass Text Classification - News Dataset

## Summary

Text classification is a supervised learning technique so we’ll need some labeled data to train our model. I’ll be using this public news classification dataset. It’s a manually labeled dataset of news articles which fit into one of 4 classes: Business, SciTech, Sports or World.

In this notebook, I have used multiple techniques to compare the classification accuracy on the news dataset.

## Data

The dataset json file I found from some site which I haven't noted, hence the same I have kept it in git repo.

## Pre-requisites

The project was developed using python 3.8.3 with the following packages.
- pandas
- numpy
- json
- sklearn
- nltk
- re
- bs4
- gensim
- matplotlib
- seaborn

Installation with pip:

```bash
pip install -r requirements.txt
```

## Files
Notebooks : 
- notebook/MultiClass_Text_Classification_using TFIDF_TruncatedSVD.ipynb : Jupyter Notebook with all the workings including basic pre-processing techniques and using Lemmatizing with explicitly passing POS taggers, used TFIDF to create features and used Truncated SVD to reduce dimensions.
Tried several classification models and found Logistic Regression and XGBoost working best. However the model performance is lower than the one trained using Glove,

- notebook/MultiClass_Text_Classification_using_custom_trained_wordembedding.ipynb : Jupyter Notebook with all the workings including basic pre-processing techniques and using Lemmatizing with explicitly passing POS taggers, trained word vectors using the available data and then using the same to create features.
Tried several classification models and found XGBoost and Logistic Regression working best.
The model performance is lower than the one trained using Glove.

- notebook/MultiClass_Text_Classification_using Word Embeddings_Glove.ipynb : Jupyter Notebook with all the workings including basic pre-processing techniques and using Lemmatizing with explicitly passing POS taggers, used Glove vectors of 300 dimension to create features.
Tried several classification models and found Logistic Regression and XGBoost working best.
The model performance of these one is better than the above two.


- requirements.txt : pre-requiste libraries for the project
- data/ : source data in JSON format.

