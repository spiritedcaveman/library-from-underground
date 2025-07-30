# 5.
Suppose that $f_n : [a,b] \to \mathbb{R}$ is an increasing function for each $n$, and that $f(x) = \lim_{n \to \infty} f_n(x)$ exists for each $x$ in $[a,b]$. Is $f$ increasing?


Let $x_1 < x_2$ in $[a,b]$. Since each $f_n$ is increasing, $f_n(x_1) \le f_n(x_2)$ for all $n$. Taking limits,
$$\lim_{n \to \infty} f_n(x_1) \le \lim_{n \to \infty} f_n(x_2),$$
i.e., $f(x_1) \le f(x_2)$. Thus, $f$ is increasing.

---
# 6.
Let $f_n : [a,b] \to \mathbb{R}$ satisfy $|f_n(x)| \le 1$ for all $x$ and $n$. Show that there is a subsequence $(f_{n_k})$ such that $\lim_{k \to \infty} f_{n_k}(x)$ exists for each rational $x$ in $[a,b]$. [Hint: This is a "diagonalization" argument.]


The set of rationals in $[a,b]$, denoted $\mathbb{Q} \cap [a,b]$, is countable. Enumerate it as ${x_1, x_2, x_3, \dots}$. For each $x_i$, the sequence $(f_n(x_i))$ is bounded, hence has a convergent subsequence by Bolzano–Weierstrass.

Proceed inductively: for $x_1$, choose a subsequence $(f_n^{(1)})$ such that $f_n^{(1)}(x_1)$ converges. For $x_2$, extract a subsequence $(f_n^{(2)})$ of $(f_n^{(1)})$ such that $f_n^{(2)}(x_2)$ converges, and so on. At step $k$, extract $(f_n^{(k)})$ from $(f_n^{(k-1)})$ such that $f_n^{(k)}(x_k)$ converges.

Define $f_{n_k} := f_n^{(k)}$. Then for each rational $x_i$, $f_{n_k}(x_i)$ converges as $k \to \infty$. Hence, $\lim_{k \to \infty} f_{n_k}(x)$ exists for each rational $x \in [a,b]$.

---
Let $\mathbb{Q} \cap [a,b] = {q_1, q_2, q_3, \dots}$ be an enumeration of the rationals in $[a,b]$. For each fixed $q_j$, the sequence $(f_n(q_j))$ is bounded in $\mathbb{R}$ (since $|f_n(q_j)| \le 1$), hence by the Bolzano–Weierstrass theorem, it has a convergent subsequence.

Proceed inductively:

- Let $n^{(1)}_k = k$, the original sequence.

- Since $(f_{n^{(1)}_k}(q_1))$ is bounded, choose a subsequence $n^{(2)}_k$ of $n^{(1)}_k$ such that $f_{n^{(2)}_k}(q_1)$ converges.

- Then choose a subsequence $n^{(3)}_k$ of $n^{(2)}_k$ such that $f_{n^{(3)}_k}(q_2)$ converges.

- Continue inductively: at step $j$, choose a subsequence $n^{(j+1)}_k$ of $n^{(j)}_k$ such that $f_{n^{(j+1)}_k}(q_j)$ converges.


Define the diagonal subsequence $f_{n_k} := f_{n^{(k)}_k}$. For each fixed $q_j$, since $n_k \ge n^{(j)}_k$ eventually, and $f_{n^{(j)}_k}(q_j)$ converges, it follows that $f_{n_k}(q_j)$ also converges.

Hence, $\lim_{k \to \infty} f_{n_k}(x)$ exists for each rational $x \in [a,b]$.

---

# 7.
Let $(f_n)$ and $(g_n)$ be real-valued functions on a set $X$, and suppose that $(f_n)$ and $(g_n)$ converge uniformly on $X$. Show that $(f_n + g_n)$ converges uniformly on $X$. Give an example showing that $(f_n g_n)$ need not converge uniformly on $X$ (although it will converge pointwise, of course).

Since $f_n \rightrightarrows f$ and $g_n \rightrightarrows g$ on $X$, for any $\varepsilon > 0$ there exists $N$ such that for all $n \ge N$ and all $x \in X$,
$$|f_n(x) - f(x)| < \varepsilon/2,\quad |g_n(x) - g(x)| < \varepsilon/2.$$Then
$$|(f_n + g_n)(x) - (f + g)(x)| \le |f_n(x) - f(x)| + |g_n(x) - g(x)| < \varepsilon.$$So $f_n + g_n \rightrightarrows f + g$.


