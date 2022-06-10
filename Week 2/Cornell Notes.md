## Multivariate Linear Regression

What is multivariate linear regression?
- Linear regression with multiple variables
- Computed using formulas that allow any number of input variables

What is the notation for multivariable input equations?
- $x^{(i)}_j=$ value of feature $j$ in the $i^{th}$ training example
- $x^{(i)}=$ the input (features) of the $i^{th}$ training example
- $m=$ the number of training examples
- $n=$ the number of features

What is a multivariable form of hypothesis functions accomodating multiple features?
- $h_\theta(x)=\theta_0+\theta_1x_1+\theta_2x_2+\theta_3x_3+...+\theta_nx_n$

How do you use Gradient Descent for multiple variables?
- $\theta_0:=\theta_0-\alpha\frac{1}{m}\sum\limits_{i=1}^m(h_0(x^{(i)})-y^{(i)})\cdot x_0^{(i)}$
- $\theta_1:=\theta_1-\alpha\frac{1}{m}\sum\limits_{i=1}^m(h_0(x^{(i)})-y^{(i)})\cdot x_1^{(i)}$
- $\theta_2:=\theta_2-\alpha\frac{1}{m}\sum\limits_{i=1}^m(h_0(x^{(i)})-y^{(i)})\cdot x_2^{(i)}$

Why do you want your input values all roughly in the same range for gradient descent
- $\theta$ will quickly descend on small ranges and slowly on large ranges, and so will oscillate inefficiently down to the optimum when the variables are uneven

How do you prevent this oscillation of $\theta$
- Ideally, you would modify the ranges of your input variables to be:
- $-1\le x_{(i)}\le1$ or $-0.5\le x_{(i)}\le0.5$

How do you debug gradient descent?
- Make a plot with the number of iterations on the x-axis. Plot the cost function $J(\theta)$ over the number of iterations of gradient descent.
- If $J(\theta)$ decreases, then you probably need to increase $\alpha$

What is an automatic convergence test?
- Declare convergence if $J(\theta)$ decreases by less than $E$ in one iteration, where $E$ is some small value like $10^{-3}$.
- In practice, however, it's difficult to choose the threshold value.

What happens if $\alpha$ is too small/too large?
- Too small: slow convergence
- Too large: $J(\theta)$ may not decrease on every iteration and thus may not converge

How do we combine multiple features into one?
- We can combine $x_1$ and $x_2$ into a new feature $x_3$ by taking $x_1\cdot x_2$

How do you change the behavior or curve of your hypothesis function?
- Make it quadratic, cubic or square root function

Give an example of the above two manipulations:
- If our hypothesis function is $h_\theta(x)=\theta_0+\theta_1x_1$, then we can create additional features based on $x_1$, to get a quadratic function $h_\theta(x)=\theta_0+\theta_1x_1+\theta_2x^2_1$ or even the cubic function $h_\theta(x)=\theta_0+\theta_1x_1+\theta_2x^2_1+\theta_3x^3_1$
- To make a square root function, we might do: $h_\theta(x)=\theta_0+\theta_1x_1+\theta_2\sqrt{x_1}$

