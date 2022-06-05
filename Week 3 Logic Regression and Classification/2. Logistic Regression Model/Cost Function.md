We cannot use the same cost function that we use for linear regression because the Logistic Function will cause the output to be wavy, causing many local optima. In other words, it will not be a convex function.

Instead, our cost function for logistic regression looks like:

$J(\theta)=\frac{1}{m}\sum\limits_{i=1}^m\text{Cost}(h_\theta(x^{(i)}),y^{(i)})$
$\text{Cost}(h_\theta(x),y)=-\log(h_\theta(x))$ if $y=1$
$\text{Cost}(h_\theta(x),y)=-\log(1-h_\theta(x))$ if $y=0$

When $y=1$, we get the following plot for $J(\theta)$ vs $h_\theta(x)$:
![[Pasted image 20220605154458.png | 500]]

When $y=0$, we get the following plot for $J(\theta)$ vs $h_\theta(x)$:
![[Pasted image 20220605154517.png | 500]]

$\text{Cost}(h_\theta(x),y)=0$ if $h_\theta(x)=y$
$\text{Cost}(h_\theta(x),y)\rightarrow\infty$ if $y=0$ and $h_\theta(x)\rightarrow1$
$\text{Cost}(h_\theta(x),y)\rightarrow\infty$ if $y=1$ and $h_\theta(x)\rightarrow0$

If our correct answer 'y' is 0, then the cost function will be 0 if our hypothesis function also outputs 0. If our hypothesis approaches 1, then the cost function will approach infinity.

If our correct answer 'y' is 1, then the cost function will be 0 if our hypothesis function outputs 1. If our hypothesis approaches 0, then the cost function will approach infinity.

Note that writing the cost function in this way guarantees that $J(\theta)$ is convex for logistic regression.