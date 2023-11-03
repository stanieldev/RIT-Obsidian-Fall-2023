### Ideal Mixtures
Using the Gibbs free energy relation $G = U + PV - TS$, with defining $x = \tfrac{N_B}{N_A+N_B} = \tfrac{N_B}{N}$.

Before the two substances are mixed:
$$G = (1-x)G_A + xG_B \text{ \; As a linear interpolation.}$$
After (ideally) mixing $A$ and $B$ :
$$\Delta S_\text{mixing} = Nk_b\left[x\log x + (1-x)\log(1-x)\right]$$
$$G = (1-x)G_A + xG_B - T\Delta S_\text{mixing}$$

### Dilute Solutions
$$G = N_A \mu_0 (T,P) + N_B f(T, P) - N_B k_b T \log N_A + k_bT\left(N_B\log N_B - N_B\right)$$
$$\begin{align}
\mu_A &= \left(\dfrac{\partial G}{\partial N_A}\right)_{T,P,N_B} = \mu_0 (T,P) - \dfrac{N_B}{N_A}k_bT \\
\mu_B &= \left(\dfrac{\partial G}{\partial N_B}\right)_{T,P,N_A} = f(T,P) - k_bT\log\dfrac{N_B}{N_A} 
\end{align}$$

### Osmosis
$$\begin{align}
&\mu_0 - \dfrac{N_B}{N_A}k_bT = \mu_0 + \delta P \dfrac{\partial \mu_0}{\partial P} \\
&\dfrac{N_B}{N_A}k_bT = \delta P \dfrac{\partial \mu_0}{\partial P} = \delta P \dfrac{V}{N_A}\\
&\implies \boxed{\delta P = \dfrac{N_Bk_bT}{V}}
\end{align}$$
