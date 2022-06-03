---
up: [[2. Multivariate Linear Regression]]
---

- [x] 06-01-2022

## Gradient Descent for Multiple Variables

The gradient descent equation itself is generally the same form; we just have to repeat it for our 'n' features:

Repeat until convergence:

$\{\theta_0:=\theta_0-\alpha\frac{1}{m}\sum\limits_{i=1}^m(h_\theta(x^{(i)})-y^{(i)})\cdot x_0^{(i)}$
$\theta_1:=\theta_1-\alpha\frac{1}{m}\sum\limits_{i=1}^m(h_\theta(x^{(i)})-y^{(i)})\cdot x_1^{(i)}$
$\theta_2:=\theta_2-\alpha\frac{1}{m}\sum\limits_{i=1}^m(h_\theta(x^{(i)})-y^{(i)})\cdot x_2^{(i)}\}$

Or:

$\{\theta_j:=\theta_j-\alpha\frac{1}{m}\sum\limits_{i=1}^m(h_\theta(x^{(i)})-y^{(i)})\cdot x_j^{(i)}\text{for }j:=0...n\}$

The following image compared gradient descent with one variable to gradient descent with multiple variables:

![[images/Pasted image 20220601092744.png]]

