# Film Review Sentiment Analysis

## Project Description

Film Junky Union, a cutting-edge community for classic movie enthusiasts, is developing a system to filter and categorize movie reviews. Your objective is to train a model to automatically detect negative reviews. To achieve this, you will use a labeled IMDB movie review dataset to build a model that classifies reviews as positive and negative. It should achieve an F1 score of at least 0.85.

## Project Instructions

1.  Load the data.
2.  Preprocess the data, if necessary.
3.  Perform exploratory data analysis and draw your conclusion about class imbalance.
4.  Perform data preprocessing for modeling.
5.  Train at least three different models on the training dataset.
6.  Test the models on the test dataset.
7.  Write some reviews and classify them with all the models.
8.  Find the differences between the test results of the models in the previous two points. Try to explain them.
9.  Show your findings.

## Data Description

The data is stored in the file `imdb_reviews.tsv`. 

The data was provided by Andrew L. Maas, Raymond E. Daly, Peter T. Pham, Dan Huang, Andrew Y. Ng, and Christopher Potts. (2011). Learning Word Vectors for Sentiment Analysis. The 49th Annual Meeting of the Association for Computational Linguistics (ACL 2011).

Here are the selected fields described:

* `review`: the text of the review
* `pos`: the target, '0' for negative and '1' for positive
* `ds_part`: 'train'/'test' for the train/test part of the dataset, respectively
