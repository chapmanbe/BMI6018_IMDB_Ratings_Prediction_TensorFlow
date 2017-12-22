# BMI6018_IMDB_Ratings_Prediction_TensorFlow

### Predicting movie ratings based on movie metadata obtained from IMDB APIs containing social media attributes and posters information.

### Used Tensor Flow and Neural Network techniques to implement the models.

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

## Libraries required

### Keras
Keras is an open source neural network library written in Python. It is capable of running on top of MXNet, Deeplearning4j, Tensorflow, CNTK or Theano. Designed to enable fast experimentation with deep neural networks, it focuses on being minimal, modular and extensible.

### Scikit-learn
Scikit-learn (formerly scikits.learn) is a free software machine learning library for the Python programming language.

### Numpy
Numpy is the fundamental package for scientific computing with Python. It contains among other things: a powerful N-dimensional array object. sophisticated (broadcasting) functions.

### Pandas
Pandas is a software library written for the Python programming language for data manipulation and analysis. In particular, it offers data structures and operations for manipulating numerical tables and time series.


## Approach

### Data PreProcessing
Replaced missing values in Numeric variables by mean value and character variables by mode value of all records in the column and showed the summary of missing values.

### Data Exploration and Visualization
Exploring and visualizing the relationship of potential predictors with the outcome variable and visualizing multi-collinearity between different variables and selecting relevant predictors.

### Model Development and Evaluation 
Created a base model with one hidden layer, a larger model with more hidden layers having less number of nodes, and a wider model with less hidden layers having more number of nodes.



## Conclusion
1. The model having more number of hidden layers is performing better than the model having more number of neurons. 
2. Director facebook likes and actors facebook likes matter. There is not much gain from adding the categorical and 
the keywords variables.
3. I have removed the correlated variables as I wanted to reduce the number of variables for the fitting to happen 
in a reasonable amount of time

## Future Improvement
1. We happened to run my models a few times (without poster information, with plot_keywords, and without directors) but still 
unable to minimize the error, I believe it might be possible with some external data.
2. Should work more on data preprocessing, feature engineering and adding hyperparameter values.
3. Should research more about tensor flow and explore neural network techniques.
