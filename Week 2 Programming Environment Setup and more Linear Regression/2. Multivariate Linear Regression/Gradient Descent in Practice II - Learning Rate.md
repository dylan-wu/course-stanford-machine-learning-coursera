**Note:** [5:20 - the x -axis label in the right graph should be \thetaθ rather than No. of iterations ]

**Debugging gradient descent.** Make a plot with _number of iterations_ on the x-axis. Now plot the cost function, $J(\theta)$ over the number of iterations of gradient descent. If $J(\theta)$ ever increases, then you probably need to decrease $\alpha$.

**Automatic convergence test**. Declare convergence if $J(\theta)$ decreases by less than $E$ in one iteration, where $E$ is some small value such as $10^{-3}$. However, in practice it's difficult to choose this threshold value.

![](Pasted%20image%2020220602083326.png)
It has been proven that if learning rate $\alpha$ is sufficiently small, then $J(\theta)$ will decrease on every iteration.

![](Pasted%20image%2020220602083552.png)

To summarize:

If $\alpha$ is too small: slow convergence.

If $\alpha$ is too large: may not decrease on every iteration and thus may not converge.

