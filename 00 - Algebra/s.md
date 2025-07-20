
Let $H$ be a finite-dimensional division algebra over a field $K$ with $[H:K] = N$. Then $H \cong K^N$ as a $K$-vector space, and $\text{End}_K(H)$, the ring of $K$-linear endomorphisms of $H$, is isomorphic to $M_N(K)$, the ring of $N \times N$ matrices over $K$. As a right $H$-module, $\text{End}_K(H)$ has a basis of size $N$.

Consider $H$ as a left $K$-vector space with basis $\{e_1, \dots, e_N\}$. Define $f_i \in \text{End}_K(H)$ for $i = 1, \dots, N$ by $f_i(e_j) = \delta_{ij} e_j$, where $\delta_{ij}$ is the Kronecker delta (1 if $i = j$, 0 otherwise), and extend $K$-linearly to all of $H$. These $f_i$ are $K$-linear maps.

To show $\{f_1, \dots, f_N\}$ is a basis for $\text{End}_K(H)$ as a right $H$-module:
- **Spanning**: Any $\phi \in \text{End}_K(H)$ maps $e_j \to \sum_{i=1}^N a_{ij} e_i$ with $a_{ij} \in K$. Since $H$ is a division algebra, for each $e_j$, we can write $\phi(e_j) = \sum_{i=1}^N f_i(e_j) h_i$ for some $h_i \in H$, as $f_i(e_j) = \delta_{ij} e_j$. Thus, $\phi = \sum_{i=1}^N f_i h_i$, where right $H$-action is $(f_i h)(x) = f_i(x) h$.
- **Linear independence**: Suppose $\sum_{i=1}^N f_i h_i = 0$. Apply to $e_j$: $\sum_{i=1}^N f_i(e_j) h_i = \sum_{i=1}^N \delta_{ij} e_j h_i = e_j h_j = 0$. Since $e_j \neq 0$ and $H$ is a division algebra, $h_j = 0$ for all $j$. Thus, the $f_i$ are independent.

Since $\text{End}_K(H) \cong M_N(K)$ has dimension $N^2$ over $K$, and $[H:K] = N$, the rank of $\text{End}_K(H)$ as a right $H$-module is $N^2 / N = N$. Hence, $\{f_1, \dots, f_N\}$ is a basis of size $N$.