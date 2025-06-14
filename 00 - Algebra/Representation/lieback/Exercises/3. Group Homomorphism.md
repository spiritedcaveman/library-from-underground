
# 1.
Let $G$ be the cyclic group of order $m$, say $G = \langle a : a^m = 1 \rangle$. Suppose that $A \in \text{GL}(n, \mathbb{C})$, and define $\rho : G \to \text{GL}(n, \mathbb{C})$ by
$$\rho : a^r \mapsto A^r \quad (0 \le r \le m - 1).$$
Show that $\rho$ is a representation of $G$ over $\mathbb{C}$ if and only if $A^m = I$.

Proof.

$(\Rightarrow)$ If $\rho$ is a representation, then it must be a group homomorphism. In particular,
$$\rho(a^m) = \rho(1_G) = I \in \mathrm{GL}(n, \mathbb{C}).$$
But $\rho(a^m) = A^m$, so $A^m = I$.\\

$(\Leftarrow)$ If $A^m = I$, then for all $r, s \in \mathbb{Z}$,
$$\rho(a^r a^s) = \rho(a^{r+s}) = A^{r+s} = A^r A^s = \rho(a^r)\rho(a^s),$$
so $\rho$ respects the group operation and is a homomorphism.


---

# 2.
Let
$$A = \begin{pmatrix} 1 & 0 \\ 0 & 1 \end{pmatrix}, \quad B = \begin{pmatrix} 1 & 0 \\ 0 & e^{2\pi i / 3} \end{pmatrix}, \quad C = \begin{pmatrix} 0 & 1 \\ -1 & -1 \end{pmatrix}$$and let $G = \langle a : a^3 = 1 \rangle \cong C_3$. Show that each of the functions $\rho_j : G \to \text{GL}(2, \mathbb{C})$ $(1 \le j \le 3)$, defined by$$\rho_1 : a^r \mapsto A^r,$$$$\rho_2 : a^r \mapsto B^r,$$$$\rho_3 : a^r \mapsto C^r \quad (0 \le r \le 2),$$
is a representation of $G$ over $\mathbb{C}$. Which of these representations are faithful?

Proof.
 $\rho_1$: $A=I$, so $A^r = I^r = I$ for all $r \implies$ not faithful (kernel is all of $G$).
 
$\rho_2$: $B^3 = \begin{pmatrix} 1 & 0 \\ 0 & e^{2\pi i} \end{pmatrix} = I$, and $B^r \ne I$ for $r=1,2 \implies$ faithful.

$\rho_3$:
$C^1 = C = \begin{pmatrix} 0 & 1 \\ -1 & -1 \end{pmatrix}$,
$C^2 = \begin{pmatrix} -1 & -1 \\ 1 & 0 \end{pmatrix}$,
$C^3 = I \implies C$ has order 3 $\implies$ faithful.
Conclusion: $\rho_1$ is not faithful; $\rho_2$ and $\rho_3$ are faithful representations of $C_3$.


---
# 3.
Suppose that $G = D_{2n} = \langle a, b : a^n = b^2 = 1, b^{-1} ab = a^{-1} \rangle$, and $F = \mathbb{R}$ or $\mathbb{C}$. Show that there is a representation $\rho : G \to \text{GL}(1, F)$ such that $\rho(a) = (1)$ and $\rho(b) = (-1)$.

Soln.

we can always form stupid representation by taking $a \mapsto 1$ and $b \mapsto -1$ via $\rho$ and this stupidly obeys the algebra of $D_{2n}$ so we are done

but the interesting part is creating more nuanced representation supposedly where the kernel is smaller and it is "closer" to be faithful

---

# 4.
Suppose that $\rho$, $\sigma$ and $\tau$ are representations of $G$ over $F$. Prove:
(1) $\rho$ is equivalent to $\rho$;
(2) if $\rho$ is equivalent to $\sigma$, then $\sigma$ is equivalent to $\rho$;
(3) if $\rho$ is equivalent to $\sigma$, and $\sigma$ is equivalent to $\tau$, then $\rho$ is equivalent to $\tau$.


Proof.
 Let $P=I$. Then for all $g \in G$,
$$P \rho(g) P^{-1} = I \rho(g) I = \rho(g),$$
so $\rho \sim \rho$.


If $\rho \sim \sigma$, then there exists invertible $P$ such that $\sigma(g) = P \rho(g) P^{-1}$. Then
$$\rho(g) = P^{-1} \sigma(g) (P^{-1})^{-1} = P^{-1} \sigma(g) P,$$
so $\sigma \sim \rho$.


If $\rho \sim \sigma$ via $P$, and $\sigma \sim \tau$ via $Q$, then
$$\tau(g) = Q \sigma(g) Q^{-1} = Q (P \rho(g) P^{-1}) Q^{-1} = (QP) \rho(g) (P^{-1} Q^{-1}) = (QP) \rho(g) (QP)^{-1},$$
so $\rho \sim \tau$.


