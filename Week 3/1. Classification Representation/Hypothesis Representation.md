We could approach the classification problem ignoring the fact that $y$ is descrete-valued, and use our old linear regression algorithm to try to predict $y$ given $x$. However, it is easy to construct examples where this method performs very poorly. Intuitively, it also doesn't make sense for $h_\theta(x)$ to take values larger than $1$ or smaller than $0$ when we know that $y\in\{0,1\}$. To fix this, let's change the form for our hypotheses $h_\theta(x)$ to satisfy $0\le h_\theta(x)\le1$. This is accomplished by plugging $\theta^Tx$ into the Logistic Function.

Our new form uses the "Sigmoid Function," also called the "Logistic Function":

$h_\theta(x)=g(\theta^Tx)$
$z=\theta^Tx$
