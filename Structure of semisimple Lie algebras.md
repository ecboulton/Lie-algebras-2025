*Not assessed for exam. Lecture 13th Oct* 

$\mathfrak{h} < \mathfrak{g}$
$\mathfrak{h}$ is Cartan, abelian, semisimple, consists of semisimple elements.
So there is simultaneous diagonalisation of any space it acts on.

Then there are functionals $\alpha: \mathfrak{h} \to \mathbb{C}$

$\mathfrak{g}=\mathfrak{h}\oplus(\bigoplus_{\alpha \in \Phi} \mathfrak{g}_{\alpha})$
here, $\mathfrak{h}=\mathfrak{g}_{0}$
$$
[\mathfrak{g}_{\alpha}, \mathfrak{g}_{\beta}] \subseteq \mathfrak{g}_{\alpha+\beta}
$$

**Properties**
1. Orthogonality -- every space is orthogonal (except $\mathfrak{g}_{\alpha}$ and $\mathfrak{g}_{-\alpha}$)
2. $\Phi$ spans $\mathfrak{h}^*$
3. $\alpha\in \Phi \implies -\alpha \in \Phi$
4. $x \in \mathfrak{g}_{\alpha}$, there exists $y_{\alpha} \in \mathfrak{g}_{\alpha}$ such that $[x,y]=k(x,y) t_{\alpha}$
5. $k(t_{\alpha}, \cdot) = \alpha(\cdot)$
6. $\alpha(t_{\alpha}) = k(t_{\alpha}, t_{\alpha}) \neq 0$
7. $0 \neq x \in \mathfrak{g}_{\alpha}$ there exists $y_{\alpha} \in \mathfrak{g}_{\alpha}$ such that $\text{span}_{\mathbb{C}} \{ x_{\alpha}, y_{\alpha}, h_{\alpha} := [x_{\alpha}, y_{\alpha}] \} \cong \mathfrak{sl}_{2} (\mathbb{C})$
8. $k_{\alpha} = \frac{2t_{\alpha}}{k(t_{\alpha}, t_{\alpha})}$
9. $\alpha(h_{\alpha}) = \alpha\left( \frac{2t_{\alpha}}{k(t_{\alpha}, t_{\alpha})} \right)=\frac{2}{k(t_{\alpha}, t_{\alpha})} k(t_{\alpha}, t_{\alpha})=2$


**Root system**
reduced <--(1:1)--> semisimple Lie alg
   U                                      U
irreducible <--(1:1)--> simple Lie alg



**Integrality**
1. $\text{dim} \mathfrak{g}_{\alpha} = 1$ for all $\alpha\in \Phi$
2. $\alpha\in \Phi \implies \mathbb{C}\alpha\cap \Phi=\{ \alpha,-\alpha \}$
3. $\alpha,\beta\in \Phi \implies \beta(\mathfrak{h}) \in \mathbb{Z}$ and $\beta-\beta(h_{\alpha})\alpha \in \Phi$
4. $\alpha,\beta, \alpha+\beta\in \Phi \implies [\mathfrak{g}_{\alpha}, \mathfrak{g}_{\beta}]=\mathfrak{g}_{\alpha+\beta}$ 
5. $\alpha,\beta \in \Phi, \beta\neq \pm\alpha$ then there exists $r,q\in \mathbb{Z}_{\geq_{0}}$ maximal such that $\beta-r\alpha, \beta+q\alpha, \beta+j\alpha \in \Phi$ for $-r\leq j\leq q$
6. $\mathfrak{g} = \langle \mathfrak{g}_{\alpha} \rangle$ as a Lie alg


**Proofs**
*1 and 2*
Pick $\alpha\in \Phi$. $\mathfrak{sl}_{2}(\mathbb{C}) \cong S_{\alpha}=\text{span}_{\mathbb{C}} \{ x_{\alpha}, y_{\alpha}, h_{\alpha} \}$ acts on $\mathfrak{g}$ by adjoint.

