# Unsupervised Learning

Unsupervised Learning is used to 'understand data'.

In contrast to [**Supervised Learning**](/01%20Supervised%20Learning%20-%20MLF) where the data is some inputs and their outputs, the data in **Unsupervised Learning** is just a set of inputs and no outputs, i.e., data is of the form $\{x^1,x^2,x^3,...,x^n\}$, where $x^i\in\mathbb{R}^d$.

!!! note

    They build models that compress, explain and group data.

## Dimensionality Reduction

### Basic Setup

Data: $\{x^1,x^2,x^3...,x^n\}$, where $x^i\in\mathbb{R}^d$

#### Encoder

The goal of the encoder is to take in a $d$-dimensional vector and compress it to give a $d'$-dimensional vector.

Mathematically, Encoder $f:\mathbb{R}^d\to\mathbb{R}^{d'}$

!!! tip Remember

    Typically $d'<d$

#### Decoder

The goal of the decoder is to take in a $d'$-dimensional vector and decompress it to give a $d$-dimensional vector.

Mathematically, Decoder $g:\mathbb{R}^{d'}\to\mathbb{R}^{d}$

!!! tip Remember

    Typically $d'<d$

### Goal

Goal of the dimensionality reduction is **$g(f(x^i))\approx x^i$**

### Loss

Loss of the dimensionality reduction is

$$
\text{Loss} = \cfrac{1}{n}\sum_{i=1}^{n}||g(f(x^i)) - x^i||^2
$$

### Uses of Dimensionality Reduction

Dimensionality Reduction finds its main uses in **compression** and **reduction**.

!!! tip Remember

    The Dimensionality Reduction comes up with two models, i.e. the [**Encoder**](#encoder) and the [**Decoder**](#decoder).

## Density Estimation

It gives out a probabilistic model, i.e., the output is a model that stores different configurations of reality.

### Basic Setup

Data: $\{x^1,x^2,x^3,\dots,x^n\}$, where $x^i\in\mathbb{R}^d$

#### Probabilistic Model

It gives out a probabilistic model $P:\mathbb{R}^d\to\mathbb{R}_+$.

!!!tip Remember

    All outputs sums up to $1$, i.e., $\sum_{i=1}^nP(x^i) = 1$

#### Goal
The goal of probability estimation is to to give a probabilistic model $P$ such that $P(x)$ is large if $x\in\text{Data}$, and low otherwise.

#### Loss 
Loss for the probabilistic model $P$ is **negative log likelihood**, i.e., 

$$
\text{Loss} = \cfrac{1}{n} \sum_{i=1}^n-log(P(x^i))
$$