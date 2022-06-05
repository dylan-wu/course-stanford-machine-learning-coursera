We cannot use the same cost function that we use for linear regression because the Logistic Function will cause the output to be wavy, causing many local optima. In other words, it will not be a convex function.

Instead, our cost function for logistic regression looks like:

$J(\theta)=\frac{1}{m}\sum\limits_{i=1}^m\text{Cost}(h_\theta(x^{(i)}),y^{(i)})$
$\text{Cost}(h_\theta(x),y)=-\log(h_\theta(x))$ if $y=1$
$\text{Cost}(h_\theta(x),y)=-\log(1-h_\theta(x))$ if $y=0$

When $y=1$, we get the following plot for $J(\theta)$ vs $h_\theta(x)$:
![[Pasted image 20220605154458.png | 500]]

When $y=0$, we get the following plot for $J(\theta)$ vs $h_\theta(x)$:
![[Pasted image 20220605154517.png | 500]]

