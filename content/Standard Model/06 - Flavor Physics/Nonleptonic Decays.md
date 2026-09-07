Nonleptonic decays are more complicated than [[Semileptonic Decays|semileptonic ones]], because this time the *hadronic current cannot be factorized*.

# Effective Lagrangian

## Tree-level
Let's call the operators 
$$
\begin{align}
	\mathcal{O}_{1}  & \equiv (\bar{s}_{L}^{\alpha} \gamma_{\mu}c_{L}^{\beta})(\bar{u}_{L}^{\beta}\gamma^{\mu}d_{L}^{\alpha}) = (\bar{s}_{L}\gamma_{\mu}d_{L})(\bar{u}_{L}\gamma^{\mu}c_{L})  \\
	\mathcal{O}_{2}  & \equiv (\bar{s}_{L} \gamma_{\mu} c_{L})(\bar{u}_{L}\gamma^{\mu}d_{L}),
\end{align}
$$
where the second identity in the first line comes from the [[Spinors and Chiral Theories#Fierz Identity|Fierz Identity]].
This time, we start with the effective Lagrangian 
$$
	\mathcal{L}_{4q} = \frac{4G_{F}}{\sqrt{ 2 }}V_{cs}^{*}V_{ud} \mathcal{O}_{2}.
$$
# One-loop matching
*We are going to use dimensional regularization and $\overline{MS}$*.

At higher orders in $\alpha_{S}$, other operators start contributing to the amplitude.

The matching is done by comparing the Standard Model amplitude with the EFT one, and imposing them to be equal at one-loop level.

The effective Lagrangian is 
$$
	\mathcal{L}_{\mathrm{eff}} = C_{1}(\mu)\mathcal{O}_{1}(\mu) + C_{2}(\mu)\mathcal{O}_{2}(\mu).
$$

The Standard Model amplitude and the effective amplitude are given by 
$$
	\begin{align}
	i A_{SM} &  = \frac{4G_{F}}{\sqrt{ 2 }} V_{ud}V_{cs}^{*}\left[ \left( 1 + \frac{\alpha_{S}}{4\pi} \; \frac{3}{N_{c}}\ln \frac{m_{W}^{2}}{q^{2}} \right)\langle \mathcal{O}_{2} \rangle - \frac{3\alpha_{S}}{4\pi}\ln \frac{m_{W}^{2}}{q^{2}} \langle \mathcal{O}_{1} \rangle  \right] \\
	i A_{EFT}  & = \frac{4G_{F}}{\sqrt{ 2 }}V_{ud}V_{cs}^{*}\biggl[   \left( C_{1}(\mu) \left( 1 + \frac{3\alpha_{S}}{4\pi N_{c}}\ln \frac{\mu^{2}}{q^{2}} \right) + C_{2}(\mu) \left( -\frac{3\alpha_{S}}{4\pi}\ln \frac{\mu^{2}}{q^{2}} \right) \right) \langle \mathcal{O}_{1} \rangle  \\
	& +C_{1}(\mu)\left( -\frac{3\alpha_{S}}{4\pi } \ln \frac{\mu^{2}}{q^{2}}\right) + C_{2}(\mu)\left( 1 + \frac{3\alpha_{S}}{4 \pi N_{c}}\ln \frac{\mu^{2}}{q^{2}} \right) \langle \mathcal{O}_{2} \rangle  \biggr].
	\end{align}
$$
Note that the loop in the standard model is finite, so no parameter $\mu$ is needed.
**Observation:** Electroweak loops are generally smaller than QCD corrections, since
- $\alpha_{EW} \ll \alpha_S$;
- there are factors $\frac{E^2}{m_W^2}$.
**Observation:** We still need *Lattice calculations* to find $\langle \mathcal{O}_{1} \rangle, \langle \mathcal{O}_{2} \rangle$.
## Results
At one-loop level, we find  
$$
	\begin{align}
	C_{1}(\mu)  & = - \frac{3\alpha_{S}}{4\pi}\ln \frac{m_{W}^{2}}{\mu^{2}}  \\
	C_{2}(\mu)  & = 1 + \frac{3\alpha_{S}}{4\pi N_{c}} \ln \frac{m_{W}^{2}}{\mu^{2}}.
	\end{align}
$$
This is just the result at one-loop order. We then need the RG flow equations and sum the large logs.
# Operator running
By requiring the independence of the physical amplitude from $\mu$, the RG flow equations are given by 
$$
	\mu   \frac{d}{d\mu} C_{i}(\mu) = \gamma_{ji} C_{j}(\mu),\quad \mu  \frac{d}{d\mu} \langle \mathcal{O}_{i}(\mu) \rangle \equiv \gamma_{ij} \langle O_{j}(\mu) \rangle .
$$
In our case the anomalous dimension matrix is 
$$
	\gamma_{ij} = \frac{\alpha_{S}}{4\pi}\begin{pmatrix}
	\frac{3}{N_{c}}  &  -3  \\
	-3  & \frac{3}{N_{c}}
	\end{pmatrix}.
$$
In the case of a single variable, the solution is given by 
$$
	C(\alpha) = e^{ \int_{\alpha_{0}}^{\alpha} \gamma(\alpha')/\beta(\alpha') d\alpha'} C(\alpha_{0}),
$$
and we can diagonalize the anomalous dimension matrix by looking at 
$$
	C_{\pm} = C_{1} \pm C_{2}.
$$
Using $\beta(\alpha) \approx -\beta_{0}  \frac{\alpha^{2}}{2\pi}$, we find 
$$
	C_{\pm}(\mu) = C_{\pm}(\mu_{0}) \left( \frac{\alpha(\mu)}{\alpha(\mu_{0})} \right)^{- 3 \gamma_{\pm}/\beta_{0}},
$$
with $\gamma_{\pm}$ the corresponding diagonal element in the matrix.

Now, we would like to see how the operators evolve from $m_W$ to our scale $\mu$. In our case, we have 
$$
	C_{+}(\mu) \sim \left( \frac{\alpha_{S}(\mu)}{\alpha_{S}(m_{W})} \right)^{-2/\beta_{0}},\quad C_{-}(\mu) \sim \left( \frac{\alpha_{S}(\mu)}{\alpha_{S}(m_{W})} \right)^{4/\beta_{0}} >1.
$$
Thus, at **low energy**, we have the relation 
$$
	C_{1}(\mu) \approx -C_{2}(\mu)
$$
