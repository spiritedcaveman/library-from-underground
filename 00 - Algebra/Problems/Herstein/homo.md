
kernerl of G \to Inn is the centre of G

---
Let $\phi: G \to G$ be an automorphism and let $N \triangleleft G$.
We want to show $\phi(N) \triangleleft G$.
Take any $g \in G$ and $n' \in \phi(N)$. Then $n' = \phi(n)$ for some $n \in N$.
Then:
$$g n' g^{-1} = g \phi(n) g^{-1} = \phi(\phi^{-1}(g) \, n \, \phi^{-1}(g)^{-1}).$$
Since $N \triangleleft G$, $\phi^{-1}(g) n \phi^{-1}(g)^{-1} \in N$, so the whole expression lies in $\phi(N)$.
Hence, $g \phi(N) g^{-1} \subseteq \phi(N)$ for all $g \in G \implies \phi(N) \triangleleft G$.

---
The composition $\phi \psi$ of automorphisms is a bijective homomorphism, so $\phi \psi \in \text{Aut}(G)$.

Also, $\phi^{-1}$ exists and is a homomorphism (since inverses of bijective homomorphisms are homomorphisms), so $\phi^{-1} \in \text{Aut}(G)$.

Hence, $\text{Aut}(G)$ is closed under composition and inverses ⟹ $\text{Aut}(G)$ is a group.

---
Let $|G| = pq^n$ with primes $p < q$. By Sylow’s theorems, $n_q \equiv 1 \mod q$ and $n_q \mid p$.

Since $p < q$, the only possibility is $n_q = 1$, so the Sylow $q$-subgroup $Q$ is unique and normal in $G$.

Then $G/Q$ has order $p$, so is cyclic, hence solvable. $Q$ has order $q^n$, a prime power, so it has a composition series (as all $q$-groups do), hence solvable.

Thus $G$ is an extension of solvable groups, hence solvable.

---

$p_{a}$ is bijective because it has the two-sided inverse $p_{a^{-1}}$. 

Then you can verify that is a homomorphism:
$$
p_{a}(x) p_{a}(y)
=
a^{-1} x a a^{-1} y a = a^{-1} x  y a
= p_{a}(xy).
$$

To prove that $Inn(G)$ is a normal subgroup of $Aut(G)$, show that $$p_{a^{-1}} \circ p_{b} = p_{b a^{-1}},$$ and $$\alpha p_{a} \alpha^{-1} = p_{\alpha(a)},$$ if $\alpha \in Aut(G)$.
