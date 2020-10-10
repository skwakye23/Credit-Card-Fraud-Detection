# Credit-Card-Fraud-Detection

Anonymized credit card transactions labeled as fraudulent or genuine

Context

It is important that credit card companies are able to recognize fraudulent credit card transactions so that customers are not charged for items that they did not purchase.
Content

The datasets contains transactions made by credit cards in September 2013 by european cardholders.
This dataset presents transactions that occurred in two days, where we have 492 frauds out of 284,807 transactions. The dataset is highly unbalanced, the positive class (frauds) account for 0.172% of all transactions.

It contains only numerical input variables which are the result of a PCA transformation. Unfortunately, due to confidentiality issues, we cannot provide the original features and more background information about the data. Features V1, V2, … V28 are the principal components obtained with PCA, the only features which have not been transformed with PCA are 'Time' and 'Amount'. Feature 'Time' contains the seconds elapsed between each transaction and the first transaction in the dataset. The feature 'Amount' is the transaction Amount, this feature can be used for example-dependant cost-senstive learning. Feature 'Class' is the response variable and it takes value 1 in case of fraud and 0 otherwise. 


#REQUIRED PACKAGES :

                      pandas==1.0.5
                      
                      numpy==1.18.5
                      
                      matplotlib==3.2.2
                      
                      MYSQL == 8.0
                      
                      Python == 3.72
  
  
 #DATA SOURCE :
 
        https://www.kaggle.com/mlg-ulb/creditcardfraud
        
 
References:

    Good blog article on different methods handling class imbalance: https://www.svds.com/learning-imbalanced-classes/
    A Survey of Predictive Modelling under Imbalanced Distributions: https://arxiv.org/pdf/1505.01658.pdf
    Short blog post about scikit-learn RandomForestClassifier balanced mode:
    https://chrisalbon.com/machine_learning/trees_and_forests/handle_imbalanced_classes_in_random_forests/
    The mechanism of doing the weighted node-split in the tree in scikit learn:
    https://github.com/scikit-learn/scikit-learn/blob/70f170dedf2927c2d805144425522459d92700a7/sklearn/tree/_criterion.pyx#L635
    Paper that introduces "Weighted Random Forests" as a method to deal with class imbalance: 
    https://statistics.berkeley.edu/sites/default/files/tech-reports/666.pdf
    This paper frames the concepts around "cost sensitive learning" , i.e., minizing cost 
    rather than just misclassification loss: https://cling.csd.uwo.ca/papers/cost_sensitive.pdf


