### Parameters
The CKM matrix is not generic, and possesses some constraints which reduce the number of its free parameters. In particular, the free parameters are
- **$\frac{N(N-1)}{2}$ angles**,
- **$\frac{(N-1)(N-2)}{2}$ phases**.

>[!math]- Derivation: CKM matrix free parameters
>A generic complex $N \times N$ matrix possesses $2N^{2}$ free parameters. However, unitarity halves the free parameters to $N^{2}$.
>A matrix can be decomposed in a symmetric and an antisymmetric part: the antisymmetric one represents the angles of rotation, and there are $\frac{N(N-1)}{2}$ possible angles.
>The symmetric part represents multiplication by a phase, but it must be kept in mind that not all phases are physical. In particular, we can rotate quarks by phase factors, and the CKM matrix changes according to 
>$$
>V^{ij}_{\mathrm{CKM}} \to e^{ -i\theta_{i} }V^{ij}_{\mathrm{CKM}}e^{ i\phi_{j} }.
>$$
>Since there are $2N$ quarks, we can rotate away $2N-1$ complex phases (the $-1$ appears because the rotation in which all angles are equal, Baryon Number symmetry, does not change the matrix). The phases are thus 
>$$
>\frac{N(N+1)}{2} - 2N + 1 = \frac{(N-1)(N-2)}{2} 
>$$

In particular, the CKM matrix for three flavor possesses **three angles and one phase**.

We parametrize the matrix by
$$
	V_{CKM} = R_{12}(\theta_{12})R_{13}(\theta_{13}, e^{ i\delta })R_{23}(\theta_{23}),
$$
and the phase was put with $\theta_{13}$ because it's the smallest angle, so there are less cancellations. We have 
$$
	R_{13}(\theta_{13},e^{ i\delta }) = \begin{pmatrix}
	\cos\theta_{13} &  & \sin \theta_{13} e^{ -i\delta } \\
	 & 1 &  \\
	 -\sin \theta_{13}e^{ i\delta }  &  & \cos\theta_{13}
	\end{pmatrix},
$$
and we have 
$$
	\theta_{12} \sim 10^{-1},\quad \theta_{13} \sim 10^{-3}, \quad \theta_{23}\sim {10}^{-2}.
$$
*We do not know why the angles behave like this.*
### Wolfenstein parametrization
We define 
$$
\begin{align}
	\sin\theta_{12}& \equiv \lambda  \sim 0.2,  \\
	\sin\theta_{23}  & \equiv \lambda^{2}A,  \\
	\sin\theta_{13}  & \equiv A\lambda^{3}(\rho-i \eta),
\end{align}
$$
from which the matrix now takes the form (at leading order)
$$
	V_{CKM} \sim \begin{pmatrix}
	1  & \lambda  & \lambda^{3}  \\
	\lambda & 1 & \lambda^{2} \\
	\lambda^{3} & \lambda^{2} & 1
	\end{pmatrix}.
$$
