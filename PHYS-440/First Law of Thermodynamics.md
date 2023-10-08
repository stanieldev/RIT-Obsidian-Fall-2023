#TODO Fix formatting, Use 0th law as a template
The [**first law of thermodynamics**](https://en.wikipedia.org/wiki/First_law_of_thermodynamics "First law of thermodynamics") is one of the four principal [[Laws of Thermodynamics\|laws of thermodynamics]].
It is a statement of the law of [[Conservation of Energy\|conservation of energy]] in the context of [[Thermodynamic Processes\|thermodynamic processes]].
#### Definition
$$ \Delta U = Q + W $$
 - $\Delta U$ is the change in [[Internal Energy\|internal energy]] of a system.
 - $Q$ is the [[Heat\|heat]] added or removed from a system.
 - $W$ is the [[Thermodynamic Work\|thermodynamic work]] done on or by the system.
### Fundamental Relations
$$\begin{align}
dU &= T dS - P dV + \displaystyle\sum_i \mu_iN_i \\
dH &= T dS + V dP \\
dF &= -SdT - PdV \\
dG &= -SdT + V dP
\end{align}$$https://en.wikipedia.org/wiki/Fundamental_thermodynamic_relation

Helmholtz Free Energy
$$\Delta F = \Delta U - T \Delta S$$
### Example: Spring and Gas
$\Delta U = 0$
$\Delta S = N k_b \log \dfrac{V_f}{V_i}$
$$\Delta F = \Delta U - T \Delta S = -N k_b T\log \left(\dfrac{V_f}{V_i}\right)$$


We have a system that is not fully isolated.
Can exchange energy with environment.
$U_{total} = U + U_R$
Energy is conserved so $dU = -dU_R$
The environment acts as a reservoir of energy, so that it can absorb or release unlimited energy without any change in its temperature.
Total entropy of the universe is $S_{total} = S + S_R$, where $S_R$ is the reservoir entropy.
By the second law of thermodynamics, $dS_{total} = dS + dS_R \ge 0$

Using $dU = TdS - PdV + \mu dN$
$$dS_R = \dfrac{dU_R}{T_R} = -\dfrac{dU}{T}$$
