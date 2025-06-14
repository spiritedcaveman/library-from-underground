# 1.
 Suppose that $G = S_3$, and that $V = \operatorname{sp}(v_1, v_2, v_3)$ is the permutation module for $G$ over $\mathbb{C}$, as in Definition 4.10. Let $\mathcal{B}_1$ be the basis $v_1, v_2, v_3$ of $V$ and let $\mathcal{B}_2$ be the basis $v_1 + v_2 + v_3, v_1 - v_2, v_1 - v_3$. Calculate the $3 \times 3$ matrices $[g]_{\mathcal{B}_1}$ and $[g]_{\mathcal{B}_2}$ for all $g$ in $S_3$. What do you notice about the matrices $[g]_{\mathcal{B}_2}$?
 
 Soln.
 The action of $S_3$ on the basis $\mathcal{B}_1 = \{v_1, v_2, v_3\}$, where each permutation $\sigma \in S_3$ sends $v_i \mapsto v_{\sigma(i)}$ 

Matrices $[g]_{\mathcal{B}_1}$:
  
$e$: identity $\rightarrow$

$I = \begin{pmatrix}1&0&0\\0&1&0\\0&0&1\end{pmatrix}$

$(12)$: swaps 1 and 2 $\rightarrow$

$\begin{pmatrix}0&1&0\\1&0&0\\0&0&1\end{pmatrix}$

$(13)$: swaps 1 and 3 $\rightarrow$

$\begin{pmatrix}0&0&1\\0&1&0\\1&0&0\end{pmatrix}$

$(23)$: swaps 2 and 3 $\rightarrow$

$\begin{pmatrix}1&0&0\\0&0&1\\0&1&0\end{pmatrix}$

$(123)$: $1 \rightarrow 2, 2 \rightarrow 3, 3 \rightarrow 1$ $\rightarrow$

$\begin{pmatrix}0&1&0\\0&0&1\\1&0&0\end{pmatrix}$

$(132)$: $1 \rightarrow 3, 3 \rightarrow 2, 2 \rightarrow 1$ $\rightarrow$

$\begin{pmatrix}0&0&1\\1&0&0\\0&1&0\end{pmatrix}$

  
$$\mathcal{B}_2 = \left\{v_1 + v_2 + v_3,\ v_1 - v_2,\ v_1 - v_3 \right\}.$$


* $w_1 = v_1 + v_2 + v_3$,

* $w_2 = v_1 - v_2$,

* $w_3 = v_1 - v_3$

---

  

### Step 1: Build change-of-basis matrix $P$

  

  

$$

P =

\begin{pmatrix}

1 & 1 & 1 \\

1 & -1 & 0 \\

1 & 0 & -1

\end{pmatrix}

\Rightarrow P^{-1} =

\frac{1}{3}

\begin{pmatrix}

1 & 1 & 1 \\

1 & -2 & 1 \\

1 & 1 & -2

\end{pmatrix}

$$

  

---

  

### Step 2: Use $[g]_{\mathcal{B}_2} = P^{-1} [g]_{\mathcal{B}_1} P$

  

  

#### 1. $g = e$ (identity):

  

$$[g]_{\mathcal{B}_1} = I \Rightarrow [e]_{\mathcal{B}_2} = P^{-1} I P = I$$

  

#### 2. $g = (12)$:

  

$$

[g]_{\mathcal{B}_1} =

\begin{pmatrix}

0 & 1 & 0 \\

1 & 0 & 0 \\

0 & 0 & 1

\end{pmatrix}

\Rightarrow

[(12)]_{\mathcal{B}_2} = P^{-1} [g]_{\mathcal{B}_1} P

=

\begin{pmatrix}

1 & 0 & 0 \\

0 & -1 & 0 \\

0 & 0 & 1

\end{pmatrix}

$$

  

#### 3. $g = (123)$:

  

$$

[g]_{\mathcal{B}_1} =

\begin{pmatrix}

0 & 1 & 0 \\

0 & 0 & 1 \\

1 & 0 & 0

\end{pmatrix}

\Rightarrow

[(123)]_{\mathcal{B}_2} = P^{-1} [g]_{\mathcal{B}_1} P

=

\begin{pmatrix}

1 & 0 & 0 \\

0 & -\frac{1}{2} & -\frac{3}{2} \\

0 & \frac{1}{2} & -\frac{1}{2}

\end{pmatrix}

$$

  

---

  

### Final Observation

  

Every matrix has the form:

  

$$

[g]_{\mathcal{B}_2} =

