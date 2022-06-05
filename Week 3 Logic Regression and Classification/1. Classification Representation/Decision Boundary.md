## Decision Boundary
In order to get our discrete 0 or 1 classification, we can translate the output of the hypothesis function as follows:

$h_\theta(x)\ge0.5\rightarrow y=1$
$h_\theta(x)<0.5\rightarrow y=1$

The way our logistic function $g$ behaves is that when its input is greather than or equal to $0.5$:

$g(z)\ge0.5$
when $z\ge0$

Remember.

$z=0,e^0=\implies g(z)=\frac{1}{2}$
$z\rightarrow\infty,e^{-\infty}\rightarrow0\implies g(z)=1$
$z\rightarrow-\infty,e^\infty\rightarrow\infty\implies g(z)=0$

So if our input to $g$ is $\theta^TX$, then that means:

$h_\theta(x)=g(\theta^Tx_\ge0.5)$
when $\theta^Tx\ge0$

From these statements we can now say:
