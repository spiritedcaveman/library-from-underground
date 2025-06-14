
We conclude that non-isomorphic groups can have isomorphic automorphism groups.

The Automorphism group permutes the generators, so to speak.
==If $x$ is a generator of $G$ and $\varphi \in \text{Aut}(G)$, then $\varphi(x)$ must be a generator of $G$.==


$\text{Aut}(G) = \{1\}$ if and only if $|G| \le 2$.

Let $G$ be an Abelian group with odd order. If $\varphi : G \to G$ such that $\varphi(x)=x^2$ is an automorphism.

# [If a group 𝐺 has odd order, then the square function is injective.](https://math.stackexchange.com/questions/522273/if-a-group-g-has-odd-order-then-the-square-function-is-injective)

# Inversion Mapping is Automorphism iff Group is Abelian

Proof.
If $G$ is abelian then the map $x\to x^{-1}$ is a homomorphism:
$$(ab)^{-1}=(ba)^{-1}=a^{-1}b^{-1}$$
If $x\to x^{-1}$ is a homomorphism, $G$ is abelian:
$$ab=(b^{-1}a^{-1})^{-1}=((ba)^{-1})^{-1}=ba$$

----------

$x\to x^{-1}$ is a bijection as proved in the question. So if it is a homomorphism, it is an automorphism.

Alternatively, $\phi$ is an automorphism, and $\phi([a,b]) = [a,b]^{-1}$, so the commutator subgroup is inverted. But inversion is trivial on the abelianization, so $[G,G] \subseteq [G,G]^{-1}$ and equal.

If $\phi$ is an automorphism, this fixes $G/G'$, so inversion acts trivially on it $\Rightarrow [G,G] = [G,G]^{-1}$.

But inversion maps $x \mapsto x^{-1}$, so if $x = x^{-1}$ for all $x \in [G,G]$, then every commutator is its own inverse $\Rightarrow$ each is of order $\le 2$. But $[a,b] = e$ for all $a,b$ implies $G$ is abelian. Thus, the map $x \mapsto x^{-1}$ is a homomorphism $\iff G$ is abelian.


**A group $G$ is ==complete== if it is centerless and every automorphism of $G$ is inner.** 

so $\operatorname{Aut}(G) \cong G$, almost every symmetric group is complete