

$$n = \sum_{d|n} \varphi(d)$$
where the sum is over all divisors $d$ of $n$ with $1 \le d \le n$.

$|\operatorname{gen}(C_d)| = |\varphi (d)|$

A group $G$ of order $n$ is cyclic if and only if, for each divisor $d$ of $n$, there is at most one cyclic subgroup of $G$ having order $d$.

Take $D_8 = \langle r, s \mid r^4 = s^2 = 1, sr = r^{-1}s \rangle$, the dihedral group of order 8. The cyclic subgroups of $D_8$ are:

$\langle r \rangle = \{1, r, r^2, r^3\}$ (of order 4), with generators $\text{gen}(\langle r \rangle) = \{r, r^3\}$.
$\langle r^2 \rangle = \{1, r^2\}$ (of order 2), with generator $\text{gen}(\langle r^2 \rangle) = \{r^2\}$.
$\langle s \rangle = \{1, s\}$ (of order 2), with generator $\text{gen}(\langle s \rangle) = \{s\}$.
$\langle rs \rangle = \{1, rs\}$ (of order 2), with generator $\text{gen}(\langle rs \rangle) = \{rs\}$.

Since $D_8$ is not cyclic, every element lies in some cyclic subgroup, and the group decomposes as
$D_8 = \{1\} \sqcup \{r, r^3\} \sqcup \{r^2\} \sqcup \{s\} \sqcup \{rs\}$.
This illustrates the decomposition of a non-cyclic group into disjoint generator sets of cyclic subgroups.

## any group is union of disjoint generator of cyclic subgroups


If $C$ is a cyclic subgroup of a group $G$, let $\text{gen}(C)$ denote the set of all its generators. It is clear that $G$ is the disjoint union
$$G = \bigsqcup \text{gen}(C)$$

