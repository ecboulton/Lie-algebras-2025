##### Ring of formal power series
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