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
## Measuring the parameters
#### Tree-level processes
- $\lvert V_{us}  \rvert\sim \lambda$ , this is the **Cabibbo angle**. You measure it from the decay $s \to u + \bar{u} + d$, or $s\to u + \bar{\nu} + \ell$. The semileptonic decays are cleaner than hadron ones. The processes are 
  $$
     K^{-} \to \pi^{0} \ell \bar{\nu}, \quad K^{0} \to \pi^{+} \ell \bar{\nu}.
  $$
- $\lvert V_{c b} \rvert = A \lambda^{2}$, this comes from the decay $b \to c + \bar{\nu} + \ell$, or in full form 
  $$
  	B \to X_{c} \ell \bar{\nu}.
  $$
- $\left| V_{ub} \right|^{2} = A^{2}\lambda^{6}(\rho^2 +\eta^2)$. The process is
$$
	b\to u + \ell + \bar{\nu}, \quad B \to X_{u} + \ell + \bar{\nu}.
$$
	Note that it does not measure CP violation.

In order to find $\eta$, I need some other *independent measurement*.
#### One-loop processes
Since one-loop processes are usually smaller, experiments  probing them are more sensitive to deviations coming from new physics.
This, *while tree-level processes help me fix $\rho$ and $\eta$*, **one-loop processes help me probe BSM physics**.

---

