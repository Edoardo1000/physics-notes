*For the fermion mass generation in general, see [[Electroweak Mass Generation]].*

In the Standard Model, neutrinos are massless fermions. However, we know from experiments that **they possess mass**, although very small. Various extensions of the Standard Model have been proposed to explain why neutrinos are so *light*.

# Dirac mass term
We could just add a **mass term** to the Lagrangian 
$$
	\mathcal{L}_{l} = Y_{e} \bar{L} H e_{R} + Y_{\nu} \bar{L} H^{c}\nu_{R},
$$
with $\nu_{R}$ a particle which is a $SU(2)$ singles, has no hypercharge and no color, so **does basically nothing**. From the known Standard model parameters, we get a value of 
$$
	Y_{\nu} \sim \frac{0.1 \ \mathrm{eV}}{10^{2} \times 10^{9} \ \mathrm{ eV}} \sim 10^{-12},
$$
which is incredibly small. 

# Majorana mass term
We would like to add a mass to the neutrino without adding another field. One can try by making the neutrino a [[Spinors and Chiral Theories#Majorana Fermions|Majorana fermion]]. However, the Majorana mass term breaks the $SU(2) \times U(1)$ gauge symmetry.

To overcome this obstacle, Weinberg proposed the **dimension 5 operator** 
$$
	\mathcal{L}_{W} = \frac{c}{\Lambda} (H \epsilon L)^{T} (H\epsilon L),
$$
where $\epsilon$ is the Levi-Civita symbol. The key idea is that the operator $H_{i}\epsilon^{ij}L_{j} = H^{c{\dagger}} L$ is a singlet of every gauge symmetry of the Standard Model.
In particular, this is the only dimension 5 operator we can write in the Standard Model Effective Field Theory (SMEFT).

When the Higgs boson acquires an expectation value, the term becomes 
$$
	\frac{v^{2}}{2\Lambda} \nu_{L}^{T} \nu_{L},
$$
which is in fact a Majorana mass.

The neutrino mass gives a **bound on $\Lambda$**: 
$$
	\Lambda \sim 10^{14} \ \mathrm{eV}.
$$

# Seesaw mechanism
The Weinberg operator is just an effective description of the neutrino mass. One of the questions that arises is what is the UV completion of the theory.

A possible answer is given by adding a **very massive right neutrino** $N_{R}$.
This neutrino is a total singlet, so does not have to obey $SU(2)$ symmetry. Thus, we can make two mass terms with it:
- *a Dirac mass term:* $-Y_{\nu}\bar{L}H^{c}N_{R}$, yielding a Dirac mass $m_{D}$,
- *a Majorana mass term:* $-\frac{1}{2} M_{R} \bar{N}^{c}_{R}N_{R}$.

At this point we have a mixing matrix 
$$
	M = \begin{pmatrix}
	0 & m_{D} \\
	m_{D} & M_{R}
	\end{pmatrix},
$$
which can be diagonalized. If $M_{R}$ is very big, one of the eigenvalues gets very small, resulting in a tiny neutrino mass. 