### Definition 1
Consider $\mathfrak{g}$ the Lie algebra of $G$, in particular thinking of $\mathfrak{g}$ as the tangent space to $1_{G} \in G$.

#### Exponential
The **exponential map** is a map $\exp: \mathfrak{g} \to G$ such that $\exp(X) = \gamma (1_{G})$, where $\gamma:\mathbb{R} \to G$ is the unique [[one-parameter subgroup]] of $G$ whose tangent vector at $1_G$ is $X$.
##### Properties
###### Smoothness
Clearly the map is smooth, because it is an integral curve.
###### Operations
- $\exp((t+s)X)=\exp(tX)\exp(sX)$
- $\exp(-X)=\exp(X)^{-1}$
- Generally, if $[X,Y]=0$, then the [[Baker-Campbell-Hausdorff formula|BCH formula]] gives $\exp(X+Y)=\exp(X)\exp(Y)$.
- Since it is smooth (hence continuous), the image of $\exp$ is contained in the identity component of $G$.
###### Behaviour at zero
$\exp(0_{\mathfrak{g}})=1_{G}$, since the one-parameter subgroup with tangent $0$ at $1_{G}$ is the constant map. Due to smoothness and the inverse function theorem, $\exp$ restricts to a local diffeomorphism near $0_{\mathfrak{g}}$ to a neighbourhood of $1_{G}$.
###### Product of exponentials
If there is a path from $1_{G}$ to some $g \in G$ (i.e. $g$ is in the identity component), then $g$ can be written as a finite product $g=\exp(X_{1})\dots \exp(X_{k})$ for $X_{i} \in \mathfrak{g}$. Further, if $G$ is connected (hence path connected due to manifold structure), then every $g$ can be written this way.
	Proof: [MSE](https://math.stackexchange.com/questions/5101778/lie-group-element-as-finite-product-of-exponentials) 

###### Derivative and differential
For a curve $X(t)$, the derivative is
$$
\frac{d}{dt} \exp^{X(t)}=e^{X(t)} \frac{{1-e^{-\text{ad}_{X}}}}{\text{ad}_{X}} \frac{dX(t)}{dt}
$$
Where $\text{ad}_{X}$ is treated as an operator, so we have the power series
$$
\frac{1-e^{-\text{ad}_{X}}}{\text{ad}_{X}}=\sum_{k=0}^\infty \frac{(-1)^k}{(k+1)!} (\text{ad}_{X})^k
$$


#### Logarithm
Since $\exp$ is smooth and $d\exp(X)|_{0}=\text{id}_{\mathfrak{g}}$, the inverse function theorem says $\exp$ restricts to a diffeomorphism from a neighbourhood $V \subseteq \mathfrak{g}$ of $0_{\mathfrak{g}}$ to a neighbourhood $U \subseteq G$ of $1_{G}$. The (local) inverse map $\log: U \to V$ is the **logarithm map**.



### Definition 2
For a matrix Lie group, the **exponential map** coincides with the matrix exponential, given by the series expansion
$$
\exp(X) := \sum_{k=0}^\infty \frac{X^k}{k!} = I + X + \frac{1}{2} X^2 + \frac{1}{6} X^3 + \dots
$$
That is, the exponential map is the restriction of the matrix exponential to $\mathfrak{g}$.

### Definition 3

##### Exponent via ring of power series
The **exponent map**, defined via [[Formal power series|formal power series]], is 
$$
\exp(t)=\sum_{n=0}^\infty \frac{t^n}{n!} \in \mathbb{Q}[[t]]
$$


### Examples
1. For $G=\mathbb{R}^{\times}_{>0}$ and $\mathfrak{g}=\mathbb{R}^+$, the Lie exponential is the usual exponential function $e^x$.
2. For $G=S^1$ the [[Circle group|circle group]], the one-parameter subgroup is $\gamma(t)=e^{it}$, so the Lie exponential coincides with the complex exponential.

