## Definition
A **Lie group** is a group $G$ which is also a [[Manifold|smooth manifold]] such that the group multiplication
$$
\begin{align}
 \mu: G \times G & \to G  \\
 (a,b) & \mapsto ab
\end{align}
$$
and inverse operation
$$
\begin{align}
 i: G & \to G \\
a & \mapsto a^{-1}
\end{align}
$$
are smooth ($C^\infty$).

## Matrix (linear) Lie groups
A Lie group which is a closed (under the topology) subgroup of $GL(n,F)$ is called a **matrix/linear Lie group**.
### Examples
[[!General linear group]]
[[Special linear group]]
[[Orthogonal and unitary groups]]
[[Symplectic group]]
[[Heisenberg group]]

### Non-examples
- Elliptic curves over $\mathbb{C}$
- The universal cover of $SL(n,\mathbb{R})$ 

### Topological properties
#### Compactness
A matrix Lie group $G \subset GL(n,F)$ is **compact** if it is closed and bounded (under the [[!General linear group|matrix norm]]) as a subset of $M(n\times n, F) \cong F^{n^2}$.
##### Examples
Every orthogonal/unitary matrix has norm $\sqrt{ n }$, so $U(n), O(n)$ are bounded and closed (hence compact).
$SL(2,\mathbb{C})$ is unbounded, so not compact. Similarly, $SL(n,\mathbb{C})$ and $SL(n,\mathbb{R})$ are unbounded.
 
#### Connectedness
##### Connectedness and path connectedness
A topological space (including manifolds, Lie groups) is **connected** if it cannot be written as a disjoint union of non-empty open sets.

A space is **path connected** if for every $x,y \in X$ there is a continuous map (a path) $f:[0,1] \to X$ with $f(0)=x$ and $f(1)=y$. Every path connected space is connected.

*For manifolds (or generally, 'locally path connected spaces'), the notions of path connectedness and connectedness are equivalent.*

###### Examples
$GL(n,F), SL(n,F),SO(n),U(n),SU(n)$ are connected. $O(n)$ is not, as it has two disconnected components, with each having $\det=\pm 1$.
The reason that $U(n)$ is connected while $O(n)$ is not, is because unitary matrices can have any $\mathbb{C}$ determinant with absolute value $1$, while orthogonal can only have $\pm 1$.

##### Simple connectedness
A space is **simply connected** if it is path connected, and every loop (path with same start and end points) can be shrunk continuously to a point.
###### Examples
$SO(2)$ is isomorphic to the circle group $S^1$, which is not simply connected.





### Subgroups
Every matrix Lie group is a subgroup of $GL(n,F)$ (by definition).
##### Identity component
Each matrix Lie group itself has a subgroup $G_{0}$ which is the identity component (the connected component which contains the identity element). In fact, $G_{0}$ is a normal subgroup.

If $G$ is connected, then $G_{0}=G$.
###### Proof:
Let $a,b \in G_{0}$. 

The inverse map is continuous, so $a^{-1}$ is in a connected subset (as connectedness is topological and hence preserved by continuous maps). This connected subset contains the identity, as it is its own inverse. So $a^{-1} \in G_{0}$.

The product map is continuous, so $ab$ is in a connected subset. This subset contains the identity, by considering $a=b^{-1}$. So $ab \in G_{0}$.

So $G_{0}$ is a subgroup (and it is closed, since a connected component is closed). 

Consider $g \in G$. The conjugate map $a\mapsto gag^{-1}$ is continuous, so is in a connected component. The set $gG_{0}g^{-1}$ contains the identity and is connected, so it is $G_{0}$. So $G_{0}$ is a normal subgroup.
###### Example
The group $O(n)$ is disconnected, with the connected identity component being $SO(n)$.

