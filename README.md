# Credit_Risk_Analysis

## Overview

The purpose of this project is to train a bunch of machine learning models to try and predict weather or not someone is going to be a high risk or low risk loan canidate.

## Results

Before we can use the model, we must prepare the data since there is a huge discrepency between the number of low risk vs high risk loan applicants. 

The first method used was the naive oversampling algorithm with a logistic regression model. The results are below:

<img width="719" alt="Screen Shot 2022-02-26 at 11 16 42 AM" src="https://user-images.githubusercontent.com/92888170/155856367-a1d5501b-342e-4101-84c2-99e45195f88d.png">

   - The balanced accuarcy score for this model was .6433
   - The precison of this model was 100% for low risk loans and 1% for high risk loans.
   - The recall of this model was 65% for low risk loans and 63% for high risk loans.

The second method used was the SMOTE oversampling algorithm with a logistic regression model. The results are below:

<img width="719" alt="Screen Shot 2022-02-26 at 11 53 05 AM" src="https://user-images.githubusercontent.com/92888170/155857230-fcb6a135-612e-4d4d-8835-a0638a04a702.png">

   - The balanced accuarcy score for this model was .6167
   - The precison of this model was 100% for low risk loans and 1% for high risk loans.
   - The recall of this model was 60% for low risk loans and 65% for high risk loans.

The third method used was the Clustered Centroids undersampling algorithm with a logistic regression model. The results are below:

<img width="719" alt="Screen Shot 2022-02-26 at 12 03 06 PM" src="https://user-images.githubusercontent.com/92888170/155857513-629c421b-4d04-4aaf-b999-7c42f704f9ba.png">

   - The balanced accuarcy score for this model was .5141
   - The precison of this model was 100% for low risk loans and 1% for high risk loans.
   - The recall of this model was 59% for low risk loans and 44% for high risk loans.

The fourth method used was the combined sampling SMOTEENN algorithm with a logistic regression model. The results are below:

<img width="719" alt="Screen Shot 2022-02-26 at 12 08 54 PM" src="https://user-images.githubusercontent.com/92888170/155857651-c567e84d-6252-4610-a318-6b04d6410f61.png">

   - The balanced accuarcy score for this model was .6322
   - The precison of this model was 100% for low risk loans and 1% for high risk loans.
   - The recall of this model was 56% for low risk loans and 70% for high risk loans.


The fifth method used was the Balanced Random Forest Classifier. The results are below:

<img width="719" alt="Screen Shot 2022-02-26 at 12 13 49 PM" src="https://user-images.githubusercontent.com/92888170/155857761-dd56c5f1-1de6-42f3-93c2-1130ec168bb8.png">

   - The balanced accuarcy score for this model was .7410
   - The precison of this model was 100% for low risk loans and 10% for high risk loans.
   - The recall of this model was 98% for low risk loans and 51% for high risk loans.

The sixth and final method used was the Easy Ensemble Classifier. The results are below:

<img width="719" alt="Screen Shot 2022-02-26 at 12 18 24 PM" src="https://user-images.githubusercontent.com/92888170/155857886-af85b229-37f6-434d-9928-306b5a02151c.png">

   - The balanced accuarcy score for this model was .9254
   - The precison of this model was 100% for low risk loans and 7% for high risk loans.
   - The recall of this model was 94% for low risk loans and 91% for high risk loans.

## Summary

In review, I would not consider most of these models useful in predicting credit risk. With that being said, if I had to recommend one I would choose the Easy Ensemlbe Classifer. That model had the highest balanced accuarcy score by far, and its recall was strong for both low and high risk loans. One thing I need to look into, perhaps with all the models, is my possibility for overfitting the models. All of my models have 100% precision with low risk loans so going forward I would need to investigate what is going on.