Here is a counter-example: 

Take $f_n(x)=g_n(x)=x+{1\over n}$. Both of these sequences are unbounded and converge uniformly to the identity function on $\Bbb R$.

The product $f_n g_n(x)=x^2+{2x\over n}+{1\over n^2}$ converges pointwise to $h(x)=x^2$. But the convergence is not uniform, as $|f_ng_n(x)-h(x)| = |{2x\over n}+{1\over n^2}|$ cannot be made uniformly small  over $\Bbb R$ for any fixed positive integer $n$.

---

# 8.
Let $f_n : \mathbb{R} \to \mathbb{R}$, and suppose that $f_n \rightrightarrows 0$ on every closed, bounded interval $[a,b]$. Does it follow that $f_n \rightrightarrows 0$ on $\mathbb{R}$? Explain.

for all [a, b] (a < b wlog) take n > b

and define the function to be 0 at [-n n] and 1 elsewhere
it stays at 0 inside the interal for every interval, but globaly it has a step so the sup is more than 0

---
Let $f_n : \mathbb{R} \to \mathbb{R}$ be defined by
$$f_n(x) = \begin{cases}
0 & \text{if } x \in [-n, n], \\
1 & \text{otherwise}.
\end{cases}$$Now fix any interval $[a,b]$ with $a < b$. Take $n > b$ so that $[a,b] \subset [-n, n]$. Then for all $x \in [a,b]$, we have $f_n(x) = 0$, so$$\sup_{x \in [a,b]} |f_n(x) - 0| = 0.$$
Hence, $f_n \rightrightarrows 0$ on every closed, bounded interval.
But globally, for each $n$, we still have $f_n(x) = 1$ for $|x| > n$, so
$$\sup_{x \in \mathbb{R}} |f_n(x) - 0| = 1.$$
So $f_n$ does not converge uniformly to $0$ on $\mathbb{R}$.

---
# 9.
For each of the following sequences, determine the pointwise limit on the given interval (if it exists) and the intervals on which the convergence is uniform (if any):
(a) $f_n(x) = x^n$ on $(-1, 1)$;

Pointwise limit:
$$f(x) = \lim_{n \to \infty} x^n = 
\begin{cases}
0 & \text{if } -1 < x < 1 \\
1 & \text{at } x = 1 \\
\text{undefined} \text{{}}\end{cases}$$
Uniform convergence:

On any closed subinterval $[-a,a] \subset (-1,1)$, yes—uniform.

On $(-1,1)$ itself—not uniform.

---

(b) $f_n(x) = n^2 x(1-x^2)^n$ on $[0, 1]$;

**Pointwise limit:**


For $x = 0$ or $x = 1$, clearly $f_n(x) = 0$.

For $x \in (0,1)$: $(1 - x^2)^n \to 0$ exponentially, and $n^2$ grows polynomially. So
$$f_n(x) = n^2 x (1 - x^2)^n \to 0.$$Thus,$$f(x) = \lim_{n \to \infty} f_n(x) = 0 \quad \text{for all } x \in [0,1].$$

**Uniform convergence:**

We estimate the maximum: let
$$x_n = \frac{1}{\sqrt{2}} \Rightarrow f_n(x_n) = n^2 \cdot \frac{1}{\sqrt{2}} \cdot \left(1 - \frac{1}{2}\right)^n = \frac{n^2}{\sqrt{2}} \cdot 2^{-n} \to 0.$$Also, $f_n(x) \ge 0$ on $[0,1]$, so$$\sup_{x \in [0,1]} |f_n(x) - 0| = \max_{x \in [0,1]} f_n(x) \le \frac{n^2}{\sqrt{2}} \cdot 2^{-n} \to 0.$$
Therefore,
$f_n \rightrightarrows 0 \text{ on } [0,1].$

---
(c) $f_n(x) = nx/(1+nx)$ on $[0, \infty)$;

Pointwise limit:

Fix $x \in [0,\infty)$.
If $x = 0$: $f_n(0) = 0$ for all $n$.
If $x > 0$:
$$f_n(x) = \frac{nx}{1 + nx} = \frac{1}{1 + \frac{1}{nx}} \to 1.$$So,
$$f(x) = \begin{cases}
0 & x = 0, \\
1 & x > 0.
\end{cases}$$

**Uniform convergence on $[0, \infty)$:**

