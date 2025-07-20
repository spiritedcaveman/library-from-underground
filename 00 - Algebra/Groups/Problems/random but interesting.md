
# 2.9.
Let $G$ be a finite group and $\Phi(G)$ the intersection of all maximal subgroups of $G$. Let $N$ be an abelian minimal normal subgroup of $G$. Then $N$ has a complement in $G$ if and only if $N \not\subseteq \Phi(G)$.

Solution:
Assume that $N$ has a complement $H$ in $G$. Then $G = NH$ and $N \cap H = 1$. Since $G$ is finite, there exists a maximal subgroup $M \ge H$. Then $N$ is not in $M$, which implies $N$ is not in $\Phi(G)$. Because, if $N \le M$, then $G = HN \le M$ which is a contradiction.

Conversely, assume that $N \not\subseteq \Phi(G)$. Then there exists a maximal subgroup $M$ of $G$ such that $N \not\subseteq M$. Then by maximality of $M$, we have $G = NM$. Since $N$ is abelian, $N$ normalizes $N \cap M$. Hence $G = NM \le N_G(N \cap M)$, i.e., $N \cap M$ is an abelian normal subgroup of $G$. But minimality of $N$ implies $N \cap M = 1$. Hence $M$ is a complement of $N$ in $G$.

---
## Definition: Every finite group G has a unique maximal normal nilpotent subgroup $\mathfrak{F}(G)$ (which is called the Fitting subgroup of G).
