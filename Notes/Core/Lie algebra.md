Def
Examples
Subalgebras, ideals, quotients
Ad map
## Definitions and core properties
### Lie algebra definition
A **Lie algebra** $\mathfrak{g}$ is a vector space over a field $F$, equipped with a **Lie bracket** map $[\cdot,\cdot]: \mathfrak{g} \times \mathfrak{g} \to \mathfrak{g}$ which is:
1. [[Bilinear form|Bilinear]].
2. [[Bilinear form|Alternating]]: for all $X \in \mathfrak{g}$, we have $[X,X]=0$.
	- Note this may be replaced in $\text{char}(F)\neq 2$ by [[Bilinear form|asymmetry]] $[X,Y]=-[Y,X]$. However, the [[Bilinear form|alternating]] condition is stronger.
3. Satisfies the **Jacobi identity**: for all $X,Y,Z \in \mathfrak{g}$, we have $[X,[Y,Z]]+[Z,[X,Y]]+[Y,[Z,X]]=0$.

For associative algebras, the Lie bracket is the commutator $[a,b]:=ab-ba$.
#### Note on definition
Property 2 (alternating, $[X,X]=0$) implies anticommutativity, $[X,Y]=-[Y,X]$. In $\text{char}(F)\neq 2$ they are equivalent.

### Morphisms of Lie algebras
A **morphism of Lie algebras** is a map $\phi:\mathfrak{g} \to \mathfrak{g}'$ which is linear and for which $\phi([X,Y]) = [\phi(x),\phi(Y)]$.

### Subalgebras
#### Definition
Given a Lie algebra $\mathfrak{g}$, a subspace $\mathfrak{a}$ is a **Lie subalgebra** if it is closed under the Lie bracket. That is, $[A,B] \in \mathfrak{a}$ whenever $A,B \in \mathfrak{a}$.

#### Examples
The subspace $\mathfrak{sl}(n,F) \subset \mathfrak{gl}(n,F)$ is the subspace in $M(n,F)$ of traceless matrices. Any product and sum of traceless matrices is traceless, so the Lie bracket preserves tracelessness. So $\mathfrak{sl}(n,F)$ is a subalgebra of $\mathfrak{gl}(n,F)$.

The Lie algebras $\mathfrak{o}(n), \mathfrak{so}(n), \mathfrak{u}(n), \mathfrak{su}(n)$ are defined over $\mathbb{R}$ and $\mathbb{C}$ respectively, so they are subalgebras of $\mathfrak{gl}(n,F)$ by Ado's theorem.

#### Ado's theorem
In fact, when $\text{char}(F)=0$, every finite dimensional Lie algebra is a subalgebra of $\mathfrak{gl}(n,F)$.
This theorem is useful to prove Lie's [[Connecting Lie groups and algebras|third theorem]].

### Ideals
#### Definition
A subalgebra $\mathfrak{a}$ of $\mathfrak{g}$ is an **ideal** of $\mathfrak{g}$ if $[\mathfrak{g},\mathfrak{a}] \subseteq \mathfrak{a}$. That is, $[x,a] \in \mathfrak{a}$ for every $x\in \mathfrak{g}, a \in \mathfrak{a}$.
This is denoted $\mathfrak{a} \;\triangleleft\; \mathfrak{g}$.

Note that $\mathfrak{a} \; \triangleleft \; \mathfrak{b}$ and $\mathfrak{b} \; \triangleleft \; \mathfrak{c}$ does not necessarily mean $\mathfrak{a} \; \triangleleft \; \mathfrak{c}$. That is, it is not transitive.

#### Properties
TODO: properties of ideals (closure etc)
#### Examples
* The kernel of a Lie algebra homomorphism $\phi: \mathfrak{g}_{1} \to \mathfrak{g}_{2}$ is an ideal $\text{ker}\phi \; \triangleleft \; \mathfrak{g}_{1}$.
	* *Image is not necessarily an ideal.*
* The centre of a Lie algebra $Z(\mathfrak{g}):=\{ x \in \mathfrak{g} \; | \;[x,y]=0 \quad \forall y \in \mathfrak{g} \} \; \triangleleft \; \mathfrak{g}$.
* The derived subalgebra $[\mathfrak{g}, \mathfrak{g}] \; \triangleleft \; \mathfrak{g}$.
* For $\mathfrak{a,b} \; \triangleleft \; \mathfrak{g}$, the subalgebra $\mathfrak{a+b}$ defined as follows, is an ideal.
	* $\mathfrak{a+b}:=\{ x+y \; | \; x \in \mathfrak{a}, y \in \mathfrak{b} \}$
	* $[\mathfrak{a},\mathfrak{b}]:=\left\{  \sum_{i} [x_{i}, y_{i}] \; | \; x_{i} \in \mathfrak{a}, y_{i} \in \mathfrak{b}  \right\}$

### Quotients
For a Lie algebra $\mathfrak{g}$ and an ideal $\mathfrak{a} \; \triangleleft \; \mathfrak{g}$, we define the **quotient Lie algebra** as $$
\begin{align}
\mathfrak{g} / \mathfrak{a} & := \{ x + \mathfrak{a} \; | \; x \in \mathfrak{g}\} \\
[x+\mathfrak{a}, y+\mathfrak{a}] & := [x,y] + \mathfrak{a}
\end{align}
$$

### Isomorphism theorems
#### First isomorphism theorem
If $\phi: \mathfrak{g} \to \mathfrak{h}$ is a Lie algebra homomorphism, then $$
\mathfrak{g} / \text{ker}(\phi) \cong \text{im}(\phi)
$$
#### Second isomorphism theorem
Let $\mathfrak{a,b} \; \triangleleft \; \mathfrak{g}$. Then $$
(\mathfrak{a+b}) / \mathfrak{a} \cong \mathfrak{b} / (\mathfrak{a} \cap \mathfrak{b})
$$

#### Third isomorphism theorem
Let $\mathfrak{a,b} \; \triangleleft \; \mathfrak{g}$ with $\mathfrak{a} \subseteq \mathfrak{b}$. Then $$
(\mathfrak{g} / \mathfrak{a}) / (\mathfrak{b} / \mathfrak{a}) \cong \mathfrak{g} / \mathfrak{b}
$$
#### Correspondence theorem
Let $\phi: \mathfrak{g} \to \mathfrak{g}'$ be a surjective Lie algebra homomorphism with kernel $\mathfrak{a}$. Then there is a bijective correspondence $$
\begin{align}
\{ \text{subalgebras of } \mathfrak{g} \text{ containing } \mathfrak{a} \} & \leftrightarrow \{ \text{subalgebras of } \mathfrak{g}' \} \\
\mathfrak{h} &\leftrightarrow  \phi(\mathfrak{h}) =: \mathfrak{h}'
\end{align}
$$
Also, $\mathfrak{h} / \mathfrak{a} \cong \mathfrak{h}'$ and $\mathfrak{h} \; \triangleleft \; \mathfrak{g} \iff \mathfrak{h}' \; \triangleleft \; \mathfrak{g}'$.

## Conceptual insight
Let $G$ be a Lie group with Lie algebra $\mathfrak{g}$. There is a natural vector space identification between $\mathfrak{g}$ and the tangent space $T_{1_{G}} G$, via the [[Exponential and logarithm maps|exponential map]]. 

## Adjoint map

With anticommutativity, the Jacobi identity is expressible as a derivation of the [[Adjoint maps|adjoint map]].
**TODO**

## Examples
[[General linear group]]: $\mathfrak{gl}(n,F)=M(n,F)$
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




