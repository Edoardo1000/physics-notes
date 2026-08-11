---
tags:
  - status/to-do
---

# Final state radiation
If we look at the amplitude 
$$
	e + \bar{e} \to f + \bar{f} + \gamma,
$$
we find that its cross section goes like 
$$
	\sigma \sim \frac{\alpha}{2\pi}\log\left( \frac{\mu_{IR}}{E} \right)\sigma_{0}.
$$
I need to get rid of the regulator, how can I do that?
There also exist contributions coming from 1-loop diagrams. For example, the vertex gives an interference contribution to the cross section
$$
	\sigma(\gamma\to f \bar{f}) = \sigma_{0}\left[ 1 +   \frac{\alpha}{4\pi}\log\left( \frac{E}{\mu_{IR}} \right)\right].
$$

The key idea is the **the experiment does not have infinite precision**, so there is a threshold energy under which the detector does not see anything. Because of this, it cannot distinguish between two electrons and two electrons plus a very soft photon. Thus, the total cross section is 
$$
	\sigma_{tot} = \sigma(\gamma\to f\bar{f}) + \sigma(\gamma\to f \bar{f} \gamma)\biggr|_{E<E_{min}} \sim \sigma_{0}\left( 1 + \frac{\alpha}{4\pi}\log\left( \frac{E}{E_{min}} \right) \right) + O(\alpha^{2}).
$$
The divergence is thus **physical**, the softer the photons I can see, the greater the cross section.

*The notes talk about a KLN theorem, look at it some day*

**Do the full calculation**