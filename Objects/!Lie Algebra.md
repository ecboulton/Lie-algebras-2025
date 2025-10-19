## Lie algebra 
### Definition
A **Lie algebra** $\mathfrak{g}$ is a vector space over a field $F$, equipped with a **Lie bracket** map $[\cdot,\cdot]: \mathfrak{g} \times \mathfrak{g} \to \mathfrak{g}$ which is:
1. [[Bilinear forms|Bilinear]].
2. [[Bilinear forms|Alternating]]: for all $X \in \mathfrak{g}$, we have $[X,X]=0$.
	- Note this may be replaced in $\text{char}(F)\neq 2$ by [[Bilinear forms|antisymmetry]]: $[X,Y]=-[Y,X]$. However, the [[Bilinear forms|alternating]] condition is stronger.
3. Satisfies the **Jacobi identity**: for all $X,Y,Z \in \mathfrak{g}$, we have $[X,[Y,Z]]+[Z,[X,Y]]+[Y,[Z,X]]=0$.

For associative algebras, the Lie bracket is the commutator $[a,b]:=ab-ba$.

### Conceptual insight
Let $G$ be a Lie group with Lie algebra $\mathfrak{g}$. There is a natural vector space identification between $\mathfrak{g}$ and the tangent space $T_{1_{G}} G$, via the [[!Exponential and logarithm maps|exponential map]]. 

### Properties
Property 2 (alternating, $[X,X]=0$) implies anticommutativity, $[X,Y]=-[Y,X]$. In $\text{char}(F)\neq 2$ they are equivalent.

With anticommutativity, the Jacobi identity is expressible as a derivation of the [[Adjoint maps|adjoint map]].


### Examples
[[!General linear group]]: $\mathfrak{gl}(n,F)=M(n,F)$
- All matrix Lie groups are submanifolds of $GL(n,F)$ so their algebras (and more generally tangent spaces) are subsets of $\mathfrak{gl}(n,F)=M(n,F)$.

[[Special linear group]]: $\mathfrak{sl}(n,F)=\{ X \in M(n,F) \; | \; \mathrm{Tr}(X)=0 \}$

[[Orthogonal and unitary groups]]: 
* $\mathfrak{o}(n)=\{ X \in M(n,\mathbb{R}) \; | \; X^T = -X \}$
	* $\mathfrak{so}(n)$ is $\mathfrak{o}(n)$ with the condition that $\mathrm{Tr}(X)=0$ due to $\mathfrak{sl}(n)$. This is automatically true when $X^T=-X$.
	* $\mathfrak{so}(n)=\mathfrak{o}(n)$
* $\mathfrak{u}(n)=\{ X \in M(n,\mathbb{C}) \; | \; X^* = -X \}$
	* $\mathfrak{su}(n)$ is $\mathfrak{u}(n)$ with the condition that $\mathrm{Tr}(X)=0$. This is stronger, because $X^*=-X$ only implies the trace is in $i\mathbb{R}$.
	* $\mathfrak{su}(n) \subsetneq \mathfrak{u}(n)$

[[Symplectic group]]: $\mathfrak{sp}(2n,F)=\{ X \in M(2n,F) \; | \; JX+X^TJ=0 \}$

[[Heisenberg group]]: $\mathfrak{h}=\{ X \in M(3,\mathbb{R}) \; | \; X \text{ is strict upper triangular} \}$

## Morphisms
### Definition
A **morphism of Lie algebras** is a map $\phi:\mathfrak{g} \to \mathfrak{g}'$ which is linear and for which $\phi([X,Y]) = [\phi(x),\phi(Y)]$.




