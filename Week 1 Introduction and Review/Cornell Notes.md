## Week 1

### Introduction

What is machine learning?
- Machine learning is the study of how to give computers the ability to learn without explicitly being programmed.
- This is an older but still useful definition
- A more modern definition is "A computer program is said to learn from experience E with respect to some class of tasks T and performance measure P, if its performance at tasks in T, as measured by P, improves with experience E."

Supervised vs Unsupervised learning
- Supervised learning is when we are given a data set, we already know what our "correct" output should look like, and so we have an idea that there is a relationship between the input and output.
- Unsupervised learning allows us to derive structure from data when we don't neccesarily know the effect of variables

### Model and Cost Function

How do we denote "input" variables?
- We use the symbol $x^{(i)}$
- These are also called input features

How do we denote "output" variables?
- We use the symbol $y^{(i)}$
- These are also called output features

What is a training example?
- A pair $(x^{(i)},y^{(i)})$ is called a training example

What is a training set?
- A training set is a list of $m$ training examples $(x^{(i)},y^{(i)});i=1,...,m$
- The superscript "(i)" in the notation is simply an index for the training set

What is the use of a cost function?
- A cost function is used to measure the accuracy of a hypothesis, it takes an average difference of all the results of the hypothesis with inputs from x's and the actual output y's
- $J(\theta_0,\theta_1)=\frac{1}{2m}\sum\limits_{i=1}^m(\hat y_i-y_i)^2=\frac{1}{2m}\sum\limits_{i=1}^m(h_\theta(x_i)-y_i)^2$

