Assume for contradiction that there exists a finite simple group $G$ of odd order.\\

Then $G$ is nontrivial and simple $\Rightarrow$ not solvable (since simple $\nRightarrow$ solvable unless cyclic of prime order).
But this contradicts \textcolor{red}{every group of odd order is solvable}, which says every group of odd order is solvable.\\

$\therefore$ No such simple group exists. So every finite simple group has even order.



**Assume $G$ is a finite group of order $p^m q^n$ and not solvable. Then $G$ has a composition series with a nonabelian simple factor, or is itself simple and nonabelian.\\**
**So we may assume $G$ is a nonabelian simple group.**

Now
$$|G| = |Z(G)| + \sum_{i} |C_i|$$
But since $G$ is simple nonabelian, $Z(G) = 1$, and all conjugacy classes have size $>1$. So:\\

$|G| = \sum \text{(conj class sizes)}$\\
All class sizes divide $|G| = p^m q^n$.
But no class size is a prime power $> 1$, by Burnside’s theorem (as given).\\
So all conjugacy class sizes are 1 (impossible) or not prime powers.\\

But all proper divisors of $p^m q^n$ are prime powers or products of two powers — so at least one class must have size a prime power $> 1$.\\
Contradiction.\\

Hence, $G$ cannot be nonabelian simple.
So all composition factors are abelian $\Rightarrow$ $G$ is solvable.\\

This proves Burnside’s theorem