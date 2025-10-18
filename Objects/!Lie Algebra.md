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
[[!General linear group]]
[[Special linear group]]
[[Orthogonal and unitary groups]]
[[Symplectic group]]
[[Heisenberg group]]

## Morphisms
### Definition
A **morphism of Lie algebras** is a map $\phi:\mathfrak{g} \to \mathfrak{h}$ which is linear and for which $\phi([X,Y]) = [\phi(x),\phi(Y)]$.




