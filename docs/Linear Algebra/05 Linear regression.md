# Linear Regression
## Given data

Let us consider a set of datapoints $\{(x_1,y_1),(x_2,y_2),\dots(x_n,y_n)\},$ where $x_i\in\R^d.$

Let us define a **loss function** $L(\theta)=\sum_{i=1}^{n}(x^T_i\theta-y_i)^2$

## Basic Setup

Let us define a **feature matrix** $A=\begin{bmatrix}x_1^T\\x_2^T\\.\\.\\.\\x^T_n\end{bmatrix}$ 

and another matrix $Y=\begin{bmatrix}y_1\\y_2\\.\\.\\.\\y_n\end{bmatrix}$

Now, $A\theta=\begin{bmatrix}x_1^T\theta\\x_2^T\theta\\.\\.\\.\\x^T_n\theta\end{bmatrix}$

Now $(A\theta-Y)=\begin{bmatrix}x_1^T\theta-y_1\\x_2^T\theta-y_2\\.\\.\\.\\x^T_n\theta-y_n\end{bmatrix}$

Now $(A\theta-Y)^T(A\theta-Y)=\begin{bmatrix}(x_1^T\theta-y_1)^2\\(x_2^T\theta-y_2)^2\\.\\.\\.\\(x^T_n\theta-y_n)^2\end{bmatrix}=\sum_{i=1}^{n}(x^T_i\theta-y_i)^2$

So now, the **loss function** $L=(A\theta-Y)^T(A\theta-Y)$

## Minimising Loss function

To minimise the **loss function** $L,$ we equate the ***gradient of loss function*** to $0,$ i.e., $\nabla_\theta L(\theta)=0$

$\to\nabla_\theta((A\theta-Y)^T(A\theta-Y)) = 0$

$\to A^T(A\theta-Y)=0$

$\to (A^TA)\theta=A^TY$

!!! note
    If $A$ is full rank then, $\theta=(A^TA)^{-1}A^TY.$

!!! tip 
    The application of $\theta$ is in finding the Maximum Likelihood Probability.

## Ridge Regression (Regularised version of Linear Regrssion)
Instead of solving the **loss function** $L(\theta)=\sum_{i=1}^{n}(x^T_i\theta-y_i)^2,$ we solve the following regularised version:

$\bar{L}(\theta)=\sum_{i=1}^{n}(x^T_i\theta-y_i)^2+\lambda||\theta||^2,$ where $\lambda||\theta||^2$ is the **regularization term** and then minimise it.

Now, if you minimise this using the above calculations, we get $(A^TA+\lambda I)\theta_{reg}=A^TY\to\theta=(A^TA+\lambda I)^{-1}A^TY$

!!! note
    $(A^TA+\lambda I) $ is invertible even if $A$ is not of full rank