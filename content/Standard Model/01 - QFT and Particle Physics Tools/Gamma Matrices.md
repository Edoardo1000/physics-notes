The gamma matrices are a representation of the Clifford algebra.
They obey the anticommutation relations 
$$
	\{ \gamma_{\mu}, \gamma_{\nu} \} = 2\eta_{\mu \nu}.
$$
We define the fifth gamma matrix as 
$$
	\gamma^{5} \equiv i \gamma^{0} \gamma^{1}\gamma^{2}\gamma^{3}
$$
There are two basis in which the matrices are usually written:
- **Weyl basis:** this is more suited for the relativistic limit. We have 
  $$
  	\gamma^{0} = \begin{pmatrix}
	0 & I \\
	I & 0
	\end{pmatrix}, \quad 
	\gamma^{i} = \begin{pmatrix}
	0 & \sigma^{i} \\
	-\sigma^{i} & 0
	\end{pmatrix}, \quad
	\gamma^{5} = \begin{pmatrix}
	I & 0 \\
	0 & -I
	\end{pmatrix}.
  $$
  - **Dirac basis:** this is best used in the context of nonrelativistic fermions. The matrices are defined as 
    $$
    	\gamma^{0} = \begin{pmatrix}
		I & 0 \\
		0 & -I
		\end{pmatrix},\quad
		\gamma^{i} = \begin{pmatrix}
		0 & \sigma^{i} \\
		-\sigma^{i} & 0
		\end{pmatrix},\quad
		\gamma^{5} = \begin{pmatrix}
		0 & I  \\
		I & 0
		\end{pmatrix}.
    $$
    
## Trace Identities

For two vectors $a_{\mu}, b_{\mu}$,  we have the following identities:
- $\mathrm{Tr}[\not\!{a}\gamma^{\mu}\not\!{b}\gamma^{\nu}] = 4(a^{\mu}b^{\nu}+a^{\nu}b^{\mu}-(a\cdot b)\eta^{\mu \nu})$
- $\mathrm{Tr}[\not\!{a}\gamma^{\mu}\not\!{b}\gamma^{\nu}\gamma^{5}] = -4i \epsilon^{\mu \rho \nu \sigma}a_{\rho} b_{\sigma}$