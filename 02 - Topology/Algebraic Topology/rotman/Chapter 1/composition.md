$X/\sim$ is always a continuous surgection but it may not be a open map


fibers are the equivalence classes of the equivalence relation $ker(f)$ on $X$

atmost relaxed case $ker$ is trivial and we get to do $X/1$ so the map is fiber is just a point now?



A continuous surjection $f: X \to Y$ is an **identification** if a subset $U$ of $Y$ is open if and only if $f^{-1}(U)$ is open in $X$.

Given two topological spaces $(X,\mathcal{T}_X)$ and $(Y,\mathcal{T}_Y)$, a map $f:X\rightarrow Y$ is an identification map iff it is surjective and for every subset $U$ of $Y$, $U\in\mathcal{T}_Y$ is equivalent to $f^{-1}(U)\in \mathcal{T}_X$.

continuous + open + surjective $\implies$identification




identification classification

```tikz
\usepackage{tikz-cd}

\begin{document}

\begin{tikzcd}
X \arrow[rr, "\nu"] \arrow[dr, "f"'] & & X/\ker f \\
& Y \arrow[ur, "\varphi^{-1}"'] &
\end{tikzcd}

\end{document}
```




That $\varphi^{-1} f = \nu$ is continuous implies that
$$\varphi^{-1}: Y \to X/ker f$$
is continuous, by hypothesis.
Also, $\varphi$ is continuous because $\nu$ is an identification. We conclude that $\varphi$ is a
homeomorphism, and the result follows at once.

