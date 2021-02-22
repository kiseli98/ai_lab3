# AI Lab3 - Machine Learning (Linear Regression)
This porject contains implementation of laboratory work for Artificial Intelligence course (UTM 2021).

 
The task was to take a raw dataset containing info regarding different residential complexes and to create a model that would
perform linear regression on the available data. As a result, the model should be able to predict
the medianCompexValue of an apartment complex, given a set of it’s characteristics. 

*Note: The lab was implemented and tested in Google Colab Notebooks*

# Approach

Given the initial set of data it was decided to perform several operations on it. Firstly, all extra columns that didn't really affect the median complex were removed. Then data normalization was applied.

During this lab 3 different apporximation models were considered:
1. Linear Regression using *keras.Sequential*  model. It performs data normalization and then applies linear transformation $(y=mx+b)$ to produce 1 output using *layers.Dense*
2. Linear Regression using Deep Neural Networks. Implementation is similar to the previous model with except the model is expanded to include some "hidden" non-linear layers. The name "hidden" here just means not directly connected to the inputs or outputs. This model contain a few more layers than the linear model:
* The normalization layer
* Two hidden, nonlinear, *Dense* layers using the *relu* nonlinearity.
* A linear single-output layer.
3. Linear Regression model using scikit learn


## Running the code

Simply import *lab3.ipynb* in Jupiter Notebook or in Google Colab Notebooks and perform all inputs one by one.

Otherwise, the code can be run in python or conda shell:
```bash
   python lab3.py
  ```

