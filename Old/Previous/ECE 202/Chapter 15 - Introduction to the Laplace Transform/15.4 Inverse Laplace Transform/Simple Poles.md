Recall that a simple pole is a first-order pole. if $F(s)$ has only simple poles, than $D(s)$ becomes a product of factors so that:
$$
F(s)= \frac{N(s)}{(s+p_{1})(s+p_{2})\dots(s+p_{n})}
$$
where $s=-p_{1},-p_{2},\dots,-p_{n}$ are simple poles and $p_{i} \ne p_{j}$ for all $i \ne j$ (i.e., the poles are distinct). Assuming that the degree of $N(s)$ is less than the degree of $D(s)$, we use [[Partial Fraction Decomposition]] to decompose $F(s)$ 
$$
F(s)=\frac{k_{1}}{s+p_{1}}+\frac{k_{2}}{s+p_{2}}+\dots+\frac{k_{n}}{s+p_{n}}
$$
The expansion of coefficients $k_{1},k_{2},\dots ,k_{n}$ are known as the *residues* of $F(s)$. There are many ways of finding the expansion of coefficients.

One way is the *residue method*. If we multiply both sides by $(s+p_{1})$ we obtain
$$
(s+p_{1})F(s)=k_{1}+\frac{(s+p_{1})k_{2}}{s+p_{2}}+\dots+\frac{(s+p_{1})k_{n}}{s+p_{n}}
$$
Because $p_{i}\ne p_{j}$ setting $s=p_{1}$ in the above equation leaves only $k_{1}$ on the right-hand side
$$
(s+p_{1})F(s)|_{s=p_{1}}=k_{1}
$$
Thus in general:
$$
k_{i}=(s+p_{i})F(s)|_{s=p_{i}}
$$
