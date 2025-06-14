Show that the following conditions on a ring $R$ are equivalent: 

 1. $R$ has only one maximal ideal. 
 2. The nonunits of $R$ form an ideal.



$1\Rightarrow 2$: Let $\mathfrak m$ be the unique maximal ideal of $R$ and $x\in R$ is nonunit. The principal ideal $xR$ is then a proper ideal, and, as a consequence of a (presumably known, based on Zorn’s lemma) theorem it is contained in a maximal ideal of $R$. Because $\mathfrak m$ is unique, that maximal ideal must be $\mathfrak m$, thus $xR\subseteq \mathfrak m$ and therefore $x\in\mathfrak m$. This proves $\mathfrak m$ *is* the set of all nonunits, which is therefore an ideal.

$2\Rightarrow 1$: Let $\mathfrak m$ be the ideal made up of non-units. Any proper ideal $\mathfrak n$ can only consist of non-units, so $\mathfrak n\subseteq \mathfrak m$. If $\mathfrak n$ is maximal, this implies $\mathfrak n=\mathfrak m$, i.e. $\mathfrak m$ is the unique maximal ideal.