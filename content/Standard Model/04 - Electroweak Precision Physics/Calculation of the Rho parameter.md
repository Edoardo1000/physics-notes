
We work in the scheme $\{ G_{F}, m_{Z}, \alpha \}$. Moreover, we will use the *on-shell renormalization scheme*. In our context, the physical values 
$$
	v^{2} = \frac{1}{\sqrt{ 2 }G_{F}},\quad g_{Z} \equiv \frac{g}{2c_{W}} = (\sqrt{ 2 } G_{F}m_{Z}^{2})^{1/2}
$$
are considered fixed.
Now, we have $g_{A}^{eff} = g_{A}\left( 1 + \frac{1}{2} \Delta \rho \right)$. Thus, the axial part of the effective vertex goes like 
$$
	\mathcal{V}_{A} = g_{Z} g_{A} \left( 1 + \frac{1}{2} \Delta \rho  \right).
$$
#### Comparison
To compare with the 1-loop amplitude, start from the bare Lagrangian 
$$
	\mathcal{L}_{B} = g_{Z 0} Z_{0 \mu} \psi_{0} \gamma^{\mu} (g_{V 0} - g_{A}\gamma_{5})\psi_{0},
$$
(notice that $g_{A}$ is just an integer, so it does not renormalize) and we do the substitution 
$$
	Z_{0 \mu} = \sqrt{ Z_{Z} }Z_{\mu},\quad \psi_{0} = \sqrt{ Z_{f} }\psi, \quad g_{Z,V,A 0} = g_{Z,V} + \delta g_{Z,V},
$$
From this substitution we find the physical tree vertex 
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
For a charged lepton, $g_{A} = -\frac{1}{2}$, so we arrive to the relation 
$$
	\Delta \rho = 2 \frac{\delta g_{Z}}{g_{Z}} + \delta Z_{Z} - 4 \Delta g_{A}.
$$
We now substitute the renormalization conditions due to the on-shell scheme:

#### Renormalization conditions
 Even though $v, m_{Z}, g_{Z}$ are fixed, their bare counterparts have counterterms $\delta v, \delta m_{Z}^{2},\delta g_{Z}$. Moreover, we have 
$$
	m_{Z,0}^{2} = g_{Z,0}^{2} v_{0}^{2} \implies 2 \frac{\delta g_{Z}}{g_{Z}} =  \frac{\delta m_{Z}^{2}}{m_{Z}^{2}} - 2 \frac{\delta v}{v}.
$$
Muon decay also fixes $\delta v$: at one-loop level, the decay amplitude is 
$$
	A_{\mu} = \frac{1}{2v^{2}}\left[ 1 - 2 \frac{\delta v}{v} - \frac{\Pi_{WW}(0)}{m_{W}^{2}} + \frac{\delta G_{F}^{V+B}}{G_{F}} \right],
$$
where $\delta G_{F}^{V+B}$ represents corrections such as 1PI vertex diagrams, box diagrams and so on. Since it should correspond to the fixed value $\frac{G_{F}}{\sqrt{ 2 }} = \frac{1}{2v^{2}}$, we must have 
$$
	2 \frac{\delta v}{v} = - \frac{\Pi_{WW}(0)}{m_{W}^{2}} + \frac{\delta G_{F}^{V+B}}{G_{F}}.
$$
Now, the other renormalization conditions also impose
- $\delta m_{Z}^{2} + \Pi_{Z Z}(m_{Z}^{2}) = 0$;
- $\delta Z_{Z} = \Pi'(m_{Z}^{2})$.
Putting all together, we find 
$$
	\Delta \rho = - \frac{\delta G_{F}^{V+B}}{G_{F}} + \frac{\Pi_{WW}(0)}{m_{W}^{2}} - \frac{\Pi_{Z Z}(m_{Z}^{2})}{m_{W}^{2}} + \Pi_{Z Z}'(m_{Z}^{2}) - 4 \Delta g_{A}.
$$
Writing  
$$
\Pi_{Z Z}(q^{2}) = \Pi_{ZZ}(0) + q^{2} F_{ZZ}(q^{2}),\quad\Pi_{ZZ}'(q^{2}) = F_{Z Z}(q^{2}) +q^{2} F'_{Z Z}(q^{2}),
$$
we find our final result 
$$
	\Delta \rho = -\frac{\Delta G_{F}^{V + B}}{G_{F}} + \left( \frac{\Pi_{WW}(0)}{m_{W}^{2}} - \frac{\Pi_{Z Z}(0)}{m_{Z}^{2}}\right) + m_{Z}^{2} F_{Z Z}'(m_{Z}^{2}) - 4 \Delta g_{A}
$$
# Calculation of the loops
