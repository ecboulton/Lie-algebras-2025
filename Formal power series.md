## Definition
The **ring of power series** is 
$$
\mathbb{Q}[[t]]=\left\{  \sum_{n=0}^\infty a_{n} t^n \; | \; a_{n}\in \mathbb{Q}  \right\}
$$
where the ring operations are
$$
\begin{align}
\left( \sum a_{n} t^n \right)+\left( \sum b_{n}t^n \right)&= \sum(a_{n}+b_{n}) t^n \\ \\
\left( \sum a_{n} t^n \right) \left( \sum b_{n}t^n \right)&= \sum_{n=0}^\infty \left( \sum_{k=0} a_{k} b_{n-k} \right) t^n
\end{align}
$$
Note for formal power series, we don't care about convergence in order to define them (there may not even be an underlying topological space in general).

### Notation
The ring of formal power series in two variables is $\mathbb{Q}[[s,t]]$ when $s$ and $t$ commute, and $\mathbb{Q} \langle \langle s,t \rangle \rangle$ if they don't commute.

## Ideals
The ring $\mathbb{Q}[[t]]$ has an ideal $t\mathbb{Q}[[t]]$, which is the truncation to terms of degree $1$ and higher. Similarly, there are ideals $t^k \mathbb{Q}[[t]]$ which truncate to terms of degree $k$ and higher.

## Composition of series
Let $f(t)=\sum_{n=0}^\infty a_{n} t^n \in \mathbb{Q}[[t]]$ and $g(t)=\sum_{n=1}^\infty b_{n} t^n \in t\mathbb{Q}[[t]]$. Then the substitution $(f \circ g)(t)$ is $$
(f \circ g)(t)=\sum_{n=0}^\infty a_{n} (g(t))^n=\sum_{n=0}^\infty a_{n} (b_{1} t + b_{2} t^2 + \dots)^n =: \sum_{n=0}^\infty c_{n} t^n
$$
Here, $c_{n}:=\sum_{k\in \mathbb{N}, |j|=n} b_{k} a_{j_{1}} \dots a_{j_{k}}$, as a sum over both $j,k$.

Since $g$ has no constant term, we get $k \leq n$ and for each $i$, $j_{i} \le n$. Then the sum defining $c_{n}$ is finite and rational. *Note: this requires that $g$ have no constant term!*
