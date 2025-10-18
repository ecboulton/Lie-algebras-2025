  ### Definition
A **multilinear form** on a vector space $V$ over field $F$ is a map $f:V^k \to F$ that is separately linear in each of its $k$ arguments.
If $k=2$ it is called a **bilinear form**.

We focus on **bilinear forms** $B:V\times V \to F$.
## Properties
###### Symmetric, Hermitian
A bilinear form is called **symmetric** if $B(u,v)=B(v,u)$ for all $u,v\in V$.

A bilinear form is called **antisymmetric** if $B(u,v)=-B(v,u)$.

If the field is $F=\mathbb{C}$, then a bilinear form is called **sesquilinear** or **Hermitian** if $B(u,v)=\overline{B(v,u)}$. This is the complex version of symmetric (and reduces to symmetric when the conjugation is trivial, like in $\mathbb{R}$).
###### Alternating
A bilinear form is called **alternating** if $B(v,v)=0$ for all $v\in V$. 
If the field has $\text{char}(F) \neq 2$, this simplifies to $B(u,v)=-B(v,u)$, antisymmetry.
###### Degenerate
A bilinear form is called **degenerate** if there is a $u_{0}\in V \setminus \{ 0 \}$ such that $B(u,v)=0$ for all $v\in V$. Equivalently, the map $u \mapsto (v \mapsto B(u,v))$ into the dual space has non-zero kernel.

A bilinear form is called **non-degenerate** if $B(u,v)=0$ if and only if $u$ or $v$ are zero.
###### Symplectic
A bilinear form is called **symplectic** if it is both alternating and non-degenerate.
*Note: these only exist on even-dimensional spaces.*
See [[Symplectic group]].
###### Definite
A bilinear form is called **definite** if it takes values which are all positive or negative for any nonzero vector. If it's always positive, it's called **positive-definite**, and likewise for **negative-definite**. These correspond bijectively to symmetric (Hermitian) forms.
###### Inner product
A bilinear form is an **inner product** if it is symmetric/Hermitian and positive-definite.

