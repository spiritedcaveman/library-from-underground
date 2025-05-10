
[Lipschitz continuity](https://en.wikipedia.org/wiki/Lipschitz_continuity#Properties)(iff bounded first derivative) is sufficient to imply uniform continuity, however L.C. is not necessary for U.C.


Consider $f(x) = \sqrt{x}$ on $[0,1]$. 

 **Uniform continuity**: For any $\epsilon > 0$, choose $\delta = \epsilon^2$. If $|x - y| < \delta$, then $$|\sqrt{x} - \sqrt{y}| = \frac{|x - y|}{|\sqrt{x} + \sqrt{y}|} \leq \frac{|x - y|}{\sqrt{x}} \leq \sqrt{|x - y|} < \sqrt{\delta} = \epsilon,$$ since $\sqrt{x} \leq 1$. Thus, $f$ is uniformly continuous on $[0,1]$.
  
 **Lipschitz continuity**: The derivative $f'(x) = \frac{1}{2\sqrt{x}}$ is unbounded near $x = 0$, as $\lim_{x \to 0^+} f'(x) = +\infty$. Since a Lipschitz function requires a bounded first derivative (or a Lipschitz constant $L$ such that $|f(x) - f(y)| \leq L|x - y|$), $f$ is not Lipschitz continuous.

---

