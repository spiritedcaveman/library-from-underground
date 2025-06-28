2.10. If $G$ is a finite group and $K \le H \le G$, then
$[G:K] = [G:H][H:K]$.

The surjection $\overline{\pi}: G/K \to G/H$ has fibers of size $|H/K|$, given by $\overline{\pi}^{-1}(aH) = a(H/K)$. Since each fiber has the same cardinality as $H/K$ we get $$[G:K] = [G:H][H:K]$$

---

# 2.11.
Let $a \in G$ have order $n = mk$, where $m, k \ge 1$. Prove that $a^k$ has order $m$.

$$(a^k)^m = a^{km} = e$$
so the order of $a^k$ divides $m$. If $(a^k)^r = e$ for some $r$, then $a^{kr} = e$, implying $n$ divides $kr$. Since $n = mk$, we get $mk \mid kr$, so $m \mid r$. Thus, $a^k$ has order exactly $m$.

---
# 2.12.
(i) Prove that every group $G$ of order $4$ is isomorphic to either $\mathbb{Z}_4$ or the 4-group $V$.

If $G$ is cyclic, then $G \cong \mathbb{Z}_4$. Otherwise, pick any two elements $a, b \neq e$. Since $|G| = 4$, their orders must be $2$ (otherwise, $G$ would be cyclic). Thus, $a^2 = b^2 = e$. Consider $ab$; if $ab \neq a, b, e$, then $G$ is cyclic, a contradiction. So, $ab$ must be another element of order $2$, forcing $G$ to be isomorphic to the Klein four-group $V_4 = \{e, a, b, ab\}$ with $ab = ba$.

(ii) If $G$ is a group with $|G| \le 5$, then $G$ is abelian.

From $ab=ba^2$ and $a^2b=ba$ you get $a^2ba=ba^2=ab$, hence $aba=b$.  The identifications 

$$\{a,b,c,d,e\}=\{a,b,ab,ba,e\}=G=aG=\{a^2,ab,a^2b,aba,a\}=\{a^2,c,d,aba,a\}=\{a^2,c,d,b,a\}$$

now tell us $a^2=e$.  But then $d=a^2b=eb=b$, a contradiction.

---
# 2.13.
If $a \in G$ has order $n$ and $k$ is an integer with $a^k = 1$, then $n$ divides $k$. Indeed, $\{k \in \mathbb{Z}: a^k = 1\}$ consists of all the multiples of $n$.

Let $a$ have order $n$, so $a^n = 1$. Applying $f$, we get $f(a^n) = f(1) = 1$, which simplifies to $f(a)^n = 1$. Hence, the order of $f(a)$ divides $n$.

---
# 2.14.
If $a \in G$ has finite order and $f: G \to H$ is a homomorphism, then the order of $f(a)$ divides the order of $a$.

Let $a$ have order $n$, so $a^n = 1$. Applying $f$, we get $f(a^n) = f(1) = 1$, which simplifies to $f(a)^n = 1$. Hence, the order of $f(a)$ divides $n$.

---
# 2.15.
Prove that a group $G$ of even order has an odd number of elements of order 2 (in particular, it has at least one such element). (Hint. If $a \in G$ does not have order 2, then $a \ne a^{-1}$.)

Elements not of order 2 pair as $(a, a^{-1})$, leaving the identity and elements of order 2 unpaired.

Since $|G|$ is even, the number of these unpaired elements must be odd to add up with the identity and even numbers of order 2 elements, ensuring at least one element of order 2.
 
 ---
# 2.16.
If $H \le G$ has index 2, then $a^2 \in H$ for every $a \in G$.

The cosets of $H$ in $G$ are $H$ and $G \setminus H$. If $a \notin H$, then $aH = G \setminus H$, so for any $b \in H$, we have $ab \notin H$, meaning $H$ is normal. 

Now $aH$ has order $2$ in $G/H$, so, $aH \cdot aH = H$, we get $a^2 \in H$ for all $a \in G$.

---
# 2.17.
(i) If $a, b \in G$ commute and if $a^m = 1 = b^n$, then $(ab)^k = 1$, where $k = \operatorname{lcm}(m, n)$. (The order of $ab$ may be smaller than $k$; for example, take $b = a^{-1}$.) Conclude that if $a$ and $b$ commute and have finite order, then $ab$ also has finite order.

