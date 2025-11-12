## Centraliser
### Definition
The **centraliser** of $S$ in an algebraic structure $A$ is the set of elements which commute with every element of a subset $S \subseteq A$. Equivalently for a group or ring, it is the set whose individual elements are fixed by conjugation.

#### Group, ring and algebra
$$
C_{G} (S) := \{ g \in G \; | \; gs = sg \quad \forall s\in S \} = \{ g\in G \;  | \; gsg^{-1}=s \quad \forall s \in S \}
$$
Replace $G$ with $R$ as needed for a ring or algebra $R$. This is subgroup, subring, subalgebra.
#### Lie algebra
In a Lie algebra, the centraliser is formulated in terms of the Lie bracket.
$$
C_{\mathfrak{g}} (S) := \{ x \in \mathfrak{g} \;  | \; [x,s] = 0 \quad \forall s \in S \}
$$
This is a Lie [[Lie algebra|subalgebra]] of $\mathfrak{g}$.
### Relation to centre 
The **centre** of an algebraic structure is the set of elements which commute with everything. $$
C_{G} (G) = \{ g \in G \;  | \; gh = hg \quad \forall h \in G \} =: Z(G)
$$It is a normal subgroup, and an ideal for the ring or algebra. For a Lie algebra, it's a Lie ideal.



## Normaliser
### Definition
The **normaliser** of a subset $S \subseteq A$ of an algebraic structure is the set which is fixed under conjugation, though the individual elements themselves may not be fixed. It is a weaker condition than the centraliser.
#### Group
$$
N_{G} (S) := \{ g \in G \;  | \; gS = Sg \} = \{ g \in G \;  | \; gSg^{-1} = S \}
$$
If in particular $S$ is a subgroup of $G$, then $N_{G} (S)$ is the largest subgroup of $G$ such that $S$ is a normal subgroup of $N_{G} (S)$.

#### Lie algebra
Again we use the Lie bracket instead of conjugation.
$$
N_{\mathfrak{g}} (S) := \{ x \in \mathfrak{g} \;  | \; [x,s] \in S \quad \forall s \in S \} = \{ x \in G \;  | \; [x,S] \subseteq S \}
$$