---
# 5.
 Let $G = D_{12} = \langle a, b : a^6 = b^2 = 1, b^{-1} ab = a^{-1} \rangle$. Define the matrices $A, B, C, D$ over $\mathbb{C}$ by
$$A = \begin{pmatrix} e^{i\pi/3} & 0 \\ 0 & e^{-i\pi/3} \end{pmatrix}, \quad B = \begin{pmatrix} 0 & 1 \\ 1 & 0 \end{pmatrix},$$
$$C = \begin{pmatrix} 1/2 & \sqrt{3}/2 \\ -\sqrt{3}/2 & 1/2 \end{pmatrix}, \quad D = \begin{pmatrix} 1 & 0 \\ 0 & -1 \end{pmatrix}.$$ Prove that each of the functions $\rho_k : G \to \text{GL}(2, \mathbb{C})$ $(k = 1, 2, 3, 4)$, given by$$\rho_1 : a^r b^s \mapsto A^r B^s,$$$$\rho_2 : a^r b^s \mapsto A^{3r} (-B)^s,$$$$\rho_3 : a^r b^s \mapsto (-A)^r B^s,$$
$$\rho_4 : a^r b^s \mapsto C^r D^s \quad (0 \le r \le 5, 0 \le s \le 1),$$
 is a representation of $G$. Which of these representations are faithful? Which are equivalent?
 
 Soln. 


- **Faithful**: $\rho_1, \rho_3, \rho_4$

- **Not faithful**: $\rho_2$

- **Equivalent**: $\rho_1 \sim \rho_3 \sim \rho_4$
  
  ---
# 6.
Give an example of a faithful representation of $D_8$ of degree 3.

Soln.
 Take $\rho: D_8 \to \mathrm{GL}(2, \mathbb{C})$ with
$$A = \begin{pmatrix} e^{i\pi/4} & 0 \\ 0 & e^{-i\pi/4} \end{pmatrix}, \quad B = \begin{pmatrix} 0 & 1 \\ 1 & 0 \end{pmatrix}.$$Define $\tilde{A}, \tilde{B} \in \mathrm{GL}(3, \mathbb{C})$ by:$$\tilde{A} = \begin{pmatrix} e^{i\pi/4} & 0 & 0 \\ 0 & e^{-i\pi/4} & 0 \\ 0 & 0 & 1 \end{pmatrix}, \quad
\tilde{B} = \begin{pmatrix} 0 & 1 & 0 \\ 1 & 0 & 0 \\ 0 & 0 & 1 \end{pmatrix}.$$Then define $\tilde{\rho}: D_8 \to \mathrm{GL}(3, \mathbb{C})$ by$$\tilde{\rho}(a^r b^s) = \tilde{A}^r \tilde{B}^s.$$
This is a faithful degree-3 representation of $D_8$.
# 7.
Suppose that $\rho$ is a representation of $G$ of degree 1. Prove that $G/\ker \rho$ is abelian.
Proof.
 Let $\rho: G \to \mathrm{GL}(1, F) = F^\times$ be a 1-dimensional representation. Then:

$\rho(g)\rho(h) = \rho(gh)$ for all $g, h \in G$,
but since the target $F^\times$ is abelian, $\rho(g)\rho(h) = \rho(h)\rho(g)$,
so $$\rho(gh) = \rho(hg) \implies \rho(ghg^{-1}h^{-1}) = 1$$
thus $$ghg^{-1}h^{-1} \in \ker \rho \, \forall g, h \in G$$
hence $G/\ker \rho$ is abelian.
So yes, any degree-1 representation has abelian image, and thus the quotient $G / \ker \rho$ must be abelian.
# 8.
Let $\rho$ be a representation of the group $G$. Suppose that $g$ and $h$ are elements of $G$ such that $\rho(g)\rho(h) = \rho(h)\rho(g)$. Does it follow that $gh = hg$?

Soln.
 The fact that $\rho(g)\rho(h) = \rho(h)\rho(g)$ means only that the images commute—not that $g$ and $h$ do in $G$. Representations, especially non-faithful ones, can collapse noncommuting elements into commuting matrices.

In a 1-dimensional representation, the image lies in $F^\times$, which is abelian. So any elements of $G$, even noncommuting ones like in $D_6$, will have commuting images. For example, define $\rho: D_6 \to \mathbb{C}^\times$ by $\rho(a) = e^{2\pi i / 3}$, $\rho(b) = -1$. Then $\rho(ab) = \rho(a)\rho(b) = \rho(b)\rho(a)$, but $ab \ne ba$ in $D_6$. Thus, commuting images do not imply commuting preimages.