Given $(ab)^k = 1$, we deduce $a^k = b^{-k}$, meaning $c = a^k = b^{-k}$ lies in $\langle a \rangle \cap \langle b \rangle$. Since $a$ and $b$ have coprime orders $m, n$, we get $\operatorname{ord}(c) \mid \gcd(m, n) = 1$, forcing $c = 1$, so $a^k = 1 = b^k$. Thus, $m, n \mid k$, implying $\operatorname{lcm}(m, n) \mid k$. Conversely, if $m, n \mid \ell$, then $(ab)^\ell = 1$, proving $\operatorname{ord}(ab) = \operatorname{lcm}(m, n)$.

---
(ii) Let $G = \operatorname{GL}(2, \mathbb{Q})$ and let $A, B \in G$ be given by
$$ A = \begin{bmatrix} 0 & 1 \\ -1 & 0 \end{bmatrix} \quad \text{and} \quad B = \begin{bmatrix} 0 & -1 \\ 1 & 0 \end{bmatrix}.$$
  Show that $A^4 = E = B^3$, but that $AB$ has infinite order.
  
  We compute:
$$A^2 = \begin{bmatrix} -1 & 0 \\ 0 & -1 \end{bmatrix}, \quad A^4 = E$$
For $B$:
$$B^2 = \begin{bmatrix} -1 & -1 \\ 1 & 0 \end{bmatrix}, \quad B^3 = E$$
Thus, $A^4 = E = B^3$.
Now, compute $AB$:
$$AB = \begin{bmatrix} 1 & 1 \\ -1 & 0 \end{bmatrix}$$
Since $AB$ has an eigenvalue $\frac{1+\sqrt{5}}{2}$ (irrational), its powers never return to $E$, so $AB$ has infinite order.

---
  
# 2.18.
Prove that every subgroup of a cyclic group is cyclic. (Hint. Use the division algorithm.)

Let $G = \langle a \rangle$ be cyclic, and let $H \leq G$. If $H = \{e\}$, it is cyclic. Otherwise, let $d$ be the smallest positive integer such that $a^d \in H$. Then $H = \langle a^d \rangle$, since any $a^k \in H$ can be written as $a^k = (a^d)^m a^r$ where $0\leq r < d$ by the division algorithm. Since $a^k, (a^d)^m \in H$, $a^r\in H$. By minimality of $d$, $r=0$. Hence, $a^k = (a^d)^m$, so $H$ is cyclic.

---
# 2.19. Prove that two cyclic groups are isomorphic if and only if they have the same order.

Define $\varphi: \langle a \rangle \rightarrow \langle b \rangle$ by $\varphi(a^n) = b^n$. This is well-defined since any element in a cyclic group is of the form $a^n$. It is a homomorphism because
$$\varphi(a^m a^n) = \varphi(a^{m+n}) = b^{m+n} = b^m b^n = \varphi(a^m) \varphi(a^n)$$  
If $|a| = |b| = k$, then $a^k = e$ implies $b^k = e$, ensuring $\varphi$ is well-defined and bijective. Hence, the groups are isomorphic. Conversely, if two cyclic groups are isomorphic, their generators must have the same order, so they have the same order.

---

## Definition.
The Euler $\varphi$-function is defined as follows:
$\varphi(1) = 1; \quad \text{if } n > 1, \text{ then } \varphi(n) = |\{k: 1 \le k < n \text{ and } (k, n) = 1\}|.$

2.20. If $G = \langle a \rangle$ is cyclic of order $n$, then $a^k$ is also a generator of $G$ if and only if $(k, n) = 1$. Conclude that the number of generators of $G$ is $\varphi(n)$.

If $a^k$ is a generator, then $\langle a^k \rangle = G$, meaning $a^k$ has order $n$, which requires $k$ to be coprime to $n$, i.e., $(k, n) = 1$. Conversely, if $(k, n) = 1$, then the order of $a^k$ is
$\frac{n}{\gcd(k, n)} = n$,
so $a^k$ generates $G$. The number of such $k$ is precisely $\varphi(n)$.

---
# 2.21.
(i) Let $G = \langle a \rangle$ have order $rs$, where $(r, s) = 1$. Show that there are unique $b, c \in G$ with $b$ of order $r, c$ of order $s$, and $a = bc$.

(ii) Use part (i) to prove that if $(r, s) = 1$, then $\varphi(rs) = \varphi(r)\varphi(s)$.


# 2.22.
(i) If $p$ is prime, then $\varphi(p^k) = p^k - p^{k-1} = p^k(1 - 1/p)$.

(ii) If the distinct prime divisors of $n$ are $p_1, \dots, p_r$, then

$$ \varphi(n) = n(1 - 1/p_1)\cdots(1 - 1/p_r).$$

---
# 2.23 (Euler).

If $(r, s) = 1$, then $a^{\varphi(s)} \equiv 1 \pmod r$. (Hint. The order of the group of units $U(Z_n)$ is $\varphi(n)$.)