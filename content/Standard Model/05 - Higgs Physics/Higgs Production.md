The direct method, using $e \bar{e}$ collisions, is not sufficient due to the value of $Y_{e}$ being to small.

One could produce a couple of tops, and one emits the Higgs, but they are too massive.

### Higgs  Strahlung
The best route is 
$$
	e+\bar{e}\to Z + h,
$$
with cross section given by 
$$
	\sigma \sim \frac{1}{2s} (g_{V}^{2} + g_{A}^{2})\left( \frac{2m_{Z}^{2}}{v} \right)^{2} \frac{1}{(s-m_{Z}^{2})^{2}} \frac{s}{m_{Z}^{2}} \frac{s}{8\pi} \sqrt{ 1-\frac{4m^{2}}{s} }.
$$
This expression has the correct $\frac{1}{s}$ behavior at infinity.

### Vector Fusion
The electrons emit bosons which annihilate and create an Higgs.
Due to the $g^{2}$, it seems less relevant. However, we are in the t-channel, so that the propagator factor has $t \sim -\frac{s}{2}(1-\cos\theta)$, which vanishes for *collinear final particles*. The resulting $h$ is **soft**.

We can find the cross section using the [[Parton Method]]. We arrive at the final result
$$
    \sigma \sim \frac{g^{4}}{256 \pi^{3}v^{2}}\left[\log\left( \frac{s }   {m_{h}^{2}} \right) - 1 \right].
$$
>[!math]- Derivation: Vector fusion cross section
>In this case we have to use the parton method twice, once for each electron. If $x_1,x_2$ are the fractions of the electron and positron momenta carried by the vectors $V(k_1), V(k_2)$, their invariant mass $\hat{s}$ is given in the collinear limit by
>$$
>\hat{s} = (k_{1}+k_{2})^{2} \simeq x_{1} x_{2} s.
>$$
>Applying the parton method we have (suppose identical splitting functions for simplicity)
>$$
>\sigma(e \bar{e} \to f \bar{f} H) = \sum_{\lambda_{1}, \lambda_{2}} \int_{0}^{1}dx_{1} \int_{0}^{1} f_{V}(x_{1}) f_{V}(x_{2})\hat{\sigma}_{\lambda_{1}\lambda_{2}}(x_{1}x_{2}s)
>$$
>For the cross section $\hat{\sigma}$, we have
>$$
>\hat{\sigma} = \frac{1}{2\hat{s}} \lvert A \rvert ^{2} \int d\Phi_{1} = \frac{\pi}{m_{h}^{2}}\lvert A \rvert ^{2} \delta(\hat{s} - m_{h}^{2}),
>$$
> with $d\Phi_1$ the one-element phase space element.
> The amplitude is found to be (average over polarizations)
> $$
> \lvert \bar{A} \rvert ^{2} \approx \frac{m_{h}^{4}}{v^{2}}.
> $$
> *Also take a look at [[Higgs Boson Decay]].*
>Now, putting everything together, we have 
>$$
>\begin{align} \sigma  & = \frac{\pi \lvert A \rvert ^{2}}{m_{h}^{2}}\int dx_{1} dx_{2} f_{L}(x_{1})f_{L}(x_{2})\delta(sx_{1}x_{2}-m_{h}^{2}) \\  & = \frac{\pi m_{h}^{2}}{v^{2} s}\int_{\tau_{h}}^{1}\frac{dx}{x}f_{L}(x)f_{L}\left( \frac{\tau_{h}}{x} \right)\end{align}.
>$$
>Here, $\tau_h \equiv \frac{m_h^2}{s}$. Now it's just a matter of substituting the splitting function and doing a simple integral.


**Observation:** In this case the energy scale is not $\sqrt{ s }$, but $v$ instead, indicating that the most relevant contributions come from the IR. The $s$ dependence comes from a logarithm. This also means that the electrons do not give much energy in the Higgs production

#### Hadron collider
In this case, one had to consider the parton system **inside the protons**. There are two parton layers (proton + quarks).

Now there is also the fact that because there are valence and sea quarks, **the parton distribution function runs**: 
$$
	\begin{align}
	f_{u,d}  & \sim 1 - g_{S}^{2} \log\left( \frac{E}{\Lambda _{QCD}} \right), \\
	f_{\bar{u},\bar{d},g,s,\bar{s}}  & \sim g_{S}^{2} \log\left( \frac{E}{\Lambda} \right), \\
    f_{c,\bar{c},b,\bar{b}}  & \sim g_{S}^{2} \log\left( \frac{E}{m_{c,b}} \right).	
	\end{align}
$$

In this case, the relevant process for Higgs production is **vector boson fusion**, in which two gluons fuse through a top loop into an Higgs. We have 
$$
	\sigma(gg\to h) = \frac{\pi^{2}}{8m_{h}^{2}}\Gamma(h\to gg)\delta(s - m_{h}^{2})
$$
### Production from gluons
In this case, the process is 
$$
	g+g \to t + \bar{t} + h,
$$
which looks like the preceding process, but a scissor cut one of the triangle sides

# Measuring Higgs decays
The Higgs must decay for the detector to be able to detect, so we are in fact measuring 
$$
	\sigma(pp\to h) \cdot \mathrm{BR}(h\to X).
$$
We have $\mathrm{BR}(h\to b\bar{b})\sim 58\%$. The problem is that $b\bar{b}$ is produced also from gluon and quark fusion.
Thus, we must look for more unusual processes.

