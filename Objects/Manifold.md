## Definitions
### Definition: Manifold
A topological space $M$ is called a **manifold** of dimension $n$ if for every $x \in M$, there exists an open neighbourhood $x\in U \subset M$ and a homeomorphism $\alpha: U \to V \subset \mathbb{R}^n$. The pair $(U,\alpha)$ is called a **chart** at $x$.

### Definition: Transition map
Let $(U_{1}, \alpha_{1})$ and $(U_{2},\alpha_{2})$ be charts with non-empty intersection. The map $$
\alpha_{1} \circ \alpha_{2}^{-1}: \alpha_{2} (U_{2} \cap U_{1}) \to \alpha_{1} (U_{2} \cap U_{1})
$$is called a **transition map**. Notably it is a map on $\mathbb{R}^n$.

### Definition: Smooth manifold
A manifold is **smooth** if all transition maps are smooth, i.e. $C^\infty$, as maps on $\mathbb{R}^n$.
### Definition: Smooth maps on manifolds
A map $f: M \to N$ between smooth manifolds is called **smooth** if for each $x\in M$ with chart $(U,\alpha)$ and its corresponding $f(x)\in N$ with chart $(V,\beta)$, the map $\beta \circ f \circ \alpha ^{-1}$ is smooth, i.e. $C^\infty$.

## Submanifolds
A **submanifold** $S$ of $M$ is a subset of $M$ with the structure of a manifold. Often the inclusion (or submanifold) map $i: S \to M$ is taken to be an **immersion** (the derivative is everywhere injective) and also often to be everywhere injective itself.



## Properties
1. A manifold is path-connected if and only if it is connected.