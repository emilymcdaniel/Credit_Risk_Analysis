# Credit Risk Analysis
Evaluating models for loan predication risk analysis 
------

# Overview 
This evaluation demonstrates the value of various computational models when a multitude of factors affect one desicion. Imagine there are 85 factors to weigh - it is difficult to demonstrate on a bar chart or through an algebraic equation - so they are run through an algorithm. When one factor only allows a yes/no response, and the next could be any numeric value, how can we balanace each data class? Not all models are built equal and some give less meaningful results than others, depending on the data.

Here, we look at credit risk data, [here](https://github.com/emilymcdaniel/Credit_Risk_Analysis/blob/main/LoanStats_2019Q1.zip), to determine whether an individual is deemed "high risk" or "low risk".

-----

# Results: 
Each decision model weighs data differently. Let's look at the balanced accuracy scores (macro-average of recall scores), precision (frequency a model's positive result is is correct), and recall(frequency a model's prediction gives the correct result) differences within each model:

## Model 1: RandomOverSampler 
RandomOverSampler randomly duplicates examples from the minority class and adds them to the training dataset. 
- Balanced accuracy score:
- Precision:
- Recall:
## Model 2: SMOTE (oversampling)
The SMOTE algorithm created synthetic data based on the existing minority class and adds them to the training dataset. NOTE: SMOTE will not promote outliers.
- Balanced accuracy score:
- Precision:
- Recall:
## Model 3: ClusterCentroids (undersampling)
Undersampling decreases the proportion of your majority class until the number is similar to the minority class. The ClusterCentroids method reduces the majority class data that is furthest from its average.
- Balanced accuracy score:
- Precision:
- Recall:
## Model 4: SMOTEENN (a combinatorial approach of over- and undersampling)
SMOTEENN combines SMOTE and ClusterCentroids to balance data classes.
- Balanced accuracy score:
- Precision:
- Recall:
## Model 5: BalancedRandomForestClassifier 
This algorithm randomly selects subsets of features used in each data sample, and ranks the relationship of each factor on the question. NOTE: It is not suited for classification problems with a skewed class distribution.
- Balanced accuracy score:
- Precision:
- Recall:
## Model 6: EasyEnsembleClassifier 
The EasyEnsembleClassifier allows each factor to help refine how the next is interpreted on the question.
- Balanced accuracy score:
- Precision:
- Recall:

-----

# Summary: 
Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. 

## Model Recommendation
If you do not recommend any of the models, justify your reasoning.



Links to images are working, and code is formatted and displayed correctly (2 pt).
