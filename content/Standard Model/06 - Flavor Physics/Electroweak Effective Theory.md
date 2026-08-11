I would like to build an effective Lagrangian for **all flavor processes**.
The Lagrangian has many terms, describing different phenomena. Here is the Lagrangian 
$$
	\begin{align}
	\mathcal{L}_{\mathrm{eff}}  & = \mathcal{L}_{\Delta B = 2} \\
	 & + \sum_{q=u,c}\lambda_{q}(C_{1} \mathcal{O}_{1}^{q} + C_{2} \mathcal{O}_{2}^{q})  \\
	 & - \lambda_{t}\left( \sum C_{i}\mathcal{O}_{i} + C_{7\gamma}\mathcal{O}_{7\gamma} + C_{8g}\mathcal{O}_{8g} + C_{9V}\mathcal{O}_{9V} + C_{10A}\mathcal{O}_{10A} \right).
	\end{align}
$$
Here, we summarize the various operators


| Sector                 | Operator                             | Phenomenon                            |
| ---------------------- | ------------------------------------ | ------------------------------------- |
| Meson mixing           | $\mathcal{O}_{\Delta F=2}$           | $M^{0}\leftrightarrow \bar{M}^{0}$    |
| Current-current        | $\mathcal{O}^{q}_{1,2}$              | Tree-level nonleptonic decay          |
| QCD penguin            | $\mathcal{O}_{3,\dots,6}$            | Loop-induced $d_{i}\to d_{j}q\bar{q}$ |
| Electroweak penguin    | $\mathcal{O}_{7,\dots,10}$           | EW loop-induced nonleptonic decay     |
| Electromagnetic dipole | $\mathcal{O}_{7\gamma}$              | $d_{i}\to d_{j}\gamma$                |
| Chromomagnetic dipole  | $\mathcal{O}_{8g}$                   | $d_{i}\to d_{j}g$                     |
| Semileptonic           | $\mathcal{O}_{9V},\mathcal{O}_{10A}$ | $d_{i}\to d_{j}\ell^{+}\ell^{-}$      |
