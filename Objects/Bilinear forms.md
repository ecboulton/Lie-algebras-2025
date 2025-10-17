  ### Definition
A **multilinear form** on a vector space $V$ over field $F$ is a map $f:V^k \to F$ that is separately linear in each of its $k$ arguments.
If $k=2$ it is called a **bilinear form**.

We focus on **bilinear forms** $B:V\times V \to F$.
## Properties
###### Symmetric
A bilinear form is called **symmetric** if $B(u,v)=B(v,u)$ for all $u,v\in V$.

A bilinear form is called **antisymmetric** if $B(u,v)=-B(v,u)$.
###### Alternating
A bilinear form is called **alternating** if $B(v,v)=0$ for all $v\in V$. 
If the field has $\text{char}(F) \neq 2$, this simplifies to $B(u,v)=-B(v,u)$, antisymmetry.
###### Degenerate
A bilinear form is called **degenerate** if there is a $u_{0}\in V \setminus \{ 0 \}$ such that $B(u,v)=0$ for all $v\in V$. Equivalently, the map $u \mapsto (v \mapsto B(u,v))$ into the dual space has non-zero kernel.

A bilinear form is called **non-degenerate** if $B(u,v)=0$ if and only if $u$ or $v$ are zero.
###### Symplectic
A bilinear form is called **symplectic** if it is both alternating and non-degenerate.

