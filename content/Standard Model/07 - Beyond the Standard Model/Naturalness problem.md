In a general QFT, coupling constants and parameters usually run. For example, for fermion and vector masses we have
$$
\begin{align}
 \delta m_{V} & \sim \log\left( \frac{\mu}{\mu_{0}} \right)m_{W} \quad \mathrm{(the\ mass\ breaks\ gauge\ symmery)} ,\\
 \delta m_{f}  & \sim \log\left( \frac{\mu}{\mu_{0}} \right)m_{f}\quad \mathrm{(the\ mass\ breaks\ chiral\ symmetry)}.
\end{align}
$$
The crucial property (which usually valid also for dimensionless coupling constants) is that the variation is proportional to the parameter itself.
This property **is not valid for the mass of scalar particles**, which might renormalize additively.

Now, suppose there is a theory which UV-completes the Standard Model beyond a certain scale $\Lambda$. It's going to generate corrections to the Higgs boson mass of the form
$$
	\delta m_{h}^{2} \sim \frac{1}{16\pi^{2}} \Lambda^{2}.
$$
Now, since $\Lambda\gg m_{h}$, we must necessarily have $\delta m_{h}^{2} \gg m_{h}^{2}$. Because of this, the experimental measured Higgs mass is 
$$
	(125 \ \mathrm{GeV})^{2} \sim m_{h}^{2}(\Lambda) - \delta m_{h}^{2}.
$$
Thus, we have a cancellation going for very many decimal places, which is very strange.

### The problem is not caused by renormalization

Suppose the Standard Model has a UV completion with a heavy particle of mass $M$ and Lagrangian 
$$
	\mathcal{L} \supset -\frac{1}{2}M^{2}S^{2} - \frac{\kappa}{2}H^{\dagger}H S^{2}.
$$
If we integrate out $S$, we find 
$$
	\delta m_{h}^{2} \sim \frac{\kappa}{16\pi^{2}}M^{2}\left( \log \frac{M^{2}}{\mu^{2}} + \dots \right),
$$
and the $M^{2}$ dependence is not a cutoff artifact.

The problems gets even **worse**. It repeats itself up to $M_{\mathrm{pl}}$, so the cancellations get even bigger.

### Other formulation

Suppose there are other irrelevant operators, 
$$
	\mathcal{L} \supset -\mu^{2} H^{\dagger}H + \frac{c_{6}}{\Lambda^{2}}\mathcal{O}_{6}.
$$
Even though it is suppressed, loops may generate contributions comparable with the marginal or relevant operators: 
$$
	\frac{c_{6}}{\Lambda^{2}} \int ^{\Lambda} \frac{d^{4}k}{k^{2}} \sim \frac{c_{6}}{16\pi^{2}}.
$$

A possible solution to the naturalness problem is the [[Composite Higgs]].