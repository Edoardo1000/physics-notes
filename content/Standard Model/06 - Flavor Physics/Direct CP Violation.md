**Note:** here, the bar stands for *both conjugation and parity transformation*.

---
We need variables which are **sensitive to the phase**, I need some amplitudes:
$$
	\begin{align}
	A_{f}  & = A(i\to f),\quad \bar{A}_{f} = A(\bar{i}\to f),  \\
	A_{\bar{f}}  & = A(i\to \bar{f}),\quad \bar{A}_{\bar{f}}=A(\bar{i}\to \bar{f})
	\end{align}
$$
We have **CP violation** only if 
$$
	\left\lvert  \frac{\bar{A}_{\bar{f}}}{A_{f}}  \right\rvert \neq 1.
$$
An observable which might help us identify CP violation is thus
$$
	A_{CP}  = \frac{\Gamma(\bar{i}\to \bar{f})-\Gamma(i\to f)}{\Gamma(\bar{i}\to \bar{f})+ \Gamma(i \to f)} = \frac{\lvert \bar{A}_{\bar{f}} \rvert ^{2} -\lvert A_{f} \rvert^{2}}{\lvert \bar{A}_{\bar{f}} \rvert^{2} + \lvert A_{f} \rvert^{2} }.
$$
Now, the amplitudes have various contributions depending on the process. Schematically, we may write
$$
	A_{f} = \sum_{k} a_{k}e^{ i\delta_{k} } e^{ i \phi_{k}} \implies \bar{A}_{\bar{f}} = \sum_{k} a_{k} e^{ -i \phi_{k} } e^{ i \delta_{k} },
$$
where:
- $\phi_k$ is called the **weak phase**. It usually comes from complex couplings in the Lagrangian, such as the CKM matrix, and *changes sign* under CP;
- $\delta_k$ is called the **strong phase**. Usually comes from strong processes, such as intermediate particles going on-shell. Since strong interactions are CP invariant, the angle *does not change sign*.
If we have for example two processes contributing to the amplitude, we find
$$
	A_{CP} = \frac{-2 a_{1} a_{2} \sin(\delta_{1}-\delta_{2}) \sin(\phi_{1}-\phi_{2})}{\lvert a_{1} \rvert ^{2} + \lvert a_{2} \rvert ^{2} + 2 \lvert a_{1} a_{2} \rvert \cos(\delta_{1}-\delta_{2})\cos(\phi_{1}-\phi_{2})}.
$$
**Observation:** In order to measure CP violation, *I need both $\phi_{1} \neq \phi_{2}$ and $\delta_{1} \neq \delta_{2}$*.

