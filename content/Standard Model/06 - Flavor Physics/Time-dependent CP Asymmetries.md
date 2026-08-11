Suppose we have a meson in which we know its flavor at $t=0$. If the meson *mixes* over time with its antimatter correspondent, we should see **oscillations** in decay time.
Consider a meson starting in the state $M^{0}$, and consider the process (for simplicity, suppose $\bar{f} = f$) 
$$
	M^{0}\to f, \quad \bar{M}^{0} \to M^{0} \to f.
$$
We can take a look at the observable
$$
	A_{CP}(t) \equiv \frac{\Gamma(\bar{M}^{0}(t)\to f) - \Gamma(M^{0}(t))\to f}{\Gamma(M^{0}(t)\to f)+\Gamma(M^{0}(t)\to f)},
$$
since now the particle evolves in time. After some calculations we find
$$
\begin{align}
 A_{CP}(t)  &  = \frac{2(1-\lvert \lambda_{f} \rvert ^{2})\cos \Delta\omega t - 2 \mathrm{Im}\lambda_{f} \sin \Delta\omega t}{1 + \lvert \lambda_{f} \rvert ^{2}} \equiv  \\
  & \equiv C_{f} \cos \Delta\omega t - S_{f} \sin \Delta\omega t
\end{align},
$$
with 
$$
\lambda_{f} \equiv \frac{\bar{A}_{f}}{A_{f}} \frac{q}{p},\quad A_{f} = \braket{ M^{0} | f },\quad \bar{A}_{f} = \braket{ \bar{M}^{0} | f } .
$$

>[!math]- Derivation: formula for $A_{CP}(t)$
>Our initial state evolves according to
>$$
>\begin{align} \ket{M^{0}(t)}   & = \frac{1}{2p}(e^{ i\omega_{L}t }\ket{M_{L}}  + e^{ i \omega_{H}t }\ket{M_{H}} ) \\ & = \frac{1}{2p} (e^{ i \omega_{L} t }(p \ket{M^{0}} +q\ket {\bar{M}^{0}}) + e^{ i \omega_{H}t }(p \ket{M^{0}- q} \ket{\bar{M}^{0}}  )). \end{align}.
>$$
>The amplitudes in function of time are thus given by
> $$
> \begin{align} \lvert \braket{ M^{0}(t) | f }  \rvert^{2}  & \sim \frac{1}{4}\lvert e^{ i \omega_{L}t } + e^{ i\omega_{H}t } + \lambda_{f} (e^{ i \omega_{L}t } - e^{ i \omega_{H}t })^{2} \rvert  \\ \lvert \braket{ \bar{M}^{0}(t) | f }  \rvert^{2}  & \sim \frac{1}{4}\lvert e^{ i \omega_{L}t } - e^{ i\omega_{H}t } + \lambda_{f} (e^{ i \omega_{L}t } + e^{ i \omega_{H}t })^{2} \rvert  \end{align}.
> $$
>We observe that
>- pieces with $|\lambda|^2$ indicate direct or indirect CP violation;
>- pieces with $\lambda$ indicate interference between the two.
>Now we just have to expand the absolute value squared and plug it into the formula for $A_{CP}$.

#### Example: B decay as a function of time
I can measure the time-dependent interference between the processes
$$
	B_{d}^{0}\to J /\psi + K_{S},\quad B_{d}^{0}\to \bar{B}_{d}^{0} \to J / \psi + K_{S}
$$
where I can measure the interference with the mixing $B^{0} \leftrightarrow \bar{B}^{0}$. It is a 1-loop process.

I get the triangle angle 
$$
	\beta = \mathrm{Arg}\left( - \frac{V_{cd}V_{cb}^{*}}{V_{td}V_{tb}^{}} \right)
$$
and also 
$$
	\mathrm{Im}\lambda_{\psi K} = \sin 2\beta = \delta_{J / \psi}
$$