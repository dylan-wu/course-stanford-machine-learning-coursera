When implementing the normal equation in octave we want to use the 'pinv' function rather than 'inv.' The 'pinv' function will give you a value of $\theta$ even if $X^TX$ is not invertible.

If $X^TX$ is **noninvertible**, the common causes might be having:
