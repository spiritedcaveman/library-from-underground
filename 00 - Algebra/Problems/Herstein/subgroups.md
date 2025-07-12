If G is a group and $x,a \in G$, prove that $C_G(x^{-1}ax)=x^{-1}C_G(a)x$ where $C_G$ is the centralizer.

I believe we have to do this by showing that $C_G(x^{-1}ax) \subset x^{-1}C_G(a)x$ and vice versa. 

So, let $g \in C_G(x^{-1}ax)$,  

then $$gx^{-1}axg^{-1} = x^{-1}ax$$

$$gx^{-1}ax = x^{-1}axg$$
$$x^{-1}ax = g^{-1}x^{-1}axg$$
$$a = xg^{-1}x^{-1}axgx^{-1}$$

So $$xgx^{-1} \in C_G(a)$$
And, $$x^{-1}C_G(a)x = g$$

The other inclusion is just reverse of the argument. 

---
$AB $ is a subgroup because $G$ is abelian. We know that $$|AB| = \frac{|A| \cdot |B|}{|A \cap B|}$$
But if $\gcd(m,n) = 1$ then $|A \cap B| = 1 $ because $|A \cap B| \mid |A| = m$ and $|A \cap B| \mid |B| = n$ by Lagrange theorem. So $$|AB| = |A| \cdot |B| = mn$$

---
Let $N = \bigcap_{x \in G} x^{-1} H x$.

Each $x^{-1} H x$ is a subgroup (a conjugate of $H$), so their intersection $N$ is a subgroup.

For any $y \in G$ and $n \in N$, we have $n \in x^{-1} H x$ for all $x$, so

$$y^{-1} n y \in (y^{-1} x^{-1}) H (x y) = (xy)^{-1} H (xy),$$

which means $y^{-1} n y \in N$. Hence $y^{-1} N y \subseteq N$, and similarly $N \subseteq y^{-1} N y$, so $y^{-1} N y = N$.

Thus, $N$ is normal in $G$.

---
Let $a, b \in N$, we need to prove that: $ab^{-1} \in N$. First we prove that $x^{-1}Hx$ is a subgroup of $G$ for any $x \in G$. For if $s, t \in x^{-1}Hx$, then $s = x^{-1}yx$, and $t = x^{-1}zx$ for some $y, z \in H$. So $st^{-1} = x^{-1}yxx^{-1}z^{-1}x = x^{-1}yz^{-1}x$. Since $y, z \in H$ and $H$ is a subgroup, we have: $yz^{-1} \in H$. So $x^{-1}yz^{-1}x \in x^{-1}Hx$. Thus: $st^{-1} \in x^{-1}Hx$, and $x^{-1}Hx$ is a subgroup of $G$. Now $a, b \in N$, so $a \in x^{-1}Hx$, and $b \in x^{-1}Hx$ for all $x \in G$. Since we just proved that $x^{-1}Hx$ is a subgroup of $G$, that means $ab^{-1} \in x^{-1}Hx$ for all $x \in G$. So $ab^{-1} \in \displaystyle \bigcap_{x \in G}x^{-1}Hx = N$, proving that $N$ is a subgroup of $G$. And for any $y \in G$, we have:
$y^{-1}Ny = \displaystyle \bigcap_{x \in G}y^{-1}x^{-1}Hxy = \displaystyle \bigcap_{x \in G}(xy)^{-1}Hxy = \displaystyle \bigcap_{z \in G}z^{-1}Hz = N$. We're done.

---

Suppose $Ha \cap Hb \ne \emptyset$. Then $\exists, h_1, h_2 \in H$ such that $h_1 a = h_2 b \Rightarrow a = h_1^{-1} h_2 b$.

Let $h = h_1^{-1} h_2 \in H$, so $a = h b \Rightarrow Ha = H(hb) = (Hh)b = Hb$ since $Hh = H$.

Hence, either $Ha = Hb$ or $Ha \cap Hb = \emptyset$.

---
Let $H$ be a finite subgroup of $G$ and fix $a \in G$. Define the left coset $Ha = {ha : h \in H}$.

Define $f: H \to Ha$ by $f(h) = ha$. This map is **injective**: if $ha = h'a$, then $h = h'$. (Multiply both sides on the right by $a^{-1}$.)

Since $H$ is finite and $f$ is injective, $f$ is bijective. So $|Ha| = |H|$.

This holds for every $a \in G$, so all cosets $Ha$, $Hb$ have the same number of elements:

$$
∣Ha∣=∣Hb∣=∣H∣.|Ha| = |Hb| = |H|.
$$
----
Since $x^{-1} M x \subseteq M$ and $x^{-1} N x \subseteq N$ for all $x \in G$, both $M$ and $N$ are normalized by $G$ (not necessarily normal).

To show $MN$ is a subgroup:

  

Take $m_1 n_1, m_2 n_2 \in MN$ with $m_i \in M$, $n_i \in N$. Then:

$$(m_1 n_1)(m_2 n_2) = m_1 (n_1 m_2 n_1^{-1}) (n_1 n_2).$$Since $x^{-1} M x \subseteq M$, $n_1 m_2 n_1^{-1} \in M$. So the product lies in $MN$.

Also, inverses: $(mn)^{-1} = n^{-1} m^{-1} = (n^{-1} m^{-1} n) n^{-1} \in MN$ since $n^{-1} m^{-1} n \in M$. So $MN$ is a subgroup.

Now for conjugation:

  

Let $x \in G$, then for any $m \in M$, $n \in N$, we have

$$x^{-1} (mn) x = (x^{-1} m x)(x^{-1} n x) \in MN,$$

since $x^{-1} M x \subseteq M$ and $x^{-1} N x \subseteq N$.

So $x^{-1} (MN) x \subseteq MN$.

---

Define the map $\varphi_x: G \to G$ by $\varphi_x(g) = x^{-1}gx$. This is conjugation by $x^{-1}$, and it's an automorphism of $G$. Now suppose $x^{-1} M x \subseteq M$ for all $x \in G$.

Then for each $x \in G$, $\varphi_x(M) \subseteq M$.

But $\varphi_x$ is a bijection (since conjugation is an automorphism), so $\varphi_x(M)$ and $M$ have the same cardinality.

Hence, $\varphi_x(M) \subseteq M$ and $|\varphi_x(M)| = |M|$ implies:

$$\varphi_x(M) = M \quad \text{or} \quad x^{-1} M x = M.$$So $M$ is normal in $G$.

**Summary: injective + same size $\Rightarrow$ equality.**

---

Let $m \in M$, $n \in N$. Consider the commutator:

$$[m,n]=m^{-1}n^{-1}mn.$$We want to show $[m, n] = e$, i.e., $mn = nm$.

Since $x^{-1} M x = M$ and $x^{-1} N x = N$ for all $x \in G$, both $M$ and $N$ are normal in $G$. So:

  

$n^{-1} m n \in M \Rightarrow m^{-1} n^{-1} m n \in M$,

$m^{-1} n m \in N \Rightarrow m^{-1} n^{-1} m n \in N$.

So $[m, n] \in M \cap N = \{e\}$.

Therefore, $m^{-1} n^{-1} m n = e \Rightarrow mn = nm$.

---
