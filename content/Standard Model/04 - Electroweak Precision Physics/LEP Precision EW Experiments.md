The LEP accelerator achieved many important results in particle physics. Here are some of the most important ones:
- **Precision tests** on neutral current interaction. It was the final test for the symmetry breaking $SU(2) \times U(1)_{Y} \to U(1)_{\mathrm{em}}$.
- Verify that **$W$ and $Z$ are weakly coupled gauge bosons**. In particular, they verified the universality of the [[Electron-Neutrino Scattering|couplings]] $g_{L,R}$ , and the nonabelian nature of the bosons (LEP II).
- **Determination of SM parameters**, such as the top mass and the Higgs mass (LHC, 2012)
- **Constraints** on BSM models.

# What LEP measured
During its period, LEP could measure:
- **scattering cross sections**;
- [[Accelerator Observables|forward and backward asymmetries]];
- **polarizations** of leptons;

Near the $Z$ pole, the measured process is
$$
	e + \bar{e} \to \gamma^{*} / Z \to f + \bar{f}.
$$
The ratio of the cross sections of the two processes is 
$$
	\frac{\sigma_{\mathrm{weak}}}{\sigma_{\mathrm{QED}}} \sim \frac{G_{F}^{2} s^{2}}{(4\pi\alpha)^{2}}\sim \left( \frac{\sqrt{ s }}{30 \ \mathrm{GeV}} \right)^{4}.
$$
Because of radiative corrections, physical observables get modified:
- *[[Running of the Electromagnetic Coupling|running coupling constants]];*
- *changing $\Gamma(s)$ in the [[Decay and Optical Theorem|Breit-Wigner distribution]];*
- *[[Final State Radiation]].*

>[!abstract] Lepton polarizations
>- LEP could only measure the polarizations of initial electrons, and of final tau particles. This could  be done because the $\tau$ decays very rapidly in neutrinos and pions. By measuring the relative angle between the pions, the initial polarizations can be inferred.
>- SLAC could polarize the beams.


# Pseudo-Observables
*The cross section formula is the same as in [[Electron-Positron Annihilation]].*

We need a way to compare theoretical prediction to actual measured data. Let's look at the cross section: near the $m_{Z}$ resonant, its leading contribution can be written 
$$
	\sigma(s)_{e e \to ff} \approx \frac{12\pi}{m_{Z}^{2}}\Gamma_{e} \Gamma_{f} \frac{s}{(s-m_{Z}^{2})^{2} + m_{Z}^{2}\Gamma_{Z}^{2}},
$$
where define the quantities
$$
	\Gamma_{f} = 4N_{c} \Gamma_{0} [(g^{eff}_{V,f})^{2} R_{V}+ (g^{eff}_{A,f})^{2}R_{A}], \quad \Gamma_{0} = \frac{G_{F}m_{Z}^{2}}{24\pi \sqrt{ 2 }}.
$$
We are doing calculations at **one-loop level**, so that the couplings are [[Effective EW parameters|effective weak couplings]]. Here, $N_{c}$ is the number of colors of the particle, and $R_{V}$ and $R_{A}$ are known functions obtained from QED and QCD radiative corrections.

Two things are worth noting:
- in general $R_{V} \approx R_{A}$, so that  we have $\Gamma_{f} \approx (g_{V,f}^{e})^{2} + (g_{A,f}^{e})^{2}$;
- at the pole mass, the Breit-Wigner distribution is purely imaginary and there is no interference term.

Given our model, we can fit experimental data to theoretical predictions, with the assumption that **radiative QED and QCD corrections are exact**. 
This implies that our observed effective couplings are not purely experimental, but require some working hypotheses. Because of this, they are usually called **pseudo-observables**.