\begin{pmatrix}

1 & 0 & 0 \\

0 & * & * \\

0 & * & *

\end{pmatrix}

$$

  

which shows that $w_1 = v_1 + v_2 + v_3$ is **fixed** and the other two components span a 2D invariant subspace — the standard rep.

All $[g]_{\mathcal{B}_2}$ matrices have the first basis vector fixed (the vector $v_1 + v_2 + v_3$), meaning the top-left entry of every matrix is 1, and the rest of the matrix acts on the 2D subspace orthogonal to it.

That is, the permutation representation splits as:

$$V \cong \mathbb{C} \oplus W$$

where $\mathbb{C}$ is the trivial representation, and $W$ is the standard (2D) representation of $S_3$.


---


# 2.
 Let $G = S_n$ and let $V$ be a vector space over $F$. Show that $V$ becomes an $FG$-module if we define, for all $v \in V$,
 $$vg = \begin{cases} v, & \text{if } g \text{ is an even permutation}, \\ -v, & \text{if } g \text{ is an odd permutation}. \end{cases}$$
 Proof.
 
 Let $\text{sgn} : S_n \to \{\pm 1\}$ be the sign homomorphism. Define the action on $V$ by:
$$v \cdot g := \text{sgn}(g)\cdot v.$$

Let $v \in V$, $g, h \in S_n$.

- Identity: $\text{sgn}(1) = 1$, so $v \cdot 1 = v$.
- Compatibility: $(v \cdot g) \cdot h = \text{sgn}(g)\cdot v \cdot h = \text{sgn}(g)\text{sgn}(h)v = \text{sgn}(gh)v = v \cdot (gh)$, since sgn is a homomorphism.
So this defines a valid $FG$-module.


---

# 3.
 Let $Q_8 = \langle a, b : a^4 = 1, b^2 = a^2, b^{-1} ab = a^{-1} \rangle$, the quaternion group of order 8. Show that there is an $\mathbb{R}Q_8$-module $V$ of dimension 4 with basis $v_1, v_2, v_3, v_4$ such that
$$v_1 a = v_2, \quad v_2 a = -v_1, \quad v_3 a = -v_4, \quad v_4 a = v_3,$$                       and$$v_1 b = v_3, \quad v_2 b = v_4, \quad v_3 b = -v_1, \quad v_4 b = -v_2.$$
Proof.
 $a$ acts via:

  $$
  a = \begin{pmatrix}
  0 & -1 & 0 & 0 \\
  1 & 0 & 0 & 0 \\
  0 & 0 & 0 & 1 \\
  0 & 0 & -1 & 0
  \end{pmatrix}
  \quad \text{so that} \quad
  a(v_1) = v_2, \,
  a(v_2) = -v_1, \,
  a(v_3) = -v_4, \,
  a(v_4) = v_3.
  $$
$b$ acts via:

  $$
  b = \begin{pmatrix}
  0 & 0 & -1 & 0 \\
  0 & 0 & 0 & -1 \\
  1 & 0 & 0 & 0 \\
  0 & 1 & 0 & 0
  \end{pmatrix}
  \quad \text{so that} \quad
  b(v_1) = v_3, \,
  b(v_2) = v_4, \,
  b(v_3) = -v_1, \,
  b(v_4) = -v_2.
  $$
 just check that these linear maps respect the group algebra
  
 ---
 
# 4.
Let $A$ be an $n \times n$ matrix and let $B$ be a matrix obtained from $A$ by permuting the rows. Show that there is an $n \times n$ permutation matrix $P$ such that $B = PA$. Find a similar result for a matrix obtained from $A$ by permuting the columns.

Soln.

 There exists a permutation matrix $P_\sigma \in \text{GL}(n, \mathbb{F})$ such that for any vector $v \in \mathbb{F}^n$,
$$P_\sigma v = v^\sigma = (v_{\sigma^{-1}(1)}, \dots, v_{\sigma^{-1}(n)}),$$i.e., left multiplication by $P_\sigma$ permutes the rows of $A$:$$B = P_\sigma A.$$Similarly, right multiplication by $P_\sigma$ permutes the columns:$$C = A P_\sigma,$$
since each column vector is sent to another column via the permutation.
So the result is:

Row permutation: $B = PA$ for a permutation matrix $P$
Column permutation: $C = AP$
These are both left and right actions of $S_n$, realized via matrix multiplication, and they form natural representations of $S_n$ — embedded in the group algebra $\mathbb{F}S_n$.

