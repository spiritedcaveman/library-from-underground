

# 2.24.
 Let $G = \langle A, B \rangle \le \text{GL}(2, \mathbb{C})$, where
 $$A = \begin{bmatrix} 0 & i \\ i & 0 \end{bmatrix} \quad \text{and} \quad B = \begin{bmatrix} 0 & 1 \\ -1 & 0 \end{bmatrix}.$$ Show that $G$ is a nonabelian group (so $G$ is not cyclic) of order 8 having a unique subgroup of order 2. (See Theorem 4.22.)
 
 Proof.
  Compute powers: $A^2 = -I$, $A^4 = I$, so $A$ has order 4. Similarly, $B^2 = -I$, $B^4 = I$, so $B$ has order 4. Product: $AB = \begin{bmatrix} 0 & i \\ -i & 0 \end{bmatrix}$, $(AB)^2 = -I$, $(AB)^4 = I$, so $AB$ has order 4. Check: $BA = -AB$, so $G$ is nonabelian.

  Elements: $G = \{ I, A, -I, -A, B, -B, AB, -AB \}$, these are distinct, so $|G| = 8$. Noncyclic: $\langle A \rangle = \{ I, A, -I, -A \}$, similarly for $\langle B \rangle$ and $\langle AB \rangle$, none generate all 8 elements.

  Order 2 subgroup: Only $(-I)^2 = I$, so $\{ I, -I \}$ is the unique subgroup of order 2, as no other element has order 2.

  Structure: 1 element of order 1 ($I$), 1 element of order 2 ($-I$), 6 elements of order 4 ($A, -A, B, -B, AB, -AB$). The center is $\{ I, -I \}$. This matches the quaternion group $Q_8$ with the identifications $A \leftrightarrow i$, $B \leftrightarrow j$, $AB \leftrightarrow k$, satisfying $A^2 = B^2 = -I$ and $BA = -AB$. It is not the dihedral group $D_8$, which has 5 elements of order 2.

  Thus, $G \cong Q_8$, which is nonabelian, of order 8, and has a unique subgroup of order 2.
