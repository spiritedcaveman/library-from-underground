We have already seen that $S_3$ is not nilpotent, but both $A_3 \cong \mathbb{Z}/3\mathbb{Z}$ and $S_3/A_3 \cong \mathbb{Z}/2\mathbb{Z}$ are abelian, hence nilpotent.

Let G be a finite group. Then G is nilpotent if and only if every subgroup of G is subnormal.
(from isaacs)

https://planetmath.org/normalizercondition


**A finite group $G$ is nilpotent if and only if it is the direct product of its Sylow subgroups.**

every finite p group is nilpotent:

Let $G$ be a finite $p$-group.

Base: $|G| = 1 \Rightarrow G$ is trivially nilpotent.

Inductive step: $|G| > 1$, assume all smaller $p$-groups are nilpotent. Then $Z(G) \ne \{e\}$ (by the class equation). So $Z(G)$ is abelian $\Rightarrow$ nilpotent. Also, $|G/Z(G)| < |G|$ $\Rightarrow$ $G/Z(G)$ is nilpotent by hypothesis. Since $Z(G) \trianglelefteq G$ and $G/Z(G)$ is nilpotent, apply: if $N \le Z(G)$ and $G/N$ is nilpotent, then $G$ is nilpotent.