To re-iterate, the following is an example of a neural network:

In this section we'll do a vectorized implementation of the above functions. We're going to define a new variable $z_k^{(j)}$ that encompasses the parameters inside our g function. In our previous example if we replaced by the variable z for all the parameters we would get:

$a_1^{(2)}=g(z_1^{(2)})$
$a_2^{(2)}=g(z_2^{(2)})$
$a_3^{(2)}=g(z_3^{(2)})$

In other words, for layer $j=2$ and node $k$, the variable $z$ will be:

$z_k^{(2)}=\Theta^{(1)}__$