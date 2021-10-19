# Hate and Offensive Tweets Identification

## Aim

The aim of this project is to create a model that identifies hate and offensive tweets and also classifies those hate/offensive tweets according to the kind of content they contain.
The dataset used is the HASOC 2019 English dataset.

## Abstract

Toxic online content has become a major issue in today’s world due to an exponential increase in the use of the internet by people of different cultures and educational backgrounds. Differentiating hate speech and offensive language is a key challenge in the automatic detection of toxic text content.

## Overview

In this report, we propose an approach to automatically classify tweets on Twitter by performing three tasks.

**task_1:**
> Classiﬁcation of Hate Speech (HOF) and non-hate/offensive content.

**task_2:**
> If the post is HOF, task_2 is used to classify it as either hate speech (HATE), offensive content (OFFN) or profanity (PRFN).

**task_3:**
> It decides the target of the post, i.e., targeted insult (TIN) or untargeted (UNT).

---

## Summary

Our project analyzed a dataset Hate Speech and Offensive Content Identification in Indo-European Languages from a TSV file containing ```5852``` tweets.

---

## Preprocessing

### Data Preprocessing

1. **Removing insignificant columns**: During many instances, some columns were not relevant to the analysis. When building a machine learning models, columns are removed if they are redundant or don’t help the model.

2. **Handling Null Values**: In any real-world dataset, there are always few null values. It doesn’t really matter whether it is a regression, classification or any other kind of problem, no model can handle these NULL or NaN values on its own so we need to intervene.

### Cleaning Tweets

Languages we speak and write are made up of several words often derived from one another and can contain words which don’t add meaning or context. In order to clean the data, we implemented 4 approaches.

1. **Special characters removal**: We next removed special characters and numbers. Numbers rarely contain useful meaning. Special characters can bloat our term-frequency matrix.

2. **Converting all letters to lower case**

3. **Stop words removal:** Stop words are usually articles or prepositions which do not help us to find the context or the true meaning of a sentence. These are words that can be removed without any negative consequences to the final model that you are training. Commonly used in English language include “is”,” and”,” are” etc.

4. **Lemmatization:** Lemmatization is the process of grouping together the different inflected forms of a word so they can be analyzed as a single item. Lemmatization is similar to stemming but it brings context to the words. So, it links words with similar meaning to one word. For example, runs, running, ran are all forms of the word run, therefore run is the lemma of all these words.

---

## Exploratory Data Analysis

EDA is primarily used to see what data can reveal beyond the formal modeling or hypothesis testing task and provides a provides a better understanding of data set variables and the relationships between them. It can also help determine if the statistical techniques you are considering for data analysis are appropriate.

The main purpose of EDA is to help look at data before making any assumptions. It can help identify obvious errors, as well as better understand patterns within the data, detect outliers or anomalous events, find interesting relations among the variables.

---