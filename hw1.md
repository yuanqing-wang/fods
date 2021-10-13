---
layout: post
title: Poisson regression
mathjax: true
---

You are given a dataset of $$ {(x_i, y_i), i = 1,...,n}$$

The $$ x_i $$ are real-valued in $$ \mathcal{R} $$.

The $$ y_i $$ are counts in $$ {0, 1, ... } $$.

You think a Poisson is a good model for the counts.

You need to modify the Poisson so it changes based on $$ x $$.

A good start would be a linear model.

\begin{equation}
P(y|x) = \operatorname{Poisson}(\exp (\beta x))
\end{equation}

1. Write down the negative log-likelihood.
2. Calculate the gradient with respect to $$ \beta $$.
3. Implement a gradient descent algorithm to the maximum likelihood estimate (MLE) of $$ \beta $$.
4. Add a ridge penalty term to $$ \beta $$, calculate the gradient of the penalized MLE, and allow the penalty weight $$ \lambda $$ to be passed in your program as a parameter.
