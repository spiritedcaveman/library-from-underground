31.
Let $G$ be the group of all nonzero real numbers under the operation $*$ which is the ordinary multiplication of real numbers, and let $H$ be the group of all real numbers under the operation $\#$, which is the addition of real numbers.
(a) Show that there is a mapping $F: G \to H$ of $G$ onto $H$ which satisfies $F(a * b) = F(a) \# F(b)$ for all $a, b \in G$ i.e., $F(ab) = F(a) + F(b)$].
(b) Show that no such mapping $F$ can be 1-1.



Let $F: G \to H$ be defined by $F(a) = \log |a|$. Then for all $a, b \in G = \mathbb{R}^\times$,

$F(ab)=log⁡∣ab∣=log⁡∣a∣+log⁡∣b∣=F(a)+F(b),F(ab) = \log |ab| = \log |a| + \log |b| = F(a) + F(b),$

so $F$ is a homomorphism from $(\mathbb{R}^\times, \cdot)$ to $(\mathbb{R}, +)$.

To show $F$ is onto: for any $y \in \mathbb{R}$, choose $x = e^y \in \mathbb{R}^+$, then $F(x) = \log |e^y| = y$, so $F$ is surjective.

$F$ is not injective: $F(2) = \log 2 = F(-2)$, but $2 \ne -2$. In fact, $F(a) = F(-a)$ for all $a \in \mathbb{R}^\times$, so the kernel is ${\pm 1}$. Hence no such $F$ can be injective.


3 consecutive integers

$a^i b = b a^i$ and $a^{i+1} b = b a^{i+1}$

$$

$$
$ab=aba^ia^{-i}=aa^iba^{-i}=a^{i+1}ba^{-i}=ba^{i+1}a^{-i}=ba.$

find a counter for 2

Let $G = UT_3(\mathbb{R})$, the group of $3 \times 3$ upper unitriangular matrices over $\mathbb{R}$:

$$a = \begin{bmatrix} 1 & x & y \\ 0 & 1 & z \\ 0 & 0 & 1 \end{bmatrix},\quad b = \begin{bmatrix} 1 & u & v \\ 0 & 1 & w \\ 0 & 0 & 1 \end{bmatrix}.$$Then $G$ is nilpotent of class 2 (non-abelian), but satisfies:$$(ab)^n = a^n b^n \quad \text{for } n = 1, 2.$$

So take $i = 1$, $i+1 = 2$.

Hence, $(ab)^i = a^i b^i$ and $(ab)^{i+1} = a^{i+1} b^{i+1}$ hold, yet $G$ is not abelian.

---
From $(ab)^3=a^3b^3$ and $(ab)^5=a^5b^5$ it follows that $(ba)^2=a^2b^2$, and $(ba)^4=a^4b^4$. This implies $(ba)^4=(ba)^2(ba)^2=a^2b^2a^2b^2=a^4b^4$, so $b^2a^2=a^2b^2$, hence all squares commute. Thus $(ba)^2=baba=a^2b^2=b^2a^2=bbaa$ and it follows that $ab=ba$.
