# Automatic-Ticket-Classification-NLP

## Introduction

In this case study, we have created models that can automatically classify customer complaints based on the products and services that the ticket mentions.

## Understanding Problem Statement

For a financial company, customer complaints carry a lot of importance, as they are often an indicator of the shortcomings in their products and services. If these complaints are resolved efficiently in time, they can bring down customer dissatisfaction to a minimum and retain them with stronger loyalty. This also gives them an idea of how to continuously improve their services to attract more customers.

These customer complaints are unstructured text data; so, traditionally, companies need to allocate the task of evaluating and assigning each ticket to the relevant department to multiple support employees. This becomes tedious as the company grows and has a large customer base.

In this case study, you will be working as an NLP engineer for a financial company that wants to automate its customer support tickets system. As a financial company, the firm has many products and services such as credit cards, banking and mortgages/loans.

## Business Goal

We need to build a model that is able to classify customer complaints based on the products/services. By doing so,  can segregate these tickets into their relevant categories and, therefore, help in the quick resolution of the issue.

 will be doing topic modelling on the .json data provided by the company. Since this data is not labelled, we need to apply NMF to analyse patterns and classify tickets into the following five clusters based on their products/services:

Credit card / Prepaid card

Bank account services

Theft/Dispute reporting

Mortgages/loans

Others 

With the help of topic modelling, you will be able to map each ticket onto its respective department/category. You can then use this data to train any supervised model such as logistic regression, decision tree or random forest. Using this trained model, you can classify any new customer complaint support ticket into its relevant department.



Business Objectives

Importing all the Libraries

## Data Loading

The data is in JSON format and we need to convert it to a dataframe.

## Data preparation

Data cleaning operations like filtering text, removing missing values & renaming column headers.

## Text Preprocessing

### Prepare the text for topic modeling

Once you have removed all the blank complaints, you need to:

Make the text lowercase
Remove text in square brackets
Remove punctuation
Remove words containing numbers
Once you have done these cleaning operations you need to perform the following:

## Lemmatize the texts

## Use POS tags to get relevant words from the texts.

Data Cleaning and Manipulation

Data Lemmatizer

## Data POS Tag Extraction

## Exploratory data analysis {EDA}

### Exploratory data analysis to get familiar with the data.¶

WE Write the code in this task to perform the following:

Visualise the data according to the 'Complaint' character length
Using a word cloud find the top 40 words by frequency among all the articles after processing the text
Find the top unigrams,bigrams and trigrams by frequency among all the complaints after processing the text. ‘

Finding the Top Unigrams,Bigrams and Trigrams

## Feature Extraction

Convert the raw texts to a matrix of TF-IDF features¶

**max_df** is used for removing terms that appear too frequently, also known as "corpus-specific stop words" max_df = 0.95 means "ignore terms that appear in more than 95% of the complaints"

**min_df** is used for removing terms that appear too infrequently min_df = 2 means "ignore terms that appear in less than 2 complaints"

## Topic Modelling

Topic Modelling using NMF

##** Non-Negative Matrix Factorization (NMF) It is an unsupervised technique so there are no labeling of topics that the model will be trained on. The way it works is that, NMF decomposes (or factorizes) high-dimensional vectors into a lower-dimensional representation. These lower-dimensional vectors are non-negative which also means their coefficients are non-negative.
**
In this task we are performing the following:

Find the best number of clusters

Apply the best number to create word clusters

Inspect & validate the correction of each cluster wrt the complaints

Correct the labels if needed

Map the clusters to topics/cluster names

Finding the best number of clusters

Applying the best number to create word clusters

Inspecting & validate the correction of each cluster wrt the complaints

Correcting the labels if needed

Map the clusters to topics/cluster names

## Model training and evaluation

### Model building using supervised learning, Model training & evaluation¶

Supervised model to predict any new complaints to the relevant Topics.

We now build the model to create the topics for each complaints.Now in the below section you will use them to classify any new complaints.

Since you will be using supervised learning technique we have to convert the topic names to numbers(numpy arrays only understand numbers)

## Preprocessing for model

Reverse topic names mapping for supervised learning

X - Y split

Train Test Split

Logistic regression, Decision Tree & Random Forest

Custom Classification Report

Stratified KFold Cross Validation

Custom Grid Search Cross Validation

Multinomial Naive Bayes Classification

Logistic Regression Classification

Decision Tree Classification

Random Forest Classification

Hyper parameter tuning with GridSearchCV

Multinomial Naive Bayes with GridSearchCV

Logistic Regression with GridSearchCV

Decision Tree Classification with GridSearchCV

Random Forest Classifier with GridSearchCV

## Model inference

## Conclusion 
