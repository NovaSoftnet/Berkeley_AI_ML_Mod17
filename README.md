# Project Documentation

## Introduction

This is a Practical Application Assignment for the Professional Certification in Machine Learning and Artificial Intelligence program at UC Berkeley Executive Education

A dataset from [UCI Irvine Machine Learning repository](https://archive.ics.uci.edu/ml/datasets/bank+marketing) was used. The data is from a Portuguese banking institution and is a collection of the results of multiple marketing campaigns

----

## Business Objective


**Apply the CRISP-DM methodology to compare the performance of several classifiers (k-nearest neighbors, logistic regression, decision trees, and support vector machines) in order to identify the best Machine Learning Classification model that can be used to determine the factors that drive the success of tele-marketing campaigns for a Banking Institution**

The evaluation of the best model will be based on the data available from the Bank's previous marketing campaigns, which include personal customer data and some parameters about the product offered to that customer, being the target variable the acceptance or rejection of the product offered.

----

## Procedure

Following the CRISP-DM methodology:

1. Business Understanding

* The Telemarketing is key for the Bank go to market strategy, its impact on reaching new customers is highly relevant to achieve their revenue goals.

2. Data Understanding

* **Exploratory Data Analysis** was performed on all features (independent variables) in the dataset
* Identified categorical and numerical features
* Features were analyzed to find  necessary vs irrelevant for the business goal
* A subset of features was selected for use in modeling
 
3. Data Preparation

* Dropped irrelevant features
* Converted and aggregated values for several features
* Filled in missing data
* Transformed categorical features accordingly using OneHotEncoding
* Training and Testing datasets were created using **stratification** given the unbalanced classes for the target variable

4. Modeling

* Established **baseline** performance
* Compared **accuracy**  for the following Classification models with default configuration:


  * Logistic Regression
  * K Nearest Neighbors
  * Decision Tree
  * Support Vector Machine


* Evaluated the initial results and executed  a second round to improve each model´s performance
* Performed Grid Search for multiple hyper-parameters for each model tuning using **f1 scoring** 

5. Evaluation

* Model performance was evaluated and compared between models using multiple metrics:

  * **F1 score**
  * **Accuracy**
  * **Precision**
  * **Recall**
  * **ROC AUC**

* Classified the corresponding metrics  to identify best performing model with optimal hyper-parameters
* Reviewed findings and elaborated final recommendations

6. Deployment

* Delivered our conclusions reached from the evaluation process
   * Provided recommendations base on the results and required resources to deploy our recommended model

----

## Conclusions


---

* Based on these results, and the different metrics used to score the models  to classify the tele-marketing data, the recommendation is to use **K Nearest Neighbors**


* The second-best option would be to use a **Decision Tree** model


* These models deliver an acceptable balance between performance scoring, easy to tune hyper-parameters, and acceptable fitting times


---

----

## Recommendations


---

* Given the challenges with the received unbalanced data set, the main recommendation is to further improve the data engineering process and apply more elaborate techniques like Synthetic Minority Oversampling Technique,(SMOTE) to reduce that condition

* Use more elaborated  tunning  on the engineered data and assess any improvement in performance. 


----
