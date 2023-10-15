In [[thermodynamics]], [**Gibbs free energy**](https://en.wikipedia.org/wiki/Gibbs_free_energy) is a thermodynamic potential that can be used to calculate the maximum amount of [[Thermodynamic Work\|work]] that may be performed by a [[closed system]] at constant [[temperature]] and [pressure](https://en.wikipedia.org/wiki/Pressure "Pressure").

### Definition
$$G = H - TS$$
 - $H$ is the [[enthalpy]].
 - $T$ is the [[temperature]].
 - S is the [[entropy]].

### Connection to Entropy
> Assume a closed system that can exchange energy and volume with a reservoir.
> Both systems have the same temperature and pressure ($T = T_R, P = P_R$).
$$\begin{align}
U_{\text{total}} &= U + U_R \implies dU = -dU_R \\
V_{\text{total}} &= V + V_R \implies dV = -dV_R
\end{align}$$
$$\begin{align}
&dS = \dfrac{dU}{T} + \dfrac{P}{T}dV \\
&dS_R = \dfrac{dU_R}{T} + \dfrac{P}{T}dV_R = -\dfrac{dU}{T} - \dfrac{P}{T}dV \\
&dS_{\text{total}} = dS + dS_R = \dfrac{1}{T}(T dS - dU - PdV) \ge 0\\
&\implies \boxed{dG \le 0}
\end{align}$$
