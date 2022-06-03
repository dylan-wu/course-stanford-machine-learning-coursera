When implementing the normal equation in octave we want to use the 'pinv' function rather than 'inv.' The 'pinv' function will give you a value of $\theta$ even if $X^TX$ is not invertible.

If $X^TX$ is **noninvertible**, the common causes might be having:
- Redundant features, where two features are very closely related (i.e. they are linearly dependent)
- Too many features (e.g. $m\le n$). In this case, delete some features or use "regularization" (to be explained in a later l)