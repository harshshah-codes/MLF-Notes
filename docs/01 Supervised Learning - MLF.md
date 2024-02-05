# Supervised Learning

## Basic setup

Here are some notations that will be used throughout the course.

$$
\mathbb{R} \rightarrow \text{Real numbers}\\ \mathbb{R}_+ \rightarrow \text{Positive Real numbers}\\ \mathbb{R}^d \rightarrow d\text{ dimensional vector of Real numbers}\\ x \rightarrow \text{vector, } x_j \to j^{th} \text{coordinate of } x\\x^1, x^2, x^3 ...x^n \to \text{Collection of }n \text{ vectors}\\ x^i_j \to j^{th} \text{ coordinate of } i^{th} \text{ vector}\\ (x_1)^2: \text{Square of first coordinate of vector }x
$$

## Regression

Regression at its core is **curve fitting**.

Given some inputs and outputs in the form ${(x^1, y^1), (x^2, y^2)...(x^n, y^n)}$, we find a model $f(x^i)\text{ is closest to } y^i$

Also note that here,

$$
x^i \in \mathbb{R}^d, y^i \in \mathbb{R}
$$

!!! danger "Remember"

    The algorithm outputs a model $f:\mathbb{R}^d\to\mathbb{R}$

!!! warning "Loss"

    Loss of the model $f$ is $ \text{Loss}[f] = \frac{1}{n}\sum_{i=1}^{n}(f(x^i)- y^i)^2$

### General form of Model

$$
f(x) = w^Tx+b=\sum_{j=1}^{d}w_jx_j + b
$$

## Classification

Given some inputs and outputs in the form ${(x^1, y^1), (x^2, y^2)...(x^n, y^n)}$

Also note that here,

$$
x^i \in \mathbb{R}^d, y^i \in \{-1, +1\}
$$

!!! danger "Remember"

    The algorithm outputs a model $f:\mathbb{R}^d\to\{-1, +1\}$

!!! warning "Loss"

    Loss of the model $f$ is $ \text{Loss}[f] = \frac{1}{n}\sum_{i=1}^{n}1(f(x^i) \neq y^i)$

### General form of Model

$$
f(x) = sign(w^Tx+b)
$$