$\mathfrak{m}:=\mathfrak{h} \oplus (\bigoplus_{c \in \mathbb{C}^\times} \mathfrak{g}_{c\alpha})$
Claim: above is a submodule / subrepresentation of $\mathfrak{g}$ (as $S_{\alpha}$ module)
Proof: $[\mathfrak{g}_{\alpha},\mathfrak{g}_{\beta}] \subseteq \mathfrak{g}_{\alpha+\beta}$ so $[\mathfrak{g}_{\alpha}, \mathfrak{g}_{c\alpha}] \subseteq \mathfrak{g}_{(1+c)\alpha}$
Firstly, notice $S_{\alpha} \subseteq \mathfrak{m}$.

$x_{\alpha}$                        $h_{\alpha}$          $y_{\alpha}$

 .                                .                       .
				.    }
				.    }
				.    } $\text{ker} \alpha$
				.    }
				

$\alpha: \mathfrak{h} \to \mathbb{C}$
$\alpha(h_{\alpha})=2\neq 0$
$\mathfrak{h}=\text{ker}\alpha \oplus \mathbb{C} h_{\alpha}$

WTS no other multiples of $\alpha$ in the module. i.e. $\mathfrak{m}=\text{ker}\alpha \oplus S_{\alpha}$.
If there was another, it would have eigenvalue 0, but we have already listed all of them above.

So weights of $h_{\alpha}$ are $0,\pm 2$ and we also know that for $x\in\mathfrak{g}_{c\alpha}$,  $[h_{\alpha}, x]=c\alpha(h_{x}) \cdot x = c \cdot 2x$, so $c \in \frac{1}{2} \mathbb{Z}$ are the only possible weights. 
- so 4 is not a root (or any multiple of 2 besides $\pm 2$)

qed

*3*
$\mathfrak{u}:=\bigoplus_{j \in \mathbb{Z}} \mathfrak{g}_{\beta+j\alpha}$, sum of 1 dim as $\beta+j\alpha\neq 0$

Let $x\in \mathfrak{g}_{\beta+j\alpha}$
$h_{\alpha} \cdot x=(\beta+j\alpha)(h_{\alpha}) \cdot x = (\beta(h_{\alpha})+2j) x$
Notice $\beta(h_{\alpha})+2j$ is an integer (as it is a weight), so $\beta(h_{\alpha}) \in \mathbb{Z}$

Let $r,q$ maximal non-negative such that $\mathfrak{g}_{\beta-r\alpha}\neq 0$ and $\mathfrak{g}_{\beta+q\alpha}$.
$\beta(h_{\alpha})-2r$                                               $\beta(h_{\alpha})+2q$
$-m, \quad \qquad -m+2, \dots, m-2,\qquad m$

$\beta(h_{\alpha})-2r+\beta(h_{\alpha})+2q=0 \implies 2\beta(h_{\alpha})+2(q-r)=0 \implies  \beta(h_{\alpha})=r-q$

Q: do we know it's irreducible?
A: write down irreducible representations, either have weight 0 (even) or 1 (odd). in $\beta(h_{\alpha})+2j$, it either contains 0 or 1, and only one copy. so irreducible.





**Rationality**
$k_{\mathfrak{g}}|_{\mathfrak{h}}$ symmetric bilinear nondegenerate form on $\mathfrak{h}$
so we can transport it to $\mathfrak{h}^*$ via $h \mapsto k(h,\cdot)$
specifically $(x,y):=k(t_{x}, t_{y})$ is a symmetric bilinear nondegenerate form on $\mathfrak{h}^*$

$\Phi$ spans $\mathfrak{h}^*$, so choose $\alpha_1, \alpha_{2}, \dots, \alpha_{l} \in \Phi$ basis of $\mathfrak{h}^*$.
$\Phi \ni \beta=\sum_{i=1}^l c_{i} \alpha_{i}$ with $c_{i} \in \mathbb{C}$

