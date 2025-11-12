Def
Properties: irred, faithful, direct sums
Schur's lemma
Adj rep

TODO TODOPAGE

## Definitions
### Via action
A **representation** of a group $G$ or associative algebra (or Lie algebra) $A$ on a vector space $V$ is a map $$
\Phi: G \times V \to V \qquad \text{or} \qquad \Phi: A \times V \to V
$$
For a given $g \in G$ (or $a \in A$), we write the action of $g$ on $v$ as $g \cdot v = \Phi(g,v)$.

Satisfying the following two properties:
1. For any $g \in G$ or $a \in A$, the following map is linear over $F$. $$
\begin{align}
\Phi(g): V & \to V  \\
v & \mapsto \Phi(g,v)
\end{align}
$$
2. The identity (if it exists) acts identically, $e \cdot v = v$.

3. Let $g_{1},g_{2}\in G$ and $v \in V$.
	1. For a group or algebra, we have associativity $g_{1} \cdot (g_{2} \cdot v)=(g_{1}g_{2}) \cdot v$.
	2. For a Lie algebra, we have $x_{1} \cdot (x_{2} \cdot v) - x_{2} \cdot (x_{1} \cdot v) = [x_{1}, x_{2}] \cdot v$.

### Via mapping
A **representation** is a map sending an element $g$ of an algebraic object (group, algebra, etc) to a linear map $\Phi(g): V \to V$, which satisfies $\Phi(g_{1} g_{2})=\Phi(g_{1}) \circ \Phi(g_{2})$ for all $g_{1}, g_{2} \in G$.

From this perspective:
- A representation of a group $G$ on a vector space $V$ is a group homomorphism $\Phi: G \to GL(V)$
- A representation of an associative algebra is an algebra homomorphism $\Phi: A \to\text{End}(V)$
- A representation of a Lie algebra is a [[Lie algebra|Lie algebra homomorphism]] $\Phi: \mathfrak{g} \to \mathfrak{gl}(V)$

## Terminology
### Faithful
A **faithful representation** is one where the homomorphism is injective.