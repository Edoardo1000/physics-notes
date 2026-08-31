# Weyl Spinors and Lorentz Representations
The Lorentz group $SO(1,3)$ algebra splits into two independent $SU(2)$ algebras. Spinors are classified by how they transform under these representations:
* **Left-handed Weyl Spinors:** $\psi^{\alpha} \in \left( \frac{1}{2}, 0 \right)$
* **Right-handed Weyl Spinors:** $\bar{\psi}^{\dot{\alpha}} \in \left( 0, \frac{1}{2} \right)$

We can build Lorentz-invariant bilinears using the antisymmetric metric tensors $\epsilon_{\alpha\beta}$ and $\epsilon_{\dot{\alpha}\dot{\beta}}$. Because spinors are Grassmann numbers (they anticommute, $\psi^\alpha \chi^\beta = - \chi^\beta \psi^\alpha$), the antisymmetric contraction is commutative:
$$
\psi \chi \equiv \psi^{\alpha} \chi^{\beta} \epsilon_{\alpha \beta} = -\chi^{\beta}\psi^{\alpha} \epsilon_{\alpha\beta} = \chi^{\alpha} \psi^{\beta} \epsilon_{\alpha\beta} = \chi \psi
$$

Similarly for the right-handed spinors: $\bar{\psi} \bar{\chi} \equiv \bar{\psi}^{\dot{\alpha}} \bar{\chi}^{\dot{\beta}} \epsilon_{\dot{\alpha} \dot{\beta}}$.

# Helicity and Chirality

Helicity and chirality appear to be very similar concepts. However, they are not the same, and must not be confused.
- **Helicity:** the projection of the spin along momentum
  $$
  	h = \frac{\vec{S} \cdot \vec{p}}{\lvert \vec{p} \rvert }
  $$
- **Chirality:** this is based on the eigenvalues of $\gamma_{5}$.  A spinor decomposes as $\psi = \psi_{L} + \psi_{R}$, with
  $$
  	\gamma_{5}\psi_{L / R} = \mp \psi_{L / R}.
  $$
Now, for massless particles, the concepts are similar, but signs change for the case of antiparticles. Thus, we have 

|              | Particle         | Antiparticle     |
| ------------ | ---------------- | ---------------- |
| left chiral  | $h=-\frac{1}{2}$ | $h=+\frac{1}{2}$ |
| right chiral | $h=+\frac{1}{2}$ | $h=-\frac{1}{2}$ |

# Dirac Spinors and Charge Conjugation
A 4-component Dirac spinor is built using a left-handed and a right-handed Weyl spinor:
$$
\psi = \begin{pmatrix} \chi_{\alpha} \\ \bar{\lambda}^{\dot{\alpha}} \end{pmatrix}
$$

**Charge Conjugation** maps a fermion to its antifermion. On Dirac spinors, it is defined as:
$$
\psi^{c} \equiv i \gamma^{2} \gamma_{0} \bar{\psi}^{T}
$$
*(Note: In the Weyl basis, $\sigma^{2}_{\alpha \beta} = -i \epsilon_{\alpha\beta}$)*. 

Applying this to our stacked Dirac spinor, it flips and swaps the chiral components:
$$
\psi^{c} = \begin{pmatrix} \lambda_{\alpha} \\ \bar{\chi}^{\dot{\alpha}} \end{pmatrix}
$$
The overall effect is the exchange $\chi \leftrightarrow \lambda$.

# Vector-like vs. Chiral Theories

Spinor theories are classified in:
* **Vector-like Theory:** If a theory contains a left-handed spinor in representation $R$, it contains a right-handed spinor in the exact same representation $R$. 
  * *Example:* **QCD** is vector-like. Both $q_L$ and $q_R$ are color triplets.
* **Chiral Theory:** Left and right-handed fields transform under *different* gauge representations.
  * *Example:* The **Electroweak Theory** is chiral. $Q_L$ is an $SU(2)$ doublet, while $u_R$ and $d_R$ are $SU(2)$ singlets.

# Fierz Identity
When calculating scattering amplitudes, the **Fierz identity** can sometimes come in handy: 
$$
	\bar{A}_{L}\gamma_{\mu}B_{L} \ \bar{C}_{L}\gamma^{\mu}D_{L} = - \bar{A}_{L}\gamma_{\mu}D_{L} \ \bar{C}_{L}\gamma^{\mu}B_{L}, 
$$
where $A,B,C,D$ are all *commuting* spinors. In the case of anticommuting ones, there is an extra minus sign.

# Nonrelativistic Limit
To get the nonrelativistic limit of spinors, we must look at the Dirac equation, written in the form 
$$
	(\vec{\alpha} \cdot \vec{p} + \beta m)\psi = E \psi,
$$
with 
$$
	\alpha = \begin{pmatrix}
	0  & \vec{\sigma} \\
	\vec{\sigma}  & 0
	\end{pmatrix},\quad
	\beta = \begin{pmatrix}
	m  & 0 \\
	0 & m
	\end{pmatrix}.
$$
*Also take a look at [[Gamma Matrices]]*.

Writing the energy as the rest mass plus a small contribution, we find 
$$
	\chi \approx \frac{\vec{\sigma} \cdot \vec{p}}{2m}\phi.
$$
From this, we can derive the vector and axial currents $J_{V}^{\mu}, J_{A}^{\mu}$: 
$$
	J_{V}^{\mu} \approx \begin{pmatrix}
	\phi ^{\dagger} \phi \\ \phi ^{\dagger} \frac{\vec{p}}{m} \phi
	\end{pmatrix}, \quad 
	J_{A}^{\mu} \approx \begin{pmatrix}
	\phi ^{\dagger} \frac{\vec{\sigma} \cdot \vec{p}}{m} \phi\\ \phi ^{\dagger}\vec{\sigma} \phi
	\end{pmatrix}.
$$
# Majorana Fermions
A Majorana fermion is a fermion which is its own conjugate: $\chi^{c} = \chi$. Majorana fermions can have a mass term 
$$
	\mathcal{L}_{M} = -\frac{1}{2} m_{M} (\bar{\chi}^{c} \chi + \mathrm{h.c.}).
$$