# Natural Language Processing - IMBd Reviews classification.

This is a project about natural language processing for classify reviews.
I created a supervised learning model that categorize reviews into positive or negative.

## Dataset

The dataset is a list of 50.000 IMbd reviews from https://www.kaggle.com/lakshmi25npathi/imdb-dataset-of-50k-movie-reviews.

Each review is classified by positive or negative. There are 25.000 positives and 25.000 negatives.
I divide the dataset into a training and test sets, using the training set for training the model and the test set for evaluate how good it does.

## Cleaning

In first place we remove all puntuaction and we made the lemmatization of the text.

<img src="images/2.jpg">

## Processing

The second part is processing the texts. We tokenize each word and encode them with a unique number.

<img src="images/1.png">

## Model

The model is a TextCNN with three convolutional layers in parallel, applying a maxpooling for each one, concatenating them and the last sigmoid layer.

<img src="images/3.png">


