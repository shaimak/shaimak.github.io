---
title: "ML Research Intern"
description: "Indian Institute of Management, Ahmedabad (IIM Ahmedabad), India"
dateString: May 2013 - Jun 2013
draft: false
tags: ["Sentiment Analysis", "ML"]
showToc: false
weight: 5

--- 
> [Project Report](https://drive.google.com/file/d/1OP2KtqALSJ68EF_p_jUu3sEgai6Qz-5P/view)

**Guide:** **Prof. S. Krishnamoorthy** (Professor, Dept. of Information Systems, IIM Ahmedabad)

### Title: Classification of Customer Product Reviews Using Sentiment Analysis

- Achieved 90.8% accuracy (compared to 79.5%) in sentiment analysis of book reviews using Python-based machine learning (ML) models and natural language processing (NLP) techniques


### Description

We consider the problem of finding out the best techniques in classifying documents not by topic, but by overall sentiment, e.g., determining whether a review is positive or negative. Using novel reviews as data, we try to find out the combination of feature extraction, feature selection and machine learning methods which results in maximum accuracy. We also look at some new weighing schemes which we later find out, are more accurate than our traditional schemes. We conclude by suggesting the combination of tools which is likely responsible for optimum accuracy considering sentiment classification only.

### Process
We started by off by comparing reviews to determine their overall sentiment in order to effectively classify them. As per the tests we’ve performed, TF-idf feature extraction methods are performing significantly better than the traditional N-gram feature extraction methods (90.8% as compared to 79.5%). When it comes to feature selection algorithms, we can also state that they are beneficial only for traditional feature selection algorithms and not for tf-idf. Logistic Regression proved to have the highest accuracy in prediction for both kinds of feature extraction models. Thus, with okapi (bm25) tf weighing with smoothed idf as feature extraction, and with logistic regression as prediction, we can expect very high accuracies.

Limitations: We’ve come up with a fairly reasonable method which does have a very good accuracy but we are still open to more explorations. These mainly correspond to changing the
parameters and observing the effect of them on our primary results. Starting with the traditional methods where feature selection was a boon, two things could have been altered to probably get better accuracy. These being the ‘n-gram’ (which is unigram in our experiments), and the count of features we select from feature selection algorithms. 

The former may have better results considering the bi-grams like ‘not pleasing’, ‘not bad’
as compared to unigram based evaluation. The later may not be of any importance since feature
selection didn’t have any benefits in case of tf-idf weighing schemes. However, reducing around
20,000 features to 500 would definitely reduce the accuracy by quite some bit. Hence is still worth
the effort.
