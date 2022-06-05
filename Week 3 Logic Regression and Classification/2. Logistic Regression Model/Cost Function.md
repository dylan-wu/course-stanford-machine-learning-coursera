We cannot use the same cost function that we use for linear regression because the Logistic Function will cause the output to be wavy, causing many local optima. In other words, it will not be a convex function.

Instead, our cost function for logistic regression looks like:

$J(\theta)=\frac{1}{m}\sum\limits_{i=1}^m\text{Cost}(h_\theta(x^{(i)}),y^{(i)})$
$\text{Cost}(h_\theta(x^{(i)}),y^{(i)})=-\log(h_\theta(x))$
$\text{Cost}(h_\theta(x^{(i)}),y^{(i)})=-\log(1-h_\theta(x))$ if $y=0$
