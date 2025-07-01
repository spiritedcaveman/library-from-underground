
# **1.15.**
Show that the $\sin(1/x)$ space $X$ is not path connected. ($\textit{Hint}$: Assume that $f: I \to X$ is a path from $(0,0)$ to $(1/2\pi, 0)$. If $t_0 = \sup\{t \in I: f(t) \in A\}$, then $a = f(t_0) \in A$ and $f(s) \notin A$ for all $s > t_0$. One may thus assume that there is a path $g: I \to X$ with $g(0) \in A$ and with $g(t) \in G$ for all $t > 0$.)

# **1.16.**
Show that $S^n$ is path connected for all $n \ge 1$.

Let $p,q \in S^n$ be distinct points. If $n=0$, $S^0 = \{-1, 1\}$, which is not path-connected. So assume $n \geq 1$.
If $p$ and $q$ are distinct, choose a point $N \in S^n$ such that $N \neq p$ and $N \neq q$. The space $S^n \setminus \{N\}$ is homeomorphic to $\mathbb{R}^n$. Since $\mathbb{R}^n$ is path-connected for all $n \ge 1$, $S^n \setminus \{N\}$ is also path-connected. Therefore, there exists a path in $S^n \setminus \{N\}$ connecting $p$ to $q$. Since this path is also a path in $S^n$, we conclude that $S^n$ is path-connected for $n \ge 1$.

**The stereographic projection is a projection of the $S^n$ onto $\mathbb{R}^{n−1}$**

# **1.17.**
If $U \subset \mathbb{R}^n$ is open, then $U$ is connected if and only if $U$ is path connected. (This is false if "open" is replaced by "closed": the $\sin(1/x)$ space is a (compact) subset of $\mathbb{R}^2$.)

Let $a \in U$ and define $H \subseteq U$ to be the set of points path-connected to $a$ in $U$. Let $K = U \setminus H$. Then $H \cap K = \varnothing$, $H \cup K = U$, and $a \in H$, so $H \ne \varnothing$.

Given any $x \in H$, since $U$ is open, a small ball around $x$ lies in $U$. Any point in that ball is joined to $x$ by a straight path, and since $x$ is joined to $a$, concatenation gives a path from $a$ to nearby points—so those are in $H$. Hence $H$ is open. The same logic shows $K$ is open: if $x \in K$ and could be connected to $a$, then $x \in H$, a contradiction.

So $U$ is the disjoint union of nonempty open sets $H$ and $K$. If $U$ is connected, then $K = \varnothing$, so $H = U$, i.e., every point is path-connected to $a$. Thus $U$ is path-connected. The converse is trivial.

# **1.18.**
Every contractible space is path connected.

# **1.19.**
(i) A space $X$ is path connected if and only if every two constant maps $X \to X$ are homotopic.
(ii) If $X$ is contractible and $Y$ is path connected, then any two continuous maps $X \to Y$ are homotopic (and each is nullhomotopic).

# **1.20.**
Let $A$ and $B$ be path connected subspaces of a space $X$. If $A \cap B \neq \varnothing$ is path connected, then $A \cup B$ is path connected.

# **1.21.**
If $X$ and $Y$ are path connected, then $X \times Y$ is path connected.

# **1.22.**
If $f: X \to Y$ is continuous and $X$ is path connected, then $f(X)$ is path connected.