# Generating-target-for-binary-classification
Explain right way of generating the y value for binary classification model.

During my academic project,<br>
I thought there is something wrong in dataset.<br>
I needed to test my logistic regression model whether it works well or not.<br>

For testing my model, I generated x and y data in a wrong way.<br>
I simulated y if p >= 0.5<br>
It makes model with good accuracy, but it can't have good intercept and coefficient prediction.<br>

On the other hand, with the right way of generating y,<br>
accuracy is relatively low but intercept and coefficient prediction is much better.

### Two ways of Generating y
#### 1. Wrong way
Put 1 when p >= 0.5, or put 0
This is same way as predicting y in logistic regression

#### 2. Right way
Generate uniformly distributed random number 'r',
and Put 1 when r <= p, or put 0

Please look at the Jupyter notebook for more detail. Click <a href='https://github.com/texasroh/Generating-target-for-binary-classification/blob/master/create%20simulation%20data%20for%20binary%20classification.ipynb'>here</a>

