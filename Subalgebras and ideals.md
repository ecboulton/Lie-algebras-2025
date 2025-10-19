## Subalgebras
### Definition
Given a Lie algebra $\mathfrak{g}$, a subspace $\mathfrak{a}$ is a **Lie subalgebra** if it is closed under the Lie bracket. That is, $[A,B] \in \mathfrak{a}$ whenever $A,B \in \mathfrak{a}$.

### Examples
The subspace $\mathfrak{sl}(n,F) \subset \mathfrak{gl}(n,F)$ is the subspace in $M(n,F)$ of traceless matrices. Any product and sum of traceless matrices is traceless, so the Lie bracket preserves tracelessness. So $\mathfrak{sl}(n,F)$ is a subalgebra of $\mathfrak{gl}(n,F)$.

The Lie algebras $\mathfrak{o}(n), \mathfrak{so}(n), \mathfrak{u}(n), \mathfrak{su}(n)$ are defined over $\mathbb{R}$ and $\mathbb{C}$ respectively, so they are subalgebras of $\mathfrak{gl}(n,F)$ by Ado's theorem.

### Ado's theorem
In fact, when $\text{char}(F)=0$, every finite dimensional Lie algebra is a subalgebra of $\mathfrak{gl}(n,F)$.
This theorem is useful to prove Lie's product formula