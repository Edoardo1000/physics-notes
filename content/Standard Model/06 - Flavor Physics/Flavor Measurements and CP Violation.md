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
Since one-loop processes are usually smaller, experiments probing them are more sensitive to deviations coming from new physics.
Thus, while *tree-level processes help me fix $\rho$ and $\eta$*, **one-loop processes help me probe BSM physics**.

---
# Examples
## Direct CP violation

In the $B^{+}$ decay, we have interference between the following two processes
$$
	B^{+} \to D^{0} + K^{+} \to f,\quad B^{+} \to \bar{D}^{0} + K^{+} \to f,
$$
where $f$ is a **common final state**. CP violation therefore originates from the *interference* between the two possible decay paths.

At tree-level, we have 
$$
	\frac{A(B\to K \bar{D}^{0})}{A(B\to KD^{0})} \propto \frac{V_{ub}^{*}V_{cs}}{V_{cb}^{*}V_{us}}.
$$
This quantity, however, changes under a rephasing of $\ket{D^{0}},\ket{\bar{D}^{0}}$, so we need to *rescale* it to have physically meaningful quantities.

The quantity we are able to measure is for example
$$
	\lambda_{Kf} \equiv \frac{A_{K\bar{D}}}{A_{KD}} \left( \frac{q}{p} \right)_{D} \sim \frac{V_{ub}^{*}V_{ud}}{V_{cd}V_{cb}^{*}}.
$$
From this, we find 
$$
	\mathrm{Arg}(\gamma) \sim \gamma,
$$
with $\gamma$ the **angle at the origin** of the unitarity triangle.

## Time-dependent CP asymmetry

### B decay 
I can measure the time-dependent interference between the processes (note that $K_{S}$ is the short-lived kaon)
$$
	B_{d}^{0}\to J /\psi + K_{S},\quad B_{d}^{0}\to \bar{B}_{d}^{0} \to J / \psi + K_{S}
$$
where I can measure the interference with the mixing $B^{0} \leftrightarrow \bar{B}^{0}$. It is a 1-loop process.

I get the triangle angle 
$$
	\beta = \mathrm{Arg}\left( - \frac{V_{cd}V_{cb}^{*}}{V_{td}V_{tb}^{}} \right)
$$
and also 
$$
	\mathrm{Im}\lambda_{\psi K} = \sin 2\beta = \delta_{J / \psi}
$$
## Meson mixing
### Kaon mixing
We need to calculate the diagram for $\bra{\bar{M}^{0}}H\ket{M^{0}}$ In fact, there is a box diagram involving the charged current. We obtain an amplitude
$$
	A \sim \left( \sum_{K} V_{ki} V_{kl}^{*} \right)^{2}.
$$
We can measure
$$
	\epsilon_{k} \sim \mathrm{Im}(M_{12}) \sim \mathrm{Im}(V_{ts}^{*}V_{td})^{2} + \dots = 2 \mathrm{Im}(V_{ts}^{*}V_{td})\mathrm{Re}(V_{ts}^{*}V_{td}).
$$
We have 
$$
	V_{ts}^{*} V_{td} \sim - A^{2} \lambda^{5}(1 - \bar{\rho} - i\bar{\eta}),
$$
from which 
$$
	\epsilon_{k} \propto (1-\bar{\rho}) \bar{\eta},
$$
which is the equation of an **hyperbola**. From this we get $\eta$.

If we calculate the element $M_{12}$, the amplitude is subject to the [[GIM Mechanism]]. The most relevant term is the one for the charm ($\xi_{t}$ is small), so that we have 
$$
	M_{12} \simeq G_{F}^{2} m_{c}^{2} \xi_{c}^{2}.
$$
In the Wolfenstein parametrization, the imaginary contribution comes from the top term instead. The physical statement is that $\mathrm{Im}(\xi_{c}\xi_{t}^{*})\neq 0$.
### B meson mixing
*This is not a CP phase measurement, it only measures the mixing amplitude.*
$$
B^0 = \bar{b}d
$$
The Hamiltonian eigenstates have a **mass difference** $\Delta m = m_{H} - m_{L}$.
The mass difference can be measured by their oscillations, in particular, we have 
$$
\begin{align}
	P(B^{0}\to B^{0};t)  & = \frac{e^{ -\Gamma t }}{2}[1+\cos(\Delta m \; t)], \\
	P(B^{0}\to \bar{B}^{0};t) & = \frac{e^{ -\Gamma t }}{2}[1-\cos(\Delta m \;  t)].
\end{align}
$$
In this case the mass difference measures $(V_{tb}^{*}V_{td})^{2}$.  With this measurement, we  find  
$$
	(1-\bar{\rho})^{2} + \bar{\eta}^{2},
$$
which is a **circumference with center 1**.