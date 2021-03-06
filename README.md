# MLCodeLab

Welcome to MLCodeLab! Today we'll be building a sentiment analysis classifier for twitter. Our task is determining if a tweet is positive or negative.

So given a tweet like `This weather is awful #boston `, we want to build a classifier to correctly classify this tweet as negative.

In this lab we cover:

- Building a classifier end to end (from raw text to features to results!)
- Analysis and feature engineering
- Experimenting with different classifiers

In the talk, I'll walk through some sample code, but working through implementing the code yourself is heavily encouraged! It's not very tricky but generating the code yourself will solidify the knowledge. Let's get started!

# 1: Building it End to End  
In this section, we'll be building feature extraction, mapping tweets to a discrete sized array (a bag of words model), training a Perceptron and evaluating our results. The relevant python file is listed bellow.

- [model.py](model.py)


# 2: Analysis and Feature Engineering
In this section, we'll look tune our model to optimize it's performance. We'll play with the number of training iterations, vocabulary size, the use of stop words and ngram representations. 

- [featureEngineering.py](featureEngineering.py)


# 3: Exploring more classifiers
Scikit-learn makes it really easy to experiment with different types of classifiers. In this section, we'll show how we can switch from the previous implemention of *model.py* with Perceptron to a Passive Agressive Classifier, or an SVM. The relevant python file is called:

- [allModels.py](allModels.py)

# Additional information:
One thing we didn't walkthrough is how we build the *.p* files. For completeness, I've included the code for that [here](data/buildDataSet.py).

### Sources
This twitter dataset for this code lab comes from [here](http://thinknook.com/twitter-sentiment-analysis-training-corpus-dataset-2012-09-22/)

The full dataset with 1.5 million tweets can be downloaded [here](http://thinknook.com/wp-content/uploads/2012/09/Sentiment-Analysis-Dataset.zip)

More information about scikit-learn can be found at their [website](http://scikit-learn.org/)