Claim: $c_{i} \in \mathbb{Q}$.
Proof: 
	$(\beta,\alpha_{j})=\sum_{i=1}^l c_{i} (\alpha_{i}, \alpha_{j})$
	multiply by $\frac{2}{(\alpha_{j}, \alpha_{j})} \in \mathbb{Z}$
	so $\frac{2(\beta,\alpha_{i})}{(\alpha_{j}, \alpha_{j})} = \sum_{i=1}^l c_{i} \frac{2(\alpha_{i}, \alpha_{j})}{(\alpha_{j}, \alpha_{j})}$, this is linear system with integer (hence rational) coefficients
	so solution is rational. so $c_{i} \in \mathbb{Q}$.


Claim: $(\alpha,\beta) \in \mathbb{Q}$ when $\alpha,\beta\in \Phi$
Proof:
	WTS $(\lambda,\mu)=k(t_{\lambda}, t_{\mu})=\sum_{\alpha \in \Phi} \alpha(t_{\lambda}) \alpha(t_{\mu})=\sum_{\alpha \in \Phi}(\alpha,\lambda)(\alpha,\mu)$
	First equality
		$(\lambda, \mu)=\mathrm{Tr}(\text{ad}_{t_{\lambda}} \cdot \text{ad}_{t_{\mu}})=\mathrm{Tr}|_{\mathfrak{h}} (\text{ad}_{t_{\lambda}} \cdot \text{ad}_{t_{\mu}})+\sum \mathrm{Tr}|_{\mathfrak{g}_{\alpha}} (\text{ad}_{t_{\lambda}} \cdot \text{ad}_{t_{\mu}})=0+\sum \dots$
	If $\alpha,\beta \in \Phi$ then $(\beta,\beta)=\sum_{\alpha \in \Phi} (\alpha,\beta)^2$
	So $\frac{1}{(\beta,\beta)}=\sum_{\alpha} \frac{(\alpha,\beta)^2}{(\beta,\beta)}$
	Which is rational because $\frac{2(\alpha,\beta)}{(\beta,\beta)} \in \mathbb{Z}$
	So $(\alpha,\beta) \in \mathbb{Q}$



**Def:** $E_{\mathbb{Q}}:=\text{span}_{\mathbb{Q}} (\Phi) \subseteq \mathfrak{h}^*$ with symmetric nondegenerate bilinear form $(,):E_{\mathbb{Q}} \times E_{\mathbb{Q}} \to \mathbb{Q}$. Also it's positive definite because $(\lambda,\lambda)=\sum(\alpha,\lambda)^2 \geq 0$ . So it's an inner product.

Consider $E:=E_{\mathbb{Q}} \otimes \mathbb{R}$, has inner product $(,)$


 **Example**
 $h_{1}=\begin{pmatrix}1 && \\ &-1& \\ &&0\end{pmatrix}, h_{2}=\begin{pmatrix}0&&\\&1&\\&&-1\end{pmatrix}$
$h=\text{span} \{ h_{1}, h_{2} \}$ acts on $\mathfrak{sl}_{3} (\mathbb{C})=\mathfrak{h} \oplus \mathbb{C} \begin{pmatrix}0 & 1 & 0 \\ 0 & 0 & 0 \\ 0 & 0 & 0\end{pmatrix} \oplus \mathbb{C} \begin{pmatrix}0&0&0\\0&0&1\\0&0&0\end{pmatrix} \oplus \mathbb{C}\begin{pmatrix}0&0&1\\0&0&0\\0&0&0\end{pmatrix} \oplus \mathbb{C}\begin{pmatrix}\\1&0&0 \\ &\end{pmatrix}\oplus \mathbb{C}\begin{pmatrix}\\ \\ 0&1&0\end{pmatrix} \oplus \mathbb{C}\begin{pmatrix}\\ \\ 1&0&0\end{pmatrix}$ 
