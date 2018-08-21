# Automatic Fact-Checking

## Plan

* Introduction
* Data
* Scripts

## Introduction

This work was done during my master thesis at the LIRMM institute in Montpellier. The thematic was Automatic Fact-Checking.
This repo contain links to data and scripts.

## Data

The archives are too heavy for a github repository, here are the google drive links :
* data.tar : https://drive.google.com/open?id=1OCUd2eFlqfaQx7FFgDkIGteHw2K4q4Yl
* ressources.tar : https://drive.google.com/open?id=14j0D5oI6mlq-MWGZSmpEwCv3FLSQRdWg

## Scripts

Here is a brief description of the scripts :
* 00_snippet_cleansing : we explore 
claims and snippets and apply some cleasning
steps
* 01_relevance_discovery_benchmark_building : we build
groundtruth data for our relevance discovery step
* 02_bow_snippets : we apply preprocessing steps on
snippets and claims, also we build lexicons
* 03_topics_models_building : we build tfidf and 
topic models on snippets and claims for each
lexicon
* 04_similarity_measures_computing : for each
model, we build representation of our snippets
and claims from our groundtruth data for relevance
discovery and we compute similarity measures
between these representations
* 05_relevance_discovery_evaluation : we use 
original metrics on the similarity mesures
to evaluate performances of the associated
models and choose the best one for relevance
discovery
* 06_filter_relevant_results : we apply the chosen
model for relevance discovery and similarity measure
between claim and snippets on the whole data set
to filter out irrelevant snippets
* 07_build_dataset : after fetching web documents
associated to relevant snippets, we process web documents
to build a data set
* 08_cleansing_documents : we explore 
claims and documents and apply some cleansing steps
* 09_bow_documents : we apply preprocessing steps
on claims and documents, also we build lexicons
* 10_topic_modeling : we build tfidf and
topic models on claims and documents for each
lexicon
* 11_features : we apply models on claims and documents
to build feature representations of claims and documents
* 12_evaluation : we train and test machine learning models
on features to figure out which feature representation
best suits machine learning models to check the veracity of
claims

For more information, look at presentation.pdf, memoir.pdf, 
comments in the scripts or contact me at :
j.bressand.34@gmail.com
