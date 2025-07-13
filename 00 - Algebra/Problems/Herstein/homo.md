
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
