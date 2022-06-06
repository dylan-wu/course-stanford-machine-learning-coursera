## Simplified Cost Function and Gradient Descent

**Note:** [6:53 - the gradient descent equation should have a 1/m factor]

We can compress our cost function's two conditional cases into one case:

$\text{Cost}(h_\theta(x),y)=-y\log(h_\theta(x))-(1-y)\log(1-h_\theta(x))$

Notice that when $y$ is equal to $1$, then the second term $(1-y)\log(1-h_\theta(x))$ will be zero and will not aff