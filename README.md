
# Charity Funding Predictor Using Neural Networks

This research aims to develop a binary classifier that can predict whether or not applicants will be successful if they are sponsored by Alphabet Soup.
To achieve success, increasingly complex methodologies were applied to model patterns in the quest for greater performance and a business case.
However, the realism afforded by these models comes at the expense of increased computing complexity.
This work report looks at how neural networks can be used to help design the organization's future. 

# Problem Statement
From Alphabet Soup’s business team, you have received a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. Within this dataset are a number of columns that capture metadata about each organization, such as the following:

* **EIN** and **NAME**—Identification columns
* **APPLICATION_TYPE**—Alphabet Soup application type
* **AFFILIATION**—Affiliated sector of industry
* **CLASSIFICATION**—Government organization classification
* **USE_CASE**—Use case for funding
* **ORGANIZATION**—Organization type
* **STATUS**—Active status
* **INCOME_AMT**—Income classification
* **SPECIAL_CONSIDERATIONS**—Special consideration for application
* **ASK_AMT**—Funding amount requested
* **IS_SUCCESSFUL**—Was the money used effectively


## Tech Stack
Libraries:
•	Pandas to read and create data frames
•	Seaborn for visualization
•	Sklearn for training and testing and standardizing data
•	Tensor flow for machine learning
•	Keras tuner for hyper parameter optimization
•	Keras layer dense to create sequential model


## Optimizations

Model 1:
Assumptions
1.  Reduce unique categories of Application type to 10 by creating a bin
2.	Reduce categories column to less than 800

Model 2:
Assumptions
1.	Reduce unique categories on Application type further to those less than 5 by creating a bin
2.	Slash classification to less than 1800
3.	Filter names with income amount greater than or equal to 10000.

Model 3:
Assumption
Leave all features and categories as describe in dataset.

Model 4:
Similar to model 1 except increase the number of neurons and reduce epochs


## Lessons Learned

Recommendation:
Since by design the ReLU activation function is unbounded in the positive domain. A further reading indicates that some form of weight regularization will help prevent potential numerical problems which will intern promote additional sparsity. Also, since the features in this project work are quite complex and not very much related the sigmoid function even though produced an accuracy of 73.2% it cannot learn complex mapping hence its deficiency for this model. The use of Convolutional Neural Networks (CNN) might be appropriate.


## Authors

- [@maxwellansah](https://github.com/maximum-boop/Charity-Funding-Predictor)


## Acknowledgements

 - [Awesome Readme Templates](https://awesomeopensource.com/project/elangosundar/awesome-README-templates)
 
- Google Colab
