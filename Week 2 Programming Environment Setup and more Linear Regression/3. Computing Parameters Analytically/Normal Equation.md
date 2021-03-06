Gradient descent gives one way of minimizing $J$. Let's discuss a second way of doing so, this time performing the minimization explicitly and without resorting to an iterative algorithm. In the "Normal Equation" method, we will minimize $J$ by explicitly taking its derivatives with respect to the $\theta_j$, and setting them to $0$. This allows us to find the optimum theta without iteration. The normal equation formula is given below:

$\theta(X^TX)^{-1}X^Ty$

Examples: $m=4$

![](images/Pasted%20image%2020220603100916.png)

There is no need to do feature scaling with the normal equation.

The following is a comparison of gradient descent and the normal equation:

| Gradient Descent             | Normal Equation                               |
| ---------------------------- | --------------------------------------------- |
| Need to choose alpha         | No need to choose alpha                       |
| Needs many iterations        | No need to iterate                            |
| $O(kn^2)$                        | $O(n^3)$, need to calculate inverse of $X^TX$ |
| Works well when $n$ is large   | Slow if $n$ is very large                     |

With the normal equation, computing the inversion has complexity $\mathcal{O}(n^3)$. So if we have a very large number of features, the normal equation will be slow. In practice, when $n$ exceeds $10,000$ it might be a good time to go from a normal solution to an iterative process.