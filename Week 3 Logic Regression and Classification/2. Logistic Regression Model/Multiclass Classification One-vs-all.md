## Multiclass Classification: One-vs-all

Now we will approach the classification of data when we have more than two categories. Instead of y = {0,1} we will expand our definition so that y = {0,1...n}.

Since y = {0,1...n}, we divide our problem into n+1 (+1 because the index starts at 0) binary classification problems; in each one, we predict the probability that 'y' is a member of one of our classes.

$y\in\{0,1...n\}$
$h_\theta^{(0)}(x)=P(y=0|x;\theta)$
$h_\theta^{(1)}(x)=P(y=1|x;\theta)$
$...$
$h_\theta^{(n)}(x)=P(y=n|x;\theta)$
$\text{prediction}=\max_i(h^{(i)}_\theta(x))$

