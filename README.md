

# Charity Funding Predictor Using Neural Networks

- This research aims to develop a binary classifier that can predict whether or not applicants will be successful if they are sponsored by Alphabet Soup.
- To achieve success, increasingly complex methodologies were applied to model patterns in the quest for greater performance and a business case.
- However, the realism afforded by these models comes at the expense of increased computing complexity.
- This work report looks at how neural networks can be used to help design the organization's future. 


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
  - unique categories of Application type to 10 by creating a bin
  - Reduce categories column to less than 800

Model 2:
Assumptions
  -	Reduce unique categories on Application type further to those less than 5 by creating a bin
  - Slash classification to less than 1800
  - Filter names with income amount greater than or equal to 10000.

Model 3:
Assumption
  - Leave all features and categories as describe in dataset.

Model 4:
  - Similar to model 1 except increase the number of neurons and reduce epochs


## Lessons Learned

- Since by design the ReLU activation function is unbounded in the positive domain. A further reading indicates that some form of weight regularization will help prevent potential numerical problems which will intern promote additional sparsity. Also, since the features in this project work are quite complex and not very much related the sigmoid function even though produced an accuracy of 73.2% it cannot learn complex mapping hence its deficiency for this model. The use of Convolutional Neural Networks (CNN) might be appropriate.


## Authors

- [@maxwellansah](https://github.com/maximum-boop/Charity-Funding-Predictor)


## Acknowledgements

 - [Awesome Readme Templates](https://awesomeopensource.com/project/elangosundar/awesome-README-templates)
 
- Google Colab
