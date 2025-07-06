```tikz
\usepackage{tikz-cd}

\begin{document}

\begin{tikzcd}
M & N & \text{Coker}(\alpha) \\
& P \arrow["\alpha", from=1-1, to=1-2] \arrow["0"', from=1-1, to=2-2] \arrow["\kappa", from=1-2, to=1-3] \arrow["\beta", from=1-2, to=2-2] \arrow["\gamma", from=1-3, to=2-2]
\end{tikzcd}

\end{document}
```
```tikz
\usepackage{tikz-cd}

\begin{document}
\begin{tikzcd}

    T
    \arrow[drr, bend left, "x"]
    \arrow[ddr, bend right, "y"]
    \arrow[dr, dotted, "{(x,y)}" description] & & \\
    K & X \times_Z Y \arrow[r, "p"] \arrow[d, "q"]
    & X \arrow[d, "f"] \\
    & Y \arrow[r, "g"]
    & Z

\end{tikzcd}
```
