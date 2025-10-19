

## Lie's three theorems
Let $G,H$ be Lie groups with corresponding algebras $\mathfrak{g}, \mathfrak{h}$.

### Lie's first theorem
If $G \cong H$, then $\mathfrak{g} \cong \mathfrak{h}$.
More generally, if $\Phi: G \to H$ is a homomorphism of Lie groups, then there is an associated map $\phi:\mathfrak{g} \to \mathfrak{h}$ that is a homomorphism of Lie algebras.


#### Proof (matrix Lie groups)
For $X \in \mathfrak{g}$, let $t \mapsto \exp(tX)$ be its [[One-parameter subgroup|one-parameter subgroup]]. 
Then due to the homomorphism $\Phi$, the associated one-parameter subgroup of $H$ is $\Phi(\exp(tX))$. This corresponds to a unique matrix $Y \in \mathfrak{h}$. 
Define a map $\phi: \mathfrak{g} \to \mathfrak{h}$ with $\phi(X)=Y$. This is a homomorphism of algebras.


### Lie's second theorem
If $\mathfrak{g} \cong \mathfrak{h}$, then $G$ and $H$ are locally isomorphic (there exists an isomorphism between neighbourhoods).

#### Proof (matrix Lie groups)
Let $\phi:\mathfrak{g} \to \mathfrak{h}$ be a Lie algebra homomorphism, with $0 \in U \subset \mathfrak{g}$ and $I \in V \subset G$ such that $\exp(U)=V$ (i.e. the neighbourhoods where there is a local homeomorphism via $\exp$).

We claim $\Phi:G \to H$ defined by $\Phi(e^X)=e^{\phi(X)}$ is a Lie group homomorphism.

To see this, note (via [[Baker-Campbell-Hausdorff formula|BCH]]) that the Lie algebra homomorphism $\phi$ satisfies $$
\begin{align}
\phi(\log(e^X e^Y)) &= \phi\left( X+Y+\frac{1}{2} [X,Y] +\dots \right) \\
&=\phi(X)+\phi(Y)+\frac{1}{2} [\phi(X), \phi(Y)]+\dots \\
&= \log(e^{\phi(X)} e^{\phi(Y)})
\end{align}
$$
So $$
\Phi(e^X e^Y)=\Phi(e^{\log(e^X e^Y)})=e^{\log(e^{\phi(X)} e^{\phi(Y)})}=e^{\phi(X)} e^{\phi(Y)}=\Phi(e^X) \Phi(e^Y)
$$


### Lie's third theorem