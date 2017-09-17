# Boston_Housing_Assignment
In this assignment we use inear regression with batch gradient descent to estimate house prices based on a Boston training set. 

As we know, our goal with linear regression is to fit a linear function to our features so that we can learn some function f(x) that can predict a dependent variable based on a set of independent variables, by learning 'weights' . The general form of the function we're trying to fit is f(x) = θ0 + θ1X1 + θ2X2 + ... + θnXn.

Gradient Descent is a process of determining the best possible values of θ so as to minimize the error rate J. 

To do that, we'll use an optimization algorithm known as 'batch gradient descent.'
On the surface, batch gradient descent is pretty easy:
Repeat Until Converged: { 

$θ = θ – α(δ/(δ θ))J(θ) }

So, every time we update theta, we will set theta equal to the previous value minus $\alpha$ (a learning rate) multiplied by the partial derivative of the cost function J, with respect to θ.

So then if we start with:

θ := θ – α(δ/(δθ))J(θ)

We can substitute the cost function for J, work through the partial derivative, and come to find that the update rule for a single iteration is: 

θ = θ – α(1/2m)∑(yi - ŷi)xi (from i = 1 to m)



