intersection of all maximal ideal

If $(a)=R$, then $1\in (a)$. In particular, $ra=1$ for some $r\in R$, and thus $a$ is a unit.


the sum of an element of rad($R$) and a unit is a unit

If $a$ is not a unit then $aR$ is a proper right ideal of $R$, so there is a maximal right ideal $m$ with $aR \subset m$. But then $a \in m$, and $x \in J(R) \subset m$ since $J(R)$ is the intersection of all the maximal right ideals, so $u \in m$, but $u$ is a unit, which contradicts $m$ being a maximal ideal.

 $\mathfrak{a} \subset rad(R)$ if $1 − \mathfrak{a} ⊂ R^\times.$
 
 

Let $a \in \mathfrak{a}$. Then $1 - a \in R^\times$ by assumption.
Let $M$ be any maximal ideal of $R$. Since $1 - a$ is a unit, its image in $R/M$ is nonzero, so $a \notin M$ would imply $1 - a \equiv 1 \pmod{M}$ is a unit $\Rightarrow$ contradiction. Hence, $a \in M$.
Since $a$ lies in every maximal ideal, $a \in \operatorname{rad}(R)$.

Because $1 - \mathfrak{a} \subset R^\times$, so for $a \in \mathfrak{a}$, we have $1 - a \in R^\times$ directly.


 **Let $A$ be a ring, $n$ the set of non-units. Then $A$ is local if and only if $n$ is an ideal; if so, then $n$ is the maximal ideal.**

---

$\sqrt{ 0 } = \{0\}$ iff domain


- If $R$ is a domain: $x^n = 0 \Rightarrow x = 0$, so $\sqrt{0} = {0}$.
    
- If $\sqrt{0} = \{0\}$, then $xy = 0 \Rightarrow x = 0$ or $y = 0$; else $x \in \sqrt{0} \setminus {0}$.
---
If $a$ is an ideal and $m$ is a maximal ideal such that $a \not\subseteq m$, then:

$a + m = R$ (since $m$ is maximal and $a$ is an ideal not contained in $m$).
So $\exists a' \in a$, $m' \in m$ such that $a' + m' = 1$.
Then for any $r \in R$:
$r = r(a' + m') = ra' + rm'$.
Since $ra' \in a$ (because $a$ is an ideal) and $rm' \in m$ (because $m$ is an ideal), we have $r \in a + m$.
Thus,
$a+m=R$.

This is not a direct sum but an ideal sum: every element of $R$ is a sum of elements from $a$ and $m$.

---

If $M$ is a **maximal ideal** of a ring $R$, then the quotient $R/M$ is a **field**.

So if $x \notin M$, then $x + M \ne 0$ in $R/M$, hence:

That is, $x + M$ is a **unit** in the field $R/M$.

---
only idempotent in local rings $\{0,1\}$

---

If $m \in \mathfrak{m}$ (the maximal ideal of a local ring), and $1 + m$ is a unit, then so is $1 - m$.
Reason: In any ring, if $u$ is a unit, so is its inverse and any power. Also:
$$(1+m)(1-m+m^2-m^3+\cdots+(-1)^n m^n+\cdots)=1$$
if the series converges (e.g., if $m$ is nilpotent or topologically nilpotent).
But more generally, in a local ring, any element of the form $1 + x$ with $x \in \mathfrak{m}$ is a unit, so:
$$1+m \in R^\times \Rightarrow 1-m \in R^\times.$$
---
$$
\boxed{\text{Units can't be written as sum of non-units in a local ring}}.
$$
$$
\boxed{\text{Units can't be written as product of non-units in a local ring}}.
$$

$$
\boxed{\text{In any ring, a unit cannot be written as a product of non-units.}}
$$

Because $R^\times$ is a group ⇒ **closed under multiplication** ⇒ **complement is not**.

---
$\overline S=A-\bigcup_{\mathfrak m\in\operatorname{Max}(A);\ \mathfrak a\subseteq\mathfrak m}\mathfrak m$.
