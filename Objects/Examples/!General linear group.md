## Lie group
$GL(n,F)$ is the group of $n \times n$ invertible matrices with entries in $F$. Any closed subgroup of $GL(n,F)$ is a Lie group, in particular a [[!Lie Group|matrix Lie group]].

Dimension is $n^2$ over $F$ since it is an open submanifold (via the continuous determinant map) of $M(n,F)$, which has dimension $n^2$.

### Topological structure
The topology comes from the matrix inner product, which is $||\cdot||: M(n, F) \to \mathbb{R}_{\geq 0}$ defined by 
$$
\begin{align}
\langle A, B \rangle & := \mathrm{Tr}(\overline{B}A) \\
||A||&:=\langle A, A \rangle^{1/2} = \left( \sum_{i,j} |a_{ij}|^2 \right)^{1/2}
\end{align}
$$



## Lie algebra