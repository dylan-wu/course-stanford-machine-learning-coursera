Gradient descent gives one way of minimizing $J$. Let's discuss a second way of doing so, this time performing the minimization explicitly and without resorting to an iterative algorithm. In the "Normal Equation" method, we will minimize $J$ by explicitly taking its derivatives with respect to the $\theta_j$, and setting them to $0$. This allows us to find the optimum theta without iteration. The normal equation formula is given below:

$\theta(X^TX)^{-1}X^Ty$

Examples: $m=4$

![[Pasted image 20220603100916.png]]

There is no need to do feature scaling with the normal equation.

The following is a comparison of gradient descent and the normal equation:

| Gradient Descent \ N