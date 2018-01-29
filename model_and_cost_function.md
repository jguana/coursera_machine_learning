# Linear Regression with One Variable

# Training Set
The training set gets fed through the Learning Algorithm.

x -> hypothesis -> estimated price

How do we represent h?

#Model Representation
$x^{(i)}$ Input variables. Living area.

$y^{(i)}$ Output/target variables. Price.

$(x^{(i)},y^{(i)})$ Training example. Dataset.

$(x^{(i)},y^{(i)});i=,...,m$ Training set.

The superscript is simply an index of the training set, not to be confused with exponentiation.

$X$ Input values

$Y$ Output values

In this example $X = Y = R$

Our goal is to develop a function h(x) as a good predictor for the corresponding values of y. This function h is called the hypothesis.

Size in feet | Price in 1000's
---| ---
2104 | 460
1416 | 232
1534 | 315
852 | 178
... | ...

Hypothesis: $h_\theta(x)=\theta_0+\theta_1x$

$\theta$ = parameters


Choose parameters so that h(x) is close to y for our training set.

For a regression problem (our example), a cost function can be used to measure the accuracy of our hypothesis function.

# Cost Function
The cost function takes an average difference (a fancy version) of all the results of the hypothesis with inputs from x's and the actual output y's.

$$J(\theta_0,\theta_1)=\frac{1}{2m}\sum_{i=1}^m(y_i-y_i)^2=\frac{1}{2m}\sum_{i=1}^m(h_\theta(x_i)-y_i)^2$$

$\frac{1}{2}\bar{x}$, where $\bar{x}$ is the mean of the squares of $h_\theta(x_i)-y_i$, or the difference between the predicted value and the actual value.

Squared error function.
