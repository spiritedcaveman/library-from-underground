# 1.2.
An element _x_ of a non-unital ring _R_ is said to be **right [quasiregular](https://en.wikipedia.org/wiki/Quasiregular_element)** if there exists _y_ in _R_ such that $x+y-xy=0$
it forms a group


# Ex. 1.6

$\emptyset$ and $M$ are the zero respectively the identity element, each non-void disjoint subsets of $M$ are zero divisors and clearly $A \cap A = A$ so that each element is idempotent. All the ring verifications are simple with the only one exception: the associativity of the addition. Let $A, B, C$ be subsets of $M$. One has to use the following immediate formula $A + B = (A \cup B) \cap C_M (A \cap B)$ and to obtain by computation $(A + B) + C =$

$$\{[(A \cup B) \cap C_M (A \cap B)] \cup C\} \cap C_M \{[(A \cup B) \cap C_M (A \cap B)] \cap C\} = (A \cup B \cup C) \cap (A \cup C_M (B) \cup C_M (C)) \cap (C_M (A) \cup B \cup C_M (C)) \cap (C_M (A) \cup C_M (B) \cup C)$$

which equals with $A + (B + C)$ by commutativity (which is obvious) and symmetry.


# ex 1.11.

rings of $p$ element


# 1.16.

$$r^2 - r \in Z(R) \Rightarrow r^{2} \in Z(R) \quad \text{and} \quad r \in Z(R)$$ The elements $a^2-a, b^2-b, (a+b)^2-(a+b) = (a^2-a) + (b^2-b) + ab+ba$ belong to $Z(R)$ so that $ab+ba \in Z(R)$. Then $a(ab+ba) = (ab+ba)a$ or $a^2b = ba^2$. These two elements being arbitrary $a^2 \in Z(R)$ and hence $a=a^2-(a^2-a) \in Z(R)$.

# 1.17.

Units of $Z[i]$ are $\{ \pm 1, \pm i \}$ and it is a cyclic group.

# 1.18.

 Let $N : \mathbb{Z}[\sqrt{d}] \to \mathbb{Z}$ be a map defined as follows: $N(a+b\sqrt{d}) = a^2 - db^2$ for each square-free integer $d$. For $x = a + b\sqrt{d}$ we denote by $\bar{x} = a - b\sqrt{d}$. Then the following hold: $N(x) = x.\bar{x} = N(\bar{x})$, $\overline{x.y} = \bar{x}.\bar{y}$, $N(x.y) = N(x).N(y)$. If $x$ is a unit in $\mathbb{Z}[\sqrt{d}]$ then, for a suitable $y \in \mathbb{Z}[\sqrt{d}]$, we have $1 = N(1) = N(xy) = N(x)N(y)$ in $\mathbb{Z}$ so that $N(x) \in \{-1,1\}$. Conversely, if $N(x) \in \{-1,1\}$ then $x \cdot (\pm \bar{x}) = 1$ and $x$ is a unit in $\mathbb{Z}[\sqrt{d}]$. Now, for $d=2$ the real number $a = 1+\sqrt{2}$ is a unit of $\mathbb{Z}[\sqrt{d}]$ because $N(a) = -1$. We check immediately that all $a^n(n \in \mathbb{N})$ are different units in $\mathbb{Z}[\sqrt{2}]$ (a strictly increasing sequence of limit $\infty$), e.g. $3 + 2\sqrt{2}, 7+5\sqrt{2}, \dots$

Units are being mapped to units in a homo, well $1$ is getting mapped to $1$ and take an element and it's inverse and look at the triangle and it's morphism


# 1.19.

 Let $u \in R$ be an inverse for $1 - ab$. Then one easily verifies that $1 + bua$ is the inverse of $1 - ba$. Indeed, for instance $(1 - ba)(1 + bua) = 1 - ba + bua - babua = 1 - ba + b(1 - ab)ua = 1 - ba + ba = 1$.



# 1.20

$\Bbb{Z}_{n}$ has no nilpotent elements **iff** $n$ is not square free

If $n = p^2t$ with $p$ prime then $\overline{0} \ne \overline{pt}$ has zero square (is nilpotent).

Conversely, let $n$ be a square-free integer, i.e. $n = p_1p_2...p_k$ and $\overline{a}^m = \overline{0}$ a nilpotent element. We prove that $\overline{a} = \overline{0}$. Indeed, $\overline{a}^m = \overline{0}$ in $\mathbb{Z}_n$ implies $n|a^m$ and hence $p_i|a^m$ ($i \in \{1,2,...,k\}$). Then $p_i|a$ and $n|a$ (because $p_i$ are different primes) so that $\overline{a} = \overline{0}$.