---
tags:
  - type/derivation
---
We work in the scheme $\{ G_{F}, m_{Z}, \alpha \}$. Moreover, we will use the *on-shell renormalization scheme*. In our context, the physical values 
$$
	v^{2} = \frac{1}{\sqrt{ 2 }G_{F}},\quad g_{Z} \equiv \frac{g}{2c_{W}} = (\sqrt{ 2 } G_{F}m_{Z}^{2})^{1/2}
$$
are considered fixed.

For the calculation of $\Delta \rho_{f}$, it is sufficient to look at the axial part of the effective vertex. Given $g_{A}^{eff} = g_{A}\left( 1 + \frac{1}{2} \Delta \rho \right)$, this has the form
$$
	\mathcal{V}_{A} = g_{Z} g_{A} \left( 1 + \frac{1}{2} \Delta \rho  \right).
$$
## One-loop amplitude
To find with the 1-loop amplitude, we are going to use renormalized perturbation theory. We start from the bare Lagrangian 
$$
	\mathcal{L}_{B} = g_{Z 0} Z_{0 \mu} \psi_{0} \gamma^{\mu} (g_{V 0} - g_{A}\gamma_{5})\psi_{0},
$$
(notice that $g_{A}$ is just an integer, so it does not renormalize) and do the substitution 
$$
	Z_{0 \mu} = \sqrt{ Z_{Z} }Z_{\mu},\quad \psi_{0} = \sqrt{ Z_{f} }\psi, \quad g_{Z,V,A 0} = g_{Z,V} + \delta g_{Z,V}.
$$
We thus have the physical tree vertex 
$$
	\mathcal{L}_{\mathrm{tree}} = g_{Z} Z_{\mu} \psi \gamma^{\mu}(g_{V}-g_{A}\gamma_{5})\psi,
$$
where the couplings and the fields are now the physical ones, plus some counterterms 
$$
	\mathcal{L}_{CT} = \mathcal{L}_{tree} \left[ \frac{\delta g_{Z}}{g_{Z}} + \frac{1}{2} \delta Z_{Z} + \delta Z_{f} \right] + g_{Z} Z_{\mu}\bar{\psi}\gamma^{\mu}\delta g_{V}\psi.  
$$
Now, let's look at the interaction vertex at 1-loop level, more specifically the axial part: 
$$
	A_{A} = g_{Z}\left[   g_{A} + g_{A}\left( \frac{\delta g_{Z}}{g_{Z}} + \frac{1}{2} \delta Z_{Z} \right) + A_{\mathrm{loop}} + g_{A}\delta Z_{f}\right].
$$
Comparing with the effective vertex, we find 
$$
	\Delta \rho = 2 \frac{\delta g_{Z}}{g_{Z}} + \delta Z_{Z} + 2 \frac{\Delta g_{A}}{g_{A}},\quad \Delta g_{A} \equiv A_{\mathrm{loop}} + g_{A}\delta Z_{f}.
$$
For a charged lepton, $g_{A} = -\frac{1}{2}$, thus we have
$$
	\Delta \rho = 2 \frac{\delta g_{Z}}{g_{Z}} + \delta Z_{Z} - 4 \Delta g_{A}.
$$
We now have to write explicitly the counterterms, which are determined by our on-shell renormalization condition.
## Renormalization conditions
 While $v, m_{Z}, g_{Z}$ are fixed, their bare counterparts possess the counterterms $\delta v, \delta m_{Z}^{2},\delta g_{Z}$. They are linked by the relation
$$
	m_{Z,0}^{2} = g_{Z,0}^{2} v_{0}^{2} \implies 2 \frac{\delta g_{Z}}{g_{Z}} =  \frac{\delta m_{Z}^{2}}{m_{Z}^{2}} - 2 \frac{\delta v}{v}.
$$
Muon decay also fixes $\delta v$: at one-loop level, the decay amplitude is 
$$
	A_{\mu} = \frac{1}{2v^{2}}\left[ 1 - 2 \frac{\delta v}{v} - \frac{\Pi_{WW}(0)}{m_{W}^{2}} + \frac{\delta G_{F}^{V+B}}{G_{F}} \right],
$$
where $\delta G_{F}^{V+B}$ represents corrections such as 1PI vertex diagrams, box diagrams and so on. Since it should correspond to the physical value $\frac{G_{F}}{\sqrt{ 2 }} = \frac{1}{2v^{2}}$, we must have 
$$
	2 \frac{\delta v}{v} = - \frac{\Pi_{WW}(0)}{m_{W}^{2}} + \frac{\delta G_{F}^{V+B}}{G_{F}}.
$$
Now, the other renormalization conditions also impose
- $\delta m_{Z}^{2} + \Pi_{Z Z}(m_{Z}^{2}) = 0$;
- $\delta Z_{Z} = \Pi'(m_{Z}^{2})$.
Putting all together, we find 
$$
	\Delta \rho_{f} = - \frac{\delta G_{F}^{V+B}}{G_{F}} + \frac{\Pi_{WW}(0)}{m_{W}^{2}} - \frac{\Pi_{Z Z}(m_{Z}^{2})}{m_{W}^{2}} + \Pi_{Z Z}'(m_{Z}^{2}) - 4 \Delta g_{A}.
$$
Writing  
$$
\Pi_{Z Z}(q^{2}) = \Pi_{ZZ}(0) + q^{2} F_{ZZ}(q^{2}),\quad\Pi_{ZZ}'(q^{2}) = F_{Z Z}(q^{2}) +q^{2} F'_{Z Z}(q^{2}),
$$
we find our final result 
$$
	\Delta \rho_{f} = -\frac{\Delta G_{F}^{V + B}}{G_{F}} + \left( \frac{\Pi_{WW}(0)}{m_{W}^{2}} - \frac{\Pi_{Z Z}(0)}{m_{Z}^{2}}\right) + m_{Z}^{2} F_{Z Z}'(m_{Z}^{2}) - 4 \Delta g_{A}.
$$
Now, the relevant part is the one in parentheses. Using that $c_{W}^{2} \Pi_{Z Z}(0) = \Pi_{33}(0)$ (the photon cannot mix at $q^{2}=0$), we have 
$$
	\Delta \rho_{f} \approx \frac{1}{m_{W}^{2}}(\Pi_{33}(0)-\Pi_{WW}(0))
$$
# Calculation of the loops
