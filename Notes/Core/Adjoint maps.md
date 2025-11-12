**define ad. show ad is derivation, justify ad=dAd**

There are two adjoint maps: $\text{Ad}: G \to \text{Aut}(\mathfrak{g})$ (the adjoint representation of $G$) and $\text{ad}: \mathfrak{g} \to \mathfrak{g}$ (the adjoint representation of $\mathfrak{g}$).
### Adjoint representation of group
Let $G$ be a Lie group. Define a Lie group homomorphism$$
\begin{align}
\text{Ad}_{g}: \mathfrak{g}& \to \mathfrak{g} \\
X & \mapsto gXg^{-1}
\end{align}
$$This is the adjoint map at $g \in G$, which is an automorphism of the Lie algebra $\mathfrak{g}$. 

*Justification*
	Conjugation is linear, so $\text{Ad}_{g}$ is linear. Also, $\exp(t(gXg^{-1}))=g \exp(tX)g^{-1} \in G$, so the map actually goes to $\mathfrak{g}$.
	Also, $gXYg^{-1}=(gXg^{-1})(gYg^{-1})$, so $\text{Ad}_{g}([X,Y])=[\text{Ad}_{g}(X), \text{Ad}_{g} (Y)]$, so it's a Lie algebra homomorphism.
	Also, $\text{Ad}_{gh}=\text{Ad}_{g} \circ \text{Ad}_{h}$ and $(\text{Ad}_{g})^{-1}=\text{Ad}_{g^{-1}}$.
	Furthermore, it is smooth because matrix operations are smooth. And $\mathfrak{g}$ is a vector space over $F$, which *..TODO....* means that it's a Lie group homomorphism.

These comprise the group homomorphism $$
\begin{align}
\text{Ad}: G & \to \text{Aut}(\mathfrak{g}) \\
g & \mapsto \text{Ad}_{g}
\end{align}
$$
In fact, this is a [[Representations|representation]], called the **adjoint representation of the group** $G$.

#### Properties
Conjugation is linear, so $\text{Ad}_{g}$ is linear. Also, $\exp(t(gXg^{-1}))=g \exp(tX)g^{-1} \in G$, so *TODO?*

### Adjoint representation of algebra

Taking the derivative of $\text{Ad}: G \to \text{Aut}(\mathfrak{g})$ at the identity

#### Adjoint action
The **adjoint action** of $\mathfrak{g}$ on itself is $$
\begin{align}
\text{ad}: \mathfrak{g \times g} & \to \mathfrak{g} \\
\text{ad}_{x}: y & \mapsto [x,y] 
\end{align}
$$
The action on a subalgebra $\mathfrak{h}$ of $\mathfrak{g}$ is the restriction: $$
\text{ad}|_{\mathfrak{h}}
$$



Let $\mathfrak{h}$ act on $\mathfrak{g}$ by the [[Adjoint maps|adjoint action]] $\text{ad}: \mathfrak{g \times g \to g}$, $\text{ad}_{x}: y \mapsto [x,y]$, where to get the action of $\mathfrak{h}$ on $\mathfrak{g}$ we set $x \in \mathfrak{h}$, or equivalently, restrict the map with $\text{ad}|_{\mathfrak{h}}$. 