In [[Thermodynamics\|thermodynamics]], [**Helmholtz free energy**](https://en.wikipedia.org/wiki/Helmholtz_free_energy) is a thermodynamic potential that measures the useful [[Thermodynamic Work\|work]] that may be performed by a [[closed system]] at constant [[temperature]].

### Definition
$$F = U - TS$$
 - $U$ is the [[internal energy]].
 - $T$ is the [[temperature]].
 - S is the [[entropy]].

### Connection to Entropy
> Assume a closed system that can exchange energy with a reservoir.
> The reservoir is large enough that it doesn't change temperature.
$$\begin{align}
U_{\text{total}} &= U + U_R \implies dU = -dU_R \\
S_{\text{total}} &= S + S_R \implies dS_{\text{total}} = dS + dS_R \ge 0
\end{align}$$
$$\begin{align}
&dS_R = \dfrac{dU_R}{T_R} = \dfrac{-dU}{T} \\
&dS_{\text{total}} = dS + dS_R = T dS - dU \ge 0\\
&\implies \boxed{dF \le 0}
\end{align}$$
