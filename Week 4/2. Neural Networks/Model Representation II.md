To re-iterate, the following is an example of a neural network:

In this section we'll do a vectorized implementation of the above functions. We're going to define a new variable $z_k^{(j)}$ that encompasses the parameters inside our g function. In our previous example if we replaced by the variable z for all the parameters we would get:

$a_1^{(2)}=g(z_1^{(2)})$
$a_2^{(2)}=g(z_2^{(2)})$
$a_3^{(2)}=g(z_3^{(2)})$

In other words, for layer $j=2$ and node $k$, the variable $z$ will be:

$z_k^{(2)}=\Theta^{(1)}_{k,0}x_0+\Theta^{(1)}_{k,1}x_1+...+\Theta^{(1)}_{k,n}x_n$

We are multiplying our matrix $\Theta^{(j-1)}$ with dimensions $s_j\times(n+1)$ (where $s_j$ is the number of our activation nodes) by our vector $a^{(j-1)}$ with height $(n+1)$. This gives us our vector $z^{(j)}$ with height $s_j$. Now we can get a vector of our activation nodes for layer $j$ as follows:

$a^{(j)}=g(z^{(j)})$

