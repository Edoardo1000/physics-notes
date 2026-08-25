The single parameters of the [[Quark Mass Mixing and CKM Matrix|CKM matrix]] are not physical, since I can perform the transformation 
$$
	u_{i} \to e^{ i\alpha_{i} }u_{i}, \quad d_{i} \to e^{ i \beta_{i} }d_{i},
$$
which corresponds to $V_{ij}\to e^{ i(\beta_{j}-\alpha_{i}) }V_{ij}$. Notice that now this transformation does not change the Yukawa sector since we diagonalized the Yukawa matrices.

To get observables, I build
- **absolute values:** $\lvert V_{ij} \rvert^{2}$;
- **products:** $\frac{V_{ik}^{*}V_{jk}}{V_{il}^{*}V_{jl}}$;
- **quartets:** $V_{ij} V_{kl} V^*_{il} V^*_{kj}$.
Because of unitarity, not all of them are independent. For example, we have 
$$
	\sum_{k} \lvert V_{ik} \rvert ^{2} = 1, \quad \sum_{k}V_{ki}^{*}V_{kj}=0,\quad i \neq j.
$$
Since $\lambda$ is small, there are nontrivial precision cancellations going on.
## Invariant expressions

The observables we built were not invariant under $U(3)$ transformations. This is because we already diagonalized the Yukawa matrices. There is another way  to describe physical CP violation, and this is done through **invariants**. 

Since, under a flavor transformations, the Yukawa matrices transform as (we use the spurion technique)
$$
	Y_{u} \to U^{\dagger}_{L}Y_{u}V_{u_{R}},\quad Y_{d}\to U_{L}^{\dagger} Y_{d} V_{d_{R}},
$$
from which we can build the matrices 
$$
	H_{u} = Y_{u}Y_{u}^{\dagger},\quad H_{d} = Y_{d}Y_{d}^{\dagger}.
$$
Now, quantities such as 
$$
	\mathrm{Tr}[H_{u},H_{d}]^{n},\quad \det[H_{u},H_{d}]
$$
are invariant. In particular, the determinant is CP-odd, and is a direct measure of physical CP violation.

We also have the **Jarlskog relation**:
$$	\det[Y_{u}Y_{u}^{\dagger},Y_{d}Y_{d}^{\dagger}] = 2iJ \prod_{i < j}(m_{u_{i}^{2}} - m_{u_{j}^{2}})(m_{d_{i}}^{2}-m_{d_{j}}^{2}).
$$
This relation shows that  **CP violation $\iff$ $J \neq 0$ and no quarks are degenerate**.
## Measuring the parameters
#### Tree-level processes
- $\lvert V_{us}  \rvert\sim \lambda$ , this is the **Cabibbo angle**. You measure it from the decay $s \to u + \bar{u} + d$, or $s\to u + \bar{\nu} + \ell$. The semileptonic decays are cleaner than hadron ones. The processes are 
  $$
     K^{-} \to \pi^{0} \ell \bar{\nu}, \quad K^{0} \to \pi^{+} \ell \bar{\nu}.
  $$
- $\lvert V_{c b} \rvert = A \lambda^{2}$, this comes from the decay $b \to c + \bar{\nu} + l$, or in full form 
  $$
  	B \to X_{c} l \bar{\nu}.
  $$
- $\left| V_{ub} \right|^{2} = A^{2}\lambda^{6}(\rho^2 +\eta^2)$. The process is
$$
	b\to u + \ell + \bar{\nu}, \quad B \to X_{u} + \ell + \bar{\nu}.
$$
	Note that it does not measure CP violation.

In order to find $\eta$, I need some other *independent measurement*.
#### One-loop processes
Since one-loop processes are usually smaller, experiments  probing them are more sensitive to **deviations coming from new physics**.
This, *while tree-level processes help me fix $\rho$ and $\eta$*, **one-loop processes help me probe BSM physics**.

---
# Measuring CP violation
- **[[Direct CP Violation]]**
- **[[Meson Mixing]]**
- **[[Time-dependent CP Asymmetries]]**

---
# Measuring the CKM matrix
- **[[Semileptonic Decays]]**
- **[[Nonleptonic Decays]]**
- **[[Flavor Effective Theory]]**
