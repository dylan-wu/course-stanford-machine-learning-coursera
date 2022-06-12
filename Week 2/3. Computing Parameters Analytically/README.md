In a normal equation method, what is the formula, and what do we do?
- Minimize $J$ by explicitly taking its derivatives with respect to the $\theta j$s, and setting them to zero.
- Find the optimum theta, without iteration
- $\theta=(X^TX)^{-1}X^Ty$

Do you need to do feature scaling on a normal equation?
- No

![[Pasted image 20220612091452.png]]

Is the normal equation invertible?
- Sometimes $X^TX$ is non-invertible, some causes are:
- Redundant features, where two features are closely related
- Too many features

