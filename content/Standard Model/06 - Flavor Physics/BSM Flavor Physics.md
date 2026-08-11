Hints of possible new physics operators might come from the **Yukawa sector**. Indeed, the Yukawa matrices are what breaks *flavor symmetry*, so we might use the **spurion technique** to find possible new terms.
We have the transformation 
$$
	Y_{u}\to U_{q}^{\dagger}Y_{u}U_{u},\quad Y_{d} \to U_{q}^{\dagger} Y_{d}U_{d}.
$$
I now suppose that **the Yukawa matrices are fundamental fields which transform accordingly**.
The key insight was that Yukawa breaks flavor symmetry by a *small* amount, so we might guess the origin of the breaking is *dynamical*.

# Effective Lagrangian
Up to order $Y^{2}$, the effective Lagrangian may have the following operators:
$$
\begin{align}
	 &  a_{q} \; \bar{q}_{L}^{i} \gamma_{\mu} q^{i}_{L} \qquad b_{q} \; \bar{q}_{L}Y_{u}Y^{\dagger}_{u}\gamma_{\mu}q_{L} \qquad c_{q} \; \bar{q}_{L} Y_{d} Y_{d}^{\dagger} \gamma_{\mu}q_{L} \\
	 & a_{u} \; \bar{u}_{R}^{i} \gamma_{\mu} u_{R}^{i} \qquad b_{u} \; \bar{u}_{R} \gamma_{\mu} Y_{u}^{\dagger} Y_{u} u_{R}  \\
	 & a_{d} \; \bar{d}_{R}^{i} \gamma_{\mu} d_{R}^{j} \qquad b_{d} \; \bar{d}_{R} \gamma_{\mu} Y_{d}^{\dagger}Y_{d}d_{R} \qquad \tilde{b}_{d} \bar{d}_{R}  \gamma_{\mu} Y_{d}^{\dagger} Y_{u} Y_{u}^{\dagger} Y_{d} d_{R}
\end{align}
$$
Observe that the last term might not be negligible since $Y_{t} \approx 1$.

Now, we perform a *change of basis* 
$$
	Y_{d} \to \hat{Y}_{d}, \quad Y_{u} \to V_{CKM}\hat{Y}_{u},
$$
with $\hat{Y}_{d}, \hat{Y}_{u}$ diagonal.
Because of this, we have the new **flavor-changing neutral current** 
$$
	b_{q} \bar{q}_{L} V_{CKM}^{\dagger} \hat{Y}_{u}^{\dagger}\hat{Y}_{u} V_{CKM}\gamma_{\mu}q_{L}.
$$
As a result, we have the currents 
$$
	(\bar{q}_{L}^{i}\gamma_{\mu}q_{L}^{j})V_{ti}^{*}V_{tj},\qquad (d_{R}^{i}\gamma_{\mu}d_{R}^{j})m_{d_{i}} m_{d_{j}} V_{ti}^{*}V_{tj}.
$$
**Observation:** at the Standard Model level, the second operator also appears in loops. Thus, *also the flavor of right quarks changes*.

