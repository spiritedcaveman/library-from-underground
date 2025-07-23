
# 2.9.
Let $G$ be a finite group and $\Phi(G)$ the intersection of all maximal subgroups of $G$. Let $N$ be an abelian minimal normal subgroup of $G$. Then $N$ has a complement in $G$ if and only if $N \not\subseteq \Phi(G)$.

Solution:
Assume that $N$ has a complement $H$ in $G$. Then $G = NH$ and $N \cap H = 1$. Since $G$ is finite, there exists a maximal subgroup $M \ge H$. Then $N$ is not in $M$, which implies $N$ is not in $\Phi(G)$. Because, if $N \le M$, then $G = HN \le M$ which is a contradiction.

Conversely, assume that $N \not\subseteq \Phi(G)$. Then there exists a maximal subgroup $M$ of $G$ such that $N \not\subseteq M$. Then by maximality of $M$, we have $G = NM$. Since $N$ is abelian, $N$ normalizes $N \cap M$. Hence $G = NM \le N_G(N \cap M)$, i.e., $N \cap M$ is an abelian normal subgroup of $G$. But minimality of $N$ implies $N \cap M = 1$. Hence $M$ is a complement of $N$ in $G$.

---
## Definition: Every finite group G has a unique maximal normal nilpotent subgroup $\mathfrak{F}(G)$ (which is called the Fitting subgroup of G).



---

2.15. Consider the direct square $G \times G$ of $G$. Let $\hat{G} = \{(g, g) : g \in G\} \subseteq G \times G$.

(i) Show that $\hat{G}$ is a subgroup of $G \times G$ which is isomorphic to $G$. $\hat{G}$ is called the diagonal subgroup of $G \times G$.



notice that $G$ and $\hat{G}$ are different subgroups and co-exist in $G \times G$

(ii) Show also that $\hat{G} \unlhd G \times G$ if and only if $G$ is abelian.

for any $(g_1 , g_2) \in G$,
$(g1, g2 )^{-1} (x, x)(g_{1} , g_{2} ) = (g_{1}^-1 xg_{1} , g_{2}^-1 x g_{2} ) \in \hat{G}$

take $g_{1}=1$ so $x =g_{2}^-1xg_{2}$ and we are done


---

Suppose $H \trianglelefteq G$. Show that if $x, y$ elements in $G$ such that
$xy \in H$, then $yx \in H$.


just take the conjugation of $xy$ by $x$ or $y$ 

$x^{-1}(xy)x = y(xy)y^{-1} = yx$


If $H \unlhd G$, implies that every left coset is also a right coset.

$$Hx = xH, \quad yH = Hy, \quad xy \in H \text{ so } H = xyH.$$

$$xH = Hx \text{ implies } xyxH = xyHx = Hx.$$

Then $yxH = x^{-1} Hx = H$.

Hence $yx \in H$.
