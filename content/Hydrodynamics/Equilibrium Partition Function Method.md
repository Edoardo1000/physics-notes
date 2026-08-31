*This method is based on the paper https://arxiv.org/abs/1203.3544.*

There is a method to obtain constraints on the [[Relativistic Hydrodynamics|constitutive relations]] based on the thermal partition function. The trick is to use the path integral formulation: 
$$
Z[g,A] = \int D\varphi e^{ -S[\varphi,g,A] },
$$
where $\phi$ are the fields of the theory, and $g,A$ are background metric and gauge fields. 

>[!warning]- Note: imaginary time
>There is a remark to be made: the calculation of the path integral proceeds in imaginary time, so the metric has to be Wick-rotated.
>Meanwhile, the relativistic hydrodynamic equations are formulated using a Lorentzian signature. 
>In the case of stationary metrics, which is the setting in which the physical system is at equilibrium, the metric components do not depend on time and the transition is seamless.

By differentiating with respect to the background fields, we can find the stress-energy tensor and the currents, whose conservation laws give the constitutive relations: 
$$
\langle T^{\mu \nu}(x) \rangle = \frac{2}{\sqrt{ g }} \frac{\delta}{\delta g_{\mu \nu}(x)}\log Z,\quad \langle J^{\mu}(x) \rangle = \frac{1}{\sqrt{ g }} \frac{\delta}{\delta g_{\mu \nu}(x)}\log Z.
$$
To get constraints on the hydrodynamic equations, the procedure is as follows:
- write the most general form of the constitutive relations based on symmetry in function of the fields $u^{\mu},T$,etc.;
- write the fields in function of the background fields in the most general form;
- write the most general form of the partition function as a function of the background fields;
- calculate the stress-energy tensor and the current by differentiating with respect to the background fields;
- equate the two expressions obtained for $T^{\mu \nu},J^{\mu}$.

It is convenient to do a [[Kaluza-Klein Reduction|Kaluza-Klein decomposition]] of the fields. Thus, our background fields, in the case of just a $U(1)$ gauge field, are $\{ g_{ij}(\vec{x}),a_{i}(\vec{x}),\phi(\vec{x}),\mathcal{A}_{\mu}(\vec{x}) \}$.

We consider fields which do not depend on time
# Partition function

### Zeroth order

At leading order, the partition function is an arbitrary functions built on the possible scalars we can build, which are just $\{ \phi, A_{0} \}$, where 
$$
A_{0}=\mathcal{A}_{0} + \mu_{0},
$$
where $\mu_{0}$ is the chemical potential of the system (a chemical potential can be incorporated in the background gauge fields through a gauge transformation).

The usual flat space thermodynamic relation 
$$
\log Z = \beta \Omega = \beta P V,
$$
where $\Omega$ is the grand-canonical partition function, lets us guess what might the general functional form. At zeroth order we eventually find $T(x) = T_{0} e^{ -\phi }$, with $T_{0}$ the temperature of the system, so that we have
$$
\log Z = \int_{\Sigma} dS \frac{1}{T_{0}e^{ -\phi }} P(T_{0}e^{ -\phi },A_{0}e^{ -\phi }),
$$
where the integral runs along a spacelike hypersurface $\Sigma$, $dS$ is the area element, and P is a function of the temperature. The area element is given by $dS_{\mu} = \sqrt{ \gamma } d^{3}x$,c with $\gamma$ the induced metric on the surface.

**Note:** The expression can also be recast in the form 
$$
\log Z = \int d^{4}x \sqrt{ -g } P(T_{0}e^{ -\sigma }).
$$
>[!math]- Example: free field
>To illustrate how the machinery works, take a free real scalar field. In this case, the Lagrangian is simply 
>$$
>\mathcal{L} = -\frac{1}{2} (\partial \phi)^{2},
>$$
>and the partition function is given by summing over all the independent modes:
>$$
>\log Z = -V \int \frac{d^{3}k}{(2\pi)^{3}} \ln(1- e^{ -\beta k }),
>$$
>from which we find 
>$$
>P(T) = \frac{\pi^{2}}{90}T^{4}.
>$$

### Second order, neutral case

At second order, the most general partition function is of the form
$$
\begin{align}
\log Z &= \int dS \ \frac{1}{T_{0}e^{-\phi}} P(T_{0}e^{ -\phi })  \\
& + \int dS \ (P_{1}(\phi)R + T_{0}^{2} P_{2}(\phi)(\partial_{i}a_{j}-\partial_{j}a_{i})^{2} + P_{3}(\phi)(\nabla \phi)^{2}),
\end{align}
$$
were $P_{1},P_{2},P_{3}$ are arbitrary functions, and $a_{i}$ is the Kaluza-Klein field. It is possible to demonstrate that 
$$
P_{i}(\phi) = P_{i}(T_{0}e^{ -\phi }).
$$
### First order, charged case

#### 3+1 dimensions
It can be shown that the partition function has the general formula 
$$
\begin{align}
\log Z & = W^{0} + W^{1}_{\mathrm{inv}} + W^{1}_{\mathrm{anom}}, \\
W^{0} & = \int dS \frac{1}{T_{0}e^{ -\phi }} P(T_{0}e^{ -\phi },A_{0} e^{ -\phi }), \\
W^{1}_{\mathrm{inv}} & = \frac{C_{0}}{2} \int AdA + T_{0}^{2} \frac{C_{1}}{2} \int a da + T_{0} \frac{C_{2}}{2} \int A da, \\
W^{1}_{\mathrm{anom}}  & = \frac{C}{2}\left( \int \frac{A_{0}}{3T_{0}} A dA + \frac{A_{0}^{2}}{6T_{0}} A da \right),
\end{align}
$$
where 
$$
A_{0} \equiv \mathcal{A}_{0} + \mu_{0},\quad A_{i} \equiv \mathcal{A}_{i} - A_{0}a_{i},
$$
and 
$$
\frac{1}{2} \int XdY \equiv \int dS \epsilon^{ijk}X_{i}\partial_{j}Y_{k},\quad \frac{1}{2} \int dY = dS_{2} \epsilon^{ij} \partial_{i}Y_{j}.
$$
Here, $dS_{2}$ is the 2-dimensional area element.

$W^{1}_{\mathrm{inv}}$ is the gauge-invariant part of the partition function, while $W^{1}_{\mathrm{anom}}$ encodes the effect of [[Anomalies]].

#### 2+1 dimensions
In this case, the partition functions takes the form 
$$
\begin{align}
\log Z  & = W^{0}+ W^{1}, \\
W^{0}  & = \int dS_{2} \frac{1}{T_{0}e^{ -\phi }}P(T_{0}e^{ -\phi },e^{ -\phi }A_{0}), \\
W & = \frac{1}{2} \int \alpha(\phi,A_{0})dA + T_{0}\beta(\phi,A_{0})da
\end{align}
$$