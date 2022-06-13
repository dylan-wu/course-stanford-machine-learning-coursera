Leftmost figure below shows the result of fitting a $y=\theta_0+\theta_1x$ to a dataset. We see the data doesn't exactly lie on the straight line, and so the fit is not that good.

![[Pasted image 20220613091402.png]]

How do we fix this?
- We could add an extra feature $x^2$, and fit $y=\theta_0+\theta_1x+\theta_2x^2$, then we'd obtain a slightly better fit to the data.
- This does not mean that adding more features is always better, there is a danger in adding too many features.
- The figure on the right for example, is from fitting a $5^{th}$ order polynomial.

The figure on the right is overfitting, while the figure on the left is underfitting