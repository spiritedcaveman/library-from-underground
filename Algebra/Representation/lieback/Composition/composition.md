
notice we can form algebra with it, since the multiplication with the modlues is set for it is not some general ring but a nice group


Definition
The vector space $FG$, with multiplication defined by
$$\left( \sum_{g \in G} \lambda_g g \right) \left( \sum_{h \in G} \mu_h h \right) = \sum_{g, h \in G} \lambda_g \mu_h (gh)$$
$(\lambda_g, \mu_h \in F)$, is called the group algebra of $G$ over $F$.


the axioms for an algebra mean that it is both a vector space and a ring.

**6.4 Proposition**

Multiplication in $FG$ satisfies the following properties, for all $r, s, t \in FG$ and $\lambda \in F$:

(1) $rs \in FG$;
(2) $r(st) = (rs)t$;
(3) $r1 = 1r = r$;
(4) $(\lambda r)s = \lambda(rs) = r(\lambda s)$;
(5) $(r + s)t = rt + st$;
(6) $r(s + t) = rs + rt$;
(7) $r0 = 0r = 0$.


* $FG \times FG \to FG$ = inner (ring-wise)
  (algebra)
  
  ---
  
**6.10 Proposition**

Suppose that $V$ is an $FG$-module. Then the following properties hold for all $u, v \in V$, all $\lambda \in F$ and all $r, s \in FG$:

(1) $vr \in V$;
(2) $v(rs) = (vr)s$;
(3) $v1 = v$;
(4) $(\lambda v)r = \lambda(vr) = v(\lambda r)$;
(5) $(u + v)r = ur + vr$;
(6) $v(r + s) = vr + vs$;
(7) $v0 = 0r = 0$.




* $FG \times V \to V$ = external action (module-wise), 

---

**6.5 Definition**

Let $G$ be a finite group and $F$ be $\mathbb{R}$ or $\mathbb{C}$. The vector space $FG$, with the natural multiplication $vg$ ($v \in FG, g \in G$), is called the ==regular $FG$-module.==

The representation $g \rightarrow [g]_{\mathcal{B}}$ obtained by taking $\mathcal{B}$ to be the natural basis of $FG$ is called the **regular representation of $G$ over $F$**.

Note that the regular $FG$-module has dimension equal to $|G|$.