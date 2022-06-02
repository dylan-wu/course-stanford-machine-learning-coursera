We can improve our features and the form of our hypothesis function in a couple different ways..

We can **combine** multiple features into one. For example, we can combine $x_1$ and $x_2$ into a new feature $x_3$ by taking $x_1\cdot x_2$.

**Polynomial Regression**

Our hypothesis function need not be a linear (a straight line) if that does not fit the data well.

We can **change the behavior or curve** of our hypothesis function by making it a quadratic, cubic or square root function (or any other form).

For example, if our hypothesis function is $h_\theta(x)=\theta_0+\theta_1x_1$ then we can create additional features based on $x_1$, to get the quadratic function $h_\theta(x)=\theta_0+\theta_1x_1+\theta_2x_1^2$ or the cubic function $h_\theta(x)=\theta_0+\theta_1x_1+\theta_2x_1^2+\theta_3x^3_1$

In the cubic version, we have created new features $x_2$ and $x_3$ where $x_2= _1^2$ and $x_3=x_1^3$.

To make it a square root function, we could do: h_\theta(x) = \theta_0 + \theta_1 x_1 + \theta_2 \sqrt{x_1}hθ​(x)=θ0​+θ1​x1​+θ2​x1​​

One important thing to keep in mind is, if you choose your features this way then feature scaling becomes very important.

eg. if x_1x1​ has range 1 - 1000 then range of x_1^2x12​ becomes 1 - 1000000 and that of x_1^3x13​ becomes 1 - 1000000000