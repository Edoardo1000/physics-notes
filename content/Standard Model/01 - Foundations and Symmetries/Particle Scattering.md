Consider the scattering of two particles $p_{1} + p_{2} \to X$ in many different products. We put ourselves in the center of mass frame, so that we have $\lvert \vec{p}_{1} \rvert=\lvert \vec{p}_{2} \rvert \equiv p_{i}$.

For two particles scattering in many products, their **differential cross section** is given by 
$$
	d\sigma = \frac{1}{4E_{1}E_{2}\lvert \vec{v}_{1} - \vec{v}_{2} \rvert } \lvert A \rvert ^{2} d\Phi_{n},
$$
where $d\Phi_{n}$ is the $n$-particle **phase space element**, given by 
$$
	d\Phi_{n} \equiv \delta^{4}\left( p_{1}+p_{2} - \sum_{i}p_{i} \right)\prod_{i} \frac{d^{3}p}{(2\pi)^{3}} \frac{1}{2E_{i}}.
$$
We also have the identity 
$$
	\lvert \vec{v}_{1}-\vec{v}_{2} \rvert = \left\lvert  \frac{\lvert \vec{p}_{1} \rvert }{E_{1}} + \frac{\lvert \vec{p}_{2} \rvert }{E_{2}}  \right\rvert = {p}_{i} \frac{\sqrt{ s }}{E_{1} E_{2}}.
$$

### Two-particle scattering

For the case of two particles $p_{1} + p_{2} \to p_{3} + p_{4}$. In this case the phase space element is given by
$$
	d\Phi_{2} = \frac{1}{16\pi^{2}} d\Omega   \frac{p_{f}}{\sqrt{ s }}\theta(E_{CM}-m_{3}-m_{4}),
$$
where $p_{f} = \lvert \vec{p}_{3} \rvert =\lvert \vec{p}_{4} \rvert$ in the center-of-mass frame.
From this we derive the formula 
$$
	\left( \frac{d\sigma}{d\Omega} \right)_{CM} = \frac{1}{64\pi^{2} s} \frac{p_{f}}{p_{i}}\lvert A \rvert ^{2}\theta(\sqrt{ s }-m_{3}-m_{4}).
$$
Which for the case of equal masses simplifies to 
$$
	\left( \frac{d\sigma}{d\Omega} \right)_{CM} = \frac{1}{64\pi^{2}s}\lvert A \rvert ^{2}
$$