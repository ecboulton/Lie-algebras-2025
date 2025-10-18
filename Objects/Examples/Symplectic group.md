## Definitions
### Symplectic form
A symplectic form is a bilinear form $B(\cdot,\cdot):F^{2n} \times F^{2n} \to F$ which is
- Nondegenerate
- Alternating: $B(v,v)=0$ for all $v\in F^{2n}$.
	- In $\text{char}(F)\neq 2$, this is equivalent to antisymmetric, $B(v,u)=-B(u,v)$.

*Symplectic forms only exist in even-dimensional spaces.*

The symplectic form is of the form
$$
J:=\begin{pmatrix}
0 & I_{n} \\
-I_{n} & 0
\end{pmatrix} \in GL(2n,F)
$$

### Symplectic space
A space equipped with a symplectic form $B$ is a **symplectic space**. Necessarily these spaces are even-dimensional over $F$. Symplectic spaces of the same dimension are unique up to change of basis (isomorphism).

### Symplectic group

The **symplectic group** is $$
Sp(2n,F)=\{ A \in GL(2n, F) \; | \; A^T JA =J\} \subset SL(2n,F)
$$
The fact that the determinant is $\pm 1$ follows from the definition, and in fact it is $+1$ for fields $F$.

~~It has degree $n(2n+1)$ over $F$.~~


