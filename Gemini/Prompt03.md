Flipping the signature convention from "mostly plus" $(+, +, +, -)$ to "mostly minus" $(-, -, -, +)$ changes the signs of individual tensor components $\eta_{\mu\nu}$, but it does not change the physical physics, inner products, or path integrals.

Because it is purely a cosmetic change of notation, flipping the overall metric sign alone does not resolve the sign problem.

### 1. Invariance of the Physical Action

In relativistic field theory, physical observables, field equations, and path integrals are invariant under a global sign flip of the metric metric tensor $\eta_{\mu\nu} \to -\eta_{\mu\nu}$.

* **Minkowski Invariant:** The line element transforms as $ds^2 = \eta_{\mu\nu} dx^\mu dx^\nu \to -ds^2$. The scalar $p^\mu p_\mu = p^\mu p^\nu \eta_{\mu\nu}$ flips sign, but all physical invariants (like invariant mass $m^2$) are redefined consistently alongside the metric.
* **Gauge Field Action:** The Yang-Mills action is written as:

$$S = -\frac{1}{4} \int d^4x \, F_{\mu\nu} F^{\mu\nu}$$



When raising/lowering indices, $F^{\mu\nu} = \eta^{\mu\alpha} \eta^{\nu\beta} F_{\alpha\beta}$. Flipping the metric signature from $(+,+,+,-)$ to $(-,-,-,+)$ introduces two factors of $(-1)$ when raising indices for $F^{\mu\nu}$, which cancel out:

$$(-1) \times (-1) = +1$$



The resulting Lagrangian density and action $S$ remain identical.

### 2. Why the Sign Problem Persists

The numerical sign problem on a lattice stems from the transition from real-time Minkowski space to Euclidean imaginary time via Wick rotation ($t \to -i\tau$):

| Metric Signature | Minkowski Space | Wick Rotation ($t = -i\tau$) | Euclidean Action / Measure |
| --- | --- | --- | --- |
| **Mostly Plus $(+,+,+,-)$** | $\text{diag}(+1,+1,+1,-1)$ | $\tau^2 = -t^2 \implies -dt^2 = +d\tau^2$ | $d s_E^2 = dx_1^2 + dx_2^2 + dx_3^2 + d\tau^2$ $\implies e^{-S_E}$ |
| **Mostly Minus $(-,-,-,+)$** | $\text{diag}(-1,-1,-1,+1)$ | $\tau^2 = -t^2 \implies +dt^2 = -d\tau^2$ | $d s_E^2 = -dx_1^2 - dx_2^2 - dx_3^2 - d\tau^2$ $\implies e^{-S_E}$ |

In both conventions, performing a standard Wick rotation converts the oscillating real-time phase $e^{i S_M}$ into a real exponential decay $e^{-S_E}$ in positive-definite Euclidean space.

The sign problem returns when physical parameters make the fermion determinant complex (such as a chemical potential $\mu \neq 0$ or a topological $\theta$-term):


$$\det M(\mu) \in \mathbb{C}$$


Because $\det M(\mu)$ becomes complex, the path integral measure $d\mu = e^{-S_E} \det M$ is complex regardless of whether you started in $(+,+,+,-)$ or $(-,-,-,+)$.

### 3. What Does Change the Sign Problem?

To alter the sign problem, the metric shift cannot be a global convention change. It must be an **analytic continuation** or **signature alteration** that breaks the standard Euclidean symmetry:

* **Complexified Metric / Complex Langevin:** Continuously deforming the spacetime metric into complex space $\eta_{\mu\nu} \in \mathbb{C}$ (integrating over complexified field configurations rather than real fields).
* **Indefinite Inner Product Spaces:** Introducing actual local signature variations (e.g., non-uniform spatial signatures or $PT$-symmetric non-Hermitian terms) where different field modes pick up relative sign flips that cancel out complex phases along stable Lefschetz thimbles.
