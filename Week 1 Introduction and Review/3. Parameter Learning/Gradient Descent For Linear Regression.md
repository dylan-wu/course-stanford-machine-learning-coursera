## Gradient Descent For Linear Regression 

When specifically applied to the case of linear regression, a new form of the gradient descent equation can be derived. We can substitute our actual cost function and our actual hypothesis function and modify the equation to:

$\theta_0:=\theta_0-\alpha\frac{1}{m}\sum\limits_{i=1}^m(h_\theta(x_i)-y_i)$

$\theta_1:=\theta_1-\alpha\frac{1}{m}\sum\limits_{i=1}^m((h_\theta(x_i)-y_i)x_i)$

