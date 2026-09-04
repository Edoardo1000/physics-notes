---
tags:
  - topic/BSM
---
# Heavy New Physics
If $\Lambda_{\mathrm{NP}} \gg m_{W}$, the important data comes from a **quantum effective action**: 
$$
	S_{eff} = \frac{1}{2} \int \frac{d^{4}q}{(2\pi)^{4}}W^{a}_{\mu}(-q^2) \Pi^{\mu \nu}_{ab}(q^{2})W^{b}_{\nu}(q^{2}),
$$
where $a,b = 1,2,3,B$, and $\Pi^{\mu \nu}_{ab}$ are the propagators after the corrections coming from possible BSM heavy particles.
**Our only hypothesis is that there is an unbroken $U(1)_{\mathrm{em}}$.**

Since we are interested in energy far *below the new physics scale*, we can *expand the propagators* 
$$
	\Pi_{ab}^{\mu \nu}(q^{2})= \eta^{\mu \nu} \Pi_{ab}(q^{2}) + q^{\mu}q^{\nu}(\dots), \quad \Pi_{ab}(q^{2}) \approx \Pi_{ab}(0) + q^{2}\Pi'_{ab}(0),
$$
where the $(\dots)$ is not relevant for our analysis, we are mainly interested in the transverse part.

The physical interpretation of the terms is:
	-  $\Pi_{ab}(0)$ is the mass of the particles
	- $\Pi'_{ab}(0)$ dictates the coefficients in the kinetic terms of the particles
## Constraints
The parameters are not free, since I have to reproduce SM operators at low energy.

#### Massless photon
since the photon remains massless, after [[Electroweak Mass Generation|spontaneous symmetry breaking]] the photon must remain massless and it cannot have a mixing with the $Z$:
$$
	\Pi_{\gamma\gamma}(0) = 0,\quad \Pi_{\gamma Z}(0) = 0.
$$
This can be translated in a relation between $\Pi_{33}(0), \Pi_{BB}(0), \Pi_{B{3}}(0)$. 

Now, we also need the condition that the vacuum is uncharged, $Q\ket{0} = 0$. This implies the condition  
$$
	\begin{pmatrix}
	\Pi_{33}(0) & \Pi_{3B}(0)  \\
	\Pi_{3B}(0) & \Pi_{BB}(0)
	\end{pmatrix} \propto 
	v^{2} \begin{pmatrix}
	g^{2} & -gg' \\
	-gg' & g'^{2}
	\end{pmatrix},
$$
which fixes our parameters. Define the value
$$
\Pi_{ZZ} \equiv \frac{\Pi_{33}(0)}{c_{W}^{2}} = \frac{\Pi_{BB}(0)}{s_{W}^{2}}.
$$

>[!math]- Derivation:  Form of the mass matrix
> Suppose that we do not know how the bosons get their mass, but suppose that BSM particles couple through the constants $g,g'$. Write 
> $$
> T_{a} = (T_{3},Y), \quad g_{a} = (g,g') .
> $$
> The mass matrix will have the general form 
> $$
> (M^{2})_{ab} = g_{a}g_{b}K_{ab},
> $$
> where $K_ab$ measures how the generators are broken. The matrix can also be interpreted as 
> $$
> K_{ab} \sim \braket{ T_{a} | T_{b} },\quad \ket{T_{a}} \equiv T_{a}\ket{0} .
> $$
> Now, let 
> $$
> x_{a} = \frac{1}{g_{a}},
> $$
>and let us apply $M^2$ to it:
>$$
>(M^{2}x)_{a} = g_{a} \sum_{b}g_{b}K_{ab},
>$$
>but 
>$$
>\sum_{b}K_{ab}\sim \bra{T_{a}} (T_{3} + Y)\ket{0}  = \bra{T_{a}}Q\ket{0} =0.
>$$
>Thus, we have found 
>$$
>M^{2} \begin{pmatrix} g' \\ g \end{pmatrix} = 0,
>$$
>which proves our statement.

### Parameters
- **Zero order:** originally, we had $\Pi_{WW}(0), \Pi_{33}(0),\Pi_{3B}(0),\Pi_{BB}(0)$. After the constraints, only two of them are independent. Their mismatch indicates [[Sigma Model for Higgs]] breaking, and we define
  $$
  	T \equiv \frac{\Pi_{33}-\Pi_{WW}}{m_{W}^{2}}.
  $$
  - **Order $q^{2}$:** out of four possible derivatives, two are absorbed by field normalization. There remain the combinations 
    $$
    	\begin{align}
		U  & \equiv\Pi_{33}'(0) - \Pi'_{WW}(0) \\
		S  & \equiv \frac{g}{g'}\Pi_{3B}'(0)
		\end{align}
    $$

They are useful because they measure how loops alter the symmetry structure.

Here is a table with some parameters and the symmetries they preserve (all the propagators and derivatives are calculated at $q^{2}=0$):

| Parameter | Expression              | $SU(2)_{L} \times SU(2)_{R}$ | $SU(2)_{L} \times U(1)_{\mathrm{em}}$ |
| --------- | ----------------------- | ---------------------------- | ------------------------------------- |
| $T$       | $\Pi_{33}-\Pi_{WW}$     | no                           | no                                    |
| $U$       | $\Pi_{33}'-\Pi'_{WW}$   | no                           | no                                    |
| $S$       | $\Pi'_{3B}$             | yes                          | no                                    |
| $V$       | $\Pi''_{33}-\Pi''_{WW}$ | no                           | no                                    |
| $X$       | $\Pi''_{3B}$            | yes                          | no                                    |
| $W$       | $\Pi'_{WW}$             | yes                          | yes                                   |
| $Y$       | $\Pi''_{BB}$            | yes                          | yes                                   |
The most important parameters are $T,S,W,Y$. LEP1 could only detect $S,T,U$.

# Corrections from composite Higgs
*Take a look at [[Composite Higgs]].*

If we have the bigger symmetry group $SO(5)$, there are two possible contributions coming from UV physics:
$$
	\mathcal{L}_{UV} = \frac{1}{2}\left( \eta_{\mu \nu} - \frac{q_{\mu}q_{\nu}}{q^{2}} \right)[\Pi_{0}(q^{2})\mathrm{Tr}(A_{\mu}A_{\nu})+ \Pi_{1}(q^{2})\Sigma ^{\dagger}A_{\mu}A_{\nu}\Sigma],
$$
where we packed the various gauge vectors as 
$$
	A_{\mu} = gW_{\mu}^{a}T^{a}_{L} + g' B_{\mu}T^{3}_{R}.
$$
