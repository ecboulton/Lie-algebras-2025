
As operators, the unitary and orthogonal groups are those which preserve an [[Bilinear form|inner product]]. That is, $\langle u,v \rangle=\langle Au, Av\rangle$.
**Unitary** refers to an operator $A$ on a complex vector space with conjugate transpose $A^*$, and **orthogonal** to an operator $A$ on a real vector space with transpose $A^T$.
## Groups
### Orthogonal group
The **orthogonal group** is the group of orthogonal matrices:
$$
\begin{align}
O(n)& :=\{ A \in GL(n,\mathbb{R}) \; | \; A^T A = I_{n} \} \\
&:= \{ A \in GL(n,\mathbb{R}) \; | \; \langle u,v \rangle = \langle Au, Av \rangle \}
\end{align}
$$
Note that this condition is exactly $A^T=A^{-1}$.

The dimension of $O(n)$ over $\mathbb{R}$ is $\frac{n(n-1)}{2}$, due to the pairwise orthogonality condition on each row/column.

The **special orthogonal group** $SO(n)$ is the group of orthogonal matrices with determinant $1$:
$$
\begin{align}
SO(n):=O(n) \cap SL(n,\mathbb{R})
\end{align}
$$

The dimension of $SO(n)$ over $\mathbb{R}$ is $\text{dim}(O(n))-1=\frac{(n+1)(n-2)}{2}$.

They are [[Core/Lie Group|matrix lie groups]].

### Unitary group
The **unitary group** is the group of unitary matrices: $$
\begin{align}
U(n)& :=\{ A \in GL(n,\mathbb{C}) \; | \; A^* A = I_{n} \} \\
&:= \{ A \in GL(n,\mathbb{C}) \; | \; \langle u,v \rangle = \langle Au, Av \rangle \}
\end{align}
$$Note that this condition is exactly $A^* = A^{-1}$.


The **special unitary group** $SU(n)$ is the group of orthogonal matrices with determinant $1$:
$$
\begin{align}
SO(n):=U(n) \cap SL(n,\mathbb{C})
\end{align}
$$

The dimension of $U(n)$ is $n^2$ over $\mathbb{R}$, and $\frac{n(n-1)}{2}$ over $\mathbb{C}$.
The dimension of $SU(n)$ over $\mathbb{R}$ is $n^2-1$.
###### Proof:
- Complex $n\times n$ matrices have dimension $2n^2$ over $\mathbb{R}$ due to $\mathbb{C}\cong \mathbb{R}^2$. 
- Unitarity has $n$ real constraints from the rows (or columns) being unit length and $\frac{n(n-1)}{2}$ complex constraints from the rows (or columns) being pairwise orthogonal. So $n(n-1)=n^2-n$ real constraints.
- The total number of real constraints is $n^2-n+n=n^2$.
- So the dimension is $2n^2-n^2=n^2$ over $\mathbb{R}$.

They are [[Core/Lie Group|matrix lie groups]].


Dimension is $n^2$ (over $\mathbb{R}$).
	- Complex $n\times n$ matrices have dimension $2n^2$ over $\mathbb{R}$ due to $\mathbb{C}\cong \mathbb{R}^2$. 
	- Unitarity has $n$ real constraints from the rows (or columns) being unit length and $\frac{n(n-1)}{2}$ complex constraints from the rows (or columns) being pairwise orthogonal. So $n(n-1)=n^2-n$ real constraints.
	- The total number of real constraints is $n^2-n+n=n^2$.
	- So the dimension is $2n^2-n^2=n^2$ over $\mathbb{R}$.
Similarly to [[Special linear group|special linear group]], the dimension of $SU(n,\mathbb{C})$ over $\mathbb{R}$ is $n^2-1$.




### Topology
TODO, compactness and connectedness


## Algebras
### Orthogonal

### Unitary
The Lie algebra of $U(n)$ is 
$$
\begin{align}
\mathfrak{u}_{n}& :=\{ X \in M(n,\mathbb{C}) \; | \; \exp(tX) \in U(n) \} \\
&= \{ X \in M(n,\mathbb{C}) \;|\; X^* + X = 0 \}
\end{align}
$$
The additive relation in the Lie algebra corresponds to the multiplication of exponentials.