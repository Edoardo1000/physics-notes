The key idea is that every quantum field theory possesses a cutoff, so in a theory valid up to some scale, and the effective Lagrangian parameters change so that physical observables remain the same.

# Toy model

*The analysis is based on this paper:https://arxiv.org/abs/1505.01537*

This is a very crude toy model, but explains the main mechanism behind the renormalization group. 

Consider a microscopic Lagrangian in 2+1 dimensions, with field $a$ canonically normalized, subject to a quartic interaction:
$$
\mathcal{L}_{\mathrm{micro}}=-\frac{1}{2} (\partial a)^{2} - \frac{g^{2}}{12}a^{4}.
$$
In our analysis, we utterly ignore the mass term. This is a very brutal approximation, but does not spoil the qualitative features of the phenomenon.

### Interacting fixed point

Let's integrate out the heavy modes, which means lowering the cutoff scale $\Lambda$ and using an effective Lagrangian $\mathcal{L}_{\mathrm{eff}}$, which depend on the cutoff itself.

If we look at how the quartic term evolves, a one-loop estimate by dimensional analysis gives 
$$
A_{\mathrm{loop}} \sim c \frac{g^{4}}{\Lambda},
$$
since the leading loop has to vertices, and it is a correction to the coupling with dimension $[g^{2}]=1$. Also remember that $[a]=1 / 2$ in 3 dimensions.

Now, the renormalization group equations should be stated in terms of dimensionless couplings, so we define 
$$
\hat{g}^{2} = \frac{g^{2}}{\Lambda}.
$$
The renormalization group flow is thus
$$
\Lambda  \frac{d\hat{g}^{2}}{d\Lambda} = \hat{g}(c \hat{g} - 1). 
$$
We see that other than the trivial fixed point $\hat{g}=0$, we also have the nontrivial one $\hat{g} = \frac{1}{c}$. By expanding, it can be shown that it is an attractive fixed point, and in its vicinity the coupling satisfies 
$$
g_{\mathrm{eff}}^{2} = h \Lambda,
$$
with $h$ some constant.

The fixed point is reached when loop corrections compensate for the leading classical flow, so we must have 
$$
\Lambda \sim g_{\mathrm{eff}}^{2},
$$
and thus the constant $h$ is of order unity.

### Nonzero expectation value for $a$

Now we know how the coupling evolves. The interesting physical case is when $a$ has a nonzero expectation value, either by a [[Spontaneous Symmetry Breaking|spontaneous symmetry breaking]] potential.

Thus, suppose that by some means the field $a$ acquired a nonzero expectation value $\langle a \rangle$. By expanding the potential, the fluctuations around that value acquire a mass 
$$
m_{a}^{2} = g^{2}_{\mathrm{eff}} a^{2}
$$

If we now push our cutoff $\Lambda$ even below this mass, the coupling constant stops running, since the corrections get suppressed by a factor $\frac{\Lambda}{m_{a}}$. Consistency with the fixed point requires 
$$
g^{2}_{\mathrm{eff}}(m_{a}^{2})= h m_{a} = h  g_{\mathrm{eff}}a,
$$
which implies 
$$
g_{\mathrm{eff}}^{2}(m_{a}^{2}) = h^{2}a^{2},\quad \Lambda \sim m_{a} = ha^{2}.
$$
Thus, at this scale, the effective potential becomes 
$$
V_{\mathrm{eff}}(a) = \frac{h^{2}}{12} a^{6}.
$$
This relation could be obtained by simple dimensional analysis plus the requirement of conformal invariance. The RG flow argument shows the dynamical process which justifies the potential, and the fact that the effective theory is conformally invariant even at the classical level (an effective theory has a cutoff which spoils the original conformal symmetry, this was not obvious).