No—take $x_n = 1/n$, then
$$f_n\left(\frac{1}{n}\right) = \frac{n \cdot \frac{1}{n}}{1 + n \cdot \frac{1}{n}} = \frac{1}{2}.$$But $f(1/n) = 1$, so$$\left|f_n(1/n) - f(1/n)\right| = \left|\frac{1}{2} - 1\right| = \frac{1}{2} \not\to 0.$$
So convergence is not uniform on $[0,\infty)$.

**Uniform convergence on $[a,\infty)$ with $a > 0$:**

For $x \ge a > 0$,
$$\left|f_n(x) - 1\right| = \frac{1}{1 + nx} \le \frac{1}{1 + na} \le \frac{1}{na} \to 0.$$
So $f_n \rightrightarrows 1$ on $[a,\infty)$ for any $a > 0$.

---

(d) $f_n(x) = nx/(1+n^2 x^2)$ on $[0, \infty)$;


**Pointwise limit:**

For all $x \in [0, \infty)$,
$$
f_n(x) = \frac{nx}{1 + n^2x^2} = \frac{x}{n^{-1} + x^2} \to 0$$

**Uniform convergence:**
– On $[a,\infty)$ with $a > 0$:

For $x \ge a$,
$$f_n(x) = \frac{nx}{1 + n^2x^2} \le \frac{nx}{n^2x^2} = \frac{1}{nx} \le \frac{1}{na} \to 0.$$So $f_n \rightrightarrows 0$ on $[a, \infty)$.
– On $[0,\infty)$:

Take $x_n = 1/n$, then
$$f_n(1/n) = \frac{n \cdot (1/n)}{1 + n^2 \cdot (1/n)^2} = \frac{1}{1 + 1} = \frac{1}{2}.$$But $f(1/n) \to 0$, so
$$\left|f_n(1/n) - 0\right| = \frac{1}{2} \not\to 0.$$
Hence, not uniform on $[0,\infty)$.

---
(e1) $f_n(x) = e^{-nx}$ on $[0, \infty)$;

**Pointwise limit:**

For $x = 0$: $f_n(0) = 1$ for all $n$.

For $x > 0$: $f_n(x) = e^{-nx} \to 0$.

So:
$$f(x) = \begin{cases}
1 & x = 0, \\
0 & x > 0.
\end{cases}$$
**Uniform convergence:**

– On $[a,\infty)$ with $a > 0$:
$$\sup_{x \ge a} |f_n(x) - 0| = \sup_{x \ge a} e^{-nx} = e^{-na} \to 0,$$
so $f_n \rightrightarrows 0$ on $[a, \infty)$.
– On $[0,\infty)$:

Take $x_n = 1/n$, then
$$f_n(1/n) = e^{-n \cdot \frac{1}{n}} = e^{-1}.$$So
$$\left|f_n(1/n) - f(1/n)\right| = e^{-1} \not\to 0.$$
Therefore, $f_n \not\rightrightarrows f$ on $[0,\infty)$.

---
(e2) $f_n(x) = xe^{-nx}$ on $[0, \infty)$;

(e3) $f_n(x) = x^{2}e^{-nx}$ on $[0, \infty)$;

(f) $f_n(x) = nxe^{-nx^2}$ on $[0, \infty)$.

In each of the above examples, will term-by-term integration or differentiation lead to a correct result?

10. Let $f: \mathbb{R} \to \mathbb{R}$ be uniformly continuous, and define $f_n(x) = f(x+(1/n))$. Show that $f_n \rightrightarrows f$ on $\mathbb{R}$.

11. Suppose that $f_n \rightrightarrows f$ on $\mathbb{R}$, and that $f: \mathbb{R} \to \mathbb{R}$ is continuous. Show that $f_n(x+(1/n)) \to f(x)$ (pointwise) on $\mathbb{R}$.

12. Prove that a sequence of functions $f_n : X \to \mathbb{R}$, where $X$ is any set, is uniformly convergent if and only if it is uniformly Cauchy. That is, prove that there exists some $f: X \to \mathbb{R}$ such that $f_n \rightrightarrows f$ on $X$ if and only if, for each $\varepsilon > 0$, there exists an $N \ge 1$ such that $\sup_{x \in X} |f_n(x) - f_m(x)| < \varepsilon$ whenever $m, n \ge N$. [Hint: Notice that if $(f_n)$ is uniformly Cauchy, then it is also pointwise Cauchy. That is, if $\sup_{x \in X} |f_n(x) - f_m(x)| \to 0$ as $m, n \to \infty$, then $(f_n(x))$ is Cauchy in $\mathbb{R}$ for each $x \in X$.]