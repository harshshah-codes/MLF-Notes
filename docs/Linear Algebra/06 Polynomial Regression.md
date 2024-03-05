# Polynomial Regression

It is a method of fitting a $n$ degree polynomial through a given set of datapoints

## Given Data

Let some ***one-dimensional*** datapoints be defined as $\{(x_1,y_1),(x_2,y_2),\dots(x_n,y_n)\}$ where $(x_i,y_i)\in R\ \forall\ i$

## Basic Setup

Let $\hat{y}(x) = \theta_1+\theta_2x+\theta_3x^2\dots\theta_nx^n = \sum_{j=0}^n\phi_j(x),$ where $\phi_j(x)=x^j$

Therefore, for a given $x,$ $\phi(x)=(1,x,x^2,\dots x^n)$

Now, $\hat{y}(x) = \theta^T\phi(x)$

## Applying Linear Regression
Now we apply linear regression on $\phi(x), $

So here $A=\begin{bmatrix}\phi(x_1)^T\\\phi(x_2)^T\\.\\.\\.\\\phi(x_n)^T\end{bmatrix}.$

Now $(A^TA)\theta=A^TY$

