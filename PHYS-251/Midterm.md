Stanley Goodwin, 10/26/2023

## Concept Questions

<hr>

1. *Spin ½ qubits are prepared in a state $\ket{\psi} = a\ket{Z^+} + b\ket{Z^-}$, where the coefficients $a$ and $b$ are unknown. The particles are sent one at a time through a Stern-Gerlach Analyzer oriented in the z-direction.*

a) *You send one particle through the analyzer and observe it leaving the "−" port. What can you infer about the coefficients $a$ and $b$?*

With a sample size N=1, there is no reasonable conclusion you can make on the coefficients.

b) *You send 30 particles through the analyzer one at a time. You observe 10 particles leave the + port of the analyzer and 20 particles leave the – port of the analyzer. Now what can you infer about the coefficients $a$ and $b$.*

$a^2 + b^2 = 1, \ \ \ b^2 = 2a^2 \implies a^2 + 2a^2 = 1$

$\ket{\psi} = \sqrt{\dfrac{1}{3}}\ket{Z^+} + \sqrt{\dfrac{2}{3}}\ket{Z^-}$
You can now be reasonably confident in the distribution of states with N=30.

<hr>

2. *Consider a quantum communication channel, where Alice encodes information on photons she wants to securely transmit to Bob. Alice and Bob want to use the quantum properties of their particles to determine if an eavesdropper Eve is listening in. When analyzing the security of their protocol, they assume Eve possesses “unlimited  resources,” meaning she is only constrained by the laws of (quantum) physics but otherwise has no technological limitations.*

a) It's a useful assumption to overestimate the resources of an attacker, as to be confident in the security in the worst possible case.

b) It's not always necessary to make an assumption like that, but by assuming the worst then you can get an upper bound on tolerance.

<hr>

3. *Photon Stuff*

a) *Describe the photon anti-bunching experiment. How does it give us the strongest evidence we have for the existence of single photons?*

Since the correlation between the signals from both detectors will have times where photons only exist on 1 branch, then it a discrete packet of energy like a photon. I.e. the probability of seeing a signal on detector B after a detection event on A is small.

b) *Compare a polarizing beam-splitter to a Z-oriented Stern-Gerlach Analyzer. How are they similar? How are they different?*

The beam-splitter does a similar effect to Z-oriented analyzers since it collapses the beam into 2 output beams of half intensity with opposing orientations. In this case, being horizontally polarized and vertically polarized.

They're different since Stern-Gerlach uses the Z-component of spin as its identifier to act upon. The beam-splitter uses light polarization orientation. They are mathematically identical binaries, but they are 2 different phenomena.

<hr>
## Calculation Questions

<hr>

1. Consider two state vectors for a spin ½ qubit.
	1. $\ket{\psi_1} = 4\ket{Z^+} + 2\ket{Z^-}$
	2. $\ket{\psi_2} = i\sqrt{\dfrac{1}{26}}\ket{Z^+} + \sqrt{\dfrac{25}{26}}\ket{Z^-}$

a) *Are the state vectors valid quantum states? If not, find a valid quantum state that represents the same physical system.*
$$\begin{align}
\langle\psi_1|\psi_1\rangle &= \left(4\bra{Z^+} + 2\bra{Z^-}\right)\left(4\ket{Z^+} + 2\ket{Z^-}\right) \\
&= 4^2\langle Z^+|Z^+\rangle + 4\cdot2\langle Z^+|Z^-\rangle+2\cdot4\langle Z^-|Z^+\rangle + 2^2\langle Z^-|Z^-\rangle \\
&= 4^2 + 2^2 = 20 \ne 1 \text{ (Not Valid)} \\
\ket{\psi'_1} &= \sqrt{\dfrac{16}{20}}\ket{Z^+} + \sqrt{\dfrac{4}{20}}\ket{Z^-}
\end{align}$$
$$\begin{align}
\langle\psi_2|\psi_2\rangle &= \left(-i\sqrt{\dfrac{1}{26}}\bra{Z^+} + \sqrt{\dfrac{25}{26}}\bra{Z^-}\right)\left(i\sqrt{\dfrac{1}{26}}\ket{Z^+} + \sqrt{\dfrac{25}{26}}\ket{Z^-}\right) \\
&= -i^2\sqrt{\dfrac{1}{26}}\sqrt{\dfrac{1}{26}}\langle Z^+|Z^+\rangle - i\sqrt{\dfrac{1}{26}}\sqrt{\dfrac{25}{26}}\langle Z^+|Z^-\rangle \\
& \ \ \ \ \ +i\sqrt{\dfrac{25}{26}}\sqrt{\dfrac{1}{26}}\langle Z^-|Z^+\rangle + \sqrt{\dfrac{25}{26}}\sqrt{\dfrac{25}{26}}\langle Z^-|Z^-\rangle \\
&= \dfrac{1}{26} + \dfrac{25}{26} = 1
\end{align}$$
b) *For each state: If an ensemble of particles are prepared in the state and sent  
through a z-oriented Stern-Gerlach Analyzer, what is the probability a particle will be  
observed leaving the + port of the analyzer. What about the – port?*
$$\begin{align}
\downarrow \ \ \ \ \ \ &\text{: + Output given }\psi_1\\
p(+|\psi'_1) &= \left|\langle Z^+|\psi'_1\rangle\right|^2 \\
&= \left|\bra{Z^+}\left(\sqrt{\dfrac{16}{20}}\ket{Z^+} + \sqrt{\dfrac{4}{20}}\ket{Z^-}\right)\right|^2 \\
&= \left|\sqrt{\dfrac{16}{20}}\langle Z^+|Z^+\rangle + \sqrt{\dfrac{4}{20}}\langle Z^+|Z^-\rangle\right|^2 \\
&= \left|\sqrt{\dfrac{16}{20}}\right|^2 = \dfrac{16}{20} = \boxed{80\%}
\end{align}$$
$$\begin{align}
p(-|\psi'_1) &= \left|\langle Z^-|\psi'_1\rangle\right|^2 \\
&= \left|\bra{Z^-}\left(\sqrt{\dfrac{16}{20}}\ket{Z^+} + \sqrt{\dfrac{4}{20}}\ket{Z^-}\right)\right|^2 \\
&= \left|\sqrt{\dfrac{16}{20}}\langle Z^-|Z^+\rangle + \sqrt{\dfrac{4}{20}}\langle Z^-|Z^-\rangle\right|^2 \\
&= \left|\sqrt{\dfrac{4}{20}}\right|^2 = \dfrac{4}{20} = \boxed{20\%}
\end{align}$$
$$\begin{align}
p(+|\psi_2) &= \left|\langle Z^+|\psi_2\rangle\right|^2 \\
&= \left|\bra{Z^+}\left(i\sqrt{\dfrac{1}{26}}\ket{Z^+} + \sqrt{\dfrac{25}{26}}\ket{Z^-}\right)\right|^2 \\
&= \left|i\sqrt{\dfrac{1}{26}}\langle Z^+|Z^+\rangle + \sqrt{\dfrac{25}{26}}\langle Z^+|Z^-\rangle\right|^2 \\
&= \left|e^{i\tfrac{\pi}{2}}\sqrt{\dfrac{1}{26}}\right|^2 = 1\cdot \dfrac{1}{26} = \boxed{3.9\%}
\end{align}$$
$$\begin{align}
p(-|\psi_2) &= \left|\langle Z^-|\psi_2\rangle\right|^2 \\
&= \left|\bra{Z^-}\left(i\sqrt{\dfrac{1}{26}}\ket{Z^+} + \sqrt{\dfrac{25}{26}}\ket{Z^-}\right)\right|^2 \\
&= \left|i\sqrt{\dfrac{1}{26}}\langle Z^-|Z^+\rangle + \sqrt{\dfrac{25}{26}}\langle Z^-|Z^-\rangle\right|^2 \\
&= \left|\sqrt{\dfrac{25}{26}}\right|^2 = \dfrac{25}{26} = \boxed{96.1\%}
\end{align}$$
c) *Repeat the calculation from part b, but instead send particles through an x-oriented analyzer.*
$$\begin{align}
p(+|\psi_1) &= \left|\langle X^+|\psi_1\rangle\right|^2 \\
&= \left|\bra{X^+}\left(\sqrt{\dfrac{16}{20}}\ket{Z^+} + \sqrt{\dfrac{4}{20}}\ket{Z^-}\right)\right|^2 \\
&= \left|\sqrt{\dfrac{16}{20}}\langle X^+|Z^+\rangle + \sqrt{\dfrac{4}{20}}\langle X^+|Z^-\rangle\right|^2 \\
&= \left|\sqrt{\dfrac{1}{2}}\sqrt{\dfrac{16}{20}}\right|^2+\left|\sqrt{\dfrac{1}{2}}\sqrt{\dfrac{4}{20}}\right|^2 = \dfrac{16}{40} + \dfrac{4}{40} = \boxed{50\%}
\end{align}$$
$$\begin{align}
p(-|\psi_1) &= \left|\langle X^-|\psi_1\rangle\right|^2 \\
&= \left|\bra{X^-}\left(\sqrt{\dfrac{16}{20}}\ket{Z^+} + \sqrt{\dfrac{4}{20}}\ket{Z^-}\right)\right|^2 \\
&= \left|\sqrt{\dfrac{16}{20}}\langle X^-|Z^+\rangle + \sqrt{\dfrac{4}{20}}\langle X^-|Z^-\rangle\right|^2 \\
&= \left|\sqrt{\dfrac{1}{2}}\sqrt{\dfrac{16}{20}}\right|^2+\left|\sqrt{\dfrac{1}{2}}\sqrt{\dfrac{4}{20}}\right|^2 = \dfrac{16}{40} + \dfrac{4}{40} = \boxed{50\%}
\end{align}$$
$$\begin{align}
p(+|\psi_2) &= \left|\langle X^+|\psi_2\rangle\right|^2 \\
&= \left|\bra{X^+}\left(i\sqrt{\dfrac{1}{26}}\ket{Z^+} + \sqrt{\dfrac{25}{26}}\ket{Z^-}\right)\right|^2 \\
&= \left|i\sqrt{\dfrac{1}{26}}\langle X^+|Z^+\rangle + \sqrt{\dfrac{25}{26}}\langle X^+|Z^-\rangle\right|^2 \\
&= \left|i\sqrt{\dfrac{1}{26}}\sqrt{\dfrac{1}{2}} + \sqrt{\dfrac{25}{26}}\sqrt{\dfrac{1}{2}}\right|^2 \\
&= \left|e^{i\tfrac{\pi}{2}}\sqrt{\dfrac{1}{26}}\sqrt{\dfrac{1}{2}}\right|^2 + \left|\sqrt{\dfrac{25}{26}}\sqrt{\dfrac{1}{2}}\right|^2 = \dfrac{1}{54} + \dfrac{25}{54} = \boxed{50\%}
\end{align}$$
$$\begin{align}
p(-|\psi_2) &= \left|\langle X^-|\psi_2\rangle\right|^2 \\
&= \left|\bra{X^-}\left(i\sqrt{\dfrac{1}{26}}\ket{Z^+} + \sqrt{\dfrac{25}{26}}\ket{Z^-}\right)\right|^2 \\
&= \left|i\sqrt{\dfrac{1}{26}}\langle X^-|Z^+\rangle + \sqrt{\dfrac{25}{26}}\langle X^-|Z^-\rangle\right|^2 \\
&= \left|i\sqrt{\dfrac{1}{26}}\sqrt{\dfrac{1}{2}} + \sqrt{\dfrac{25}{26}}\sqrt{\dfrac{1}{2}}\right|^2 \\
&= \left|e^{i\tfrac{\pi}{2}}\sqrt{\dfrac{1}{26}}\sqrt{\dfrac{1}{2}}\right|^2 + \left|\sqrt{\dfrac{25}{26}}\sqrt{\dfrac{1}{2}}\right|^2 = \dfrac{1}{54} + \dfrac{25}{54} = \boxed{50\%}
\end{align}$$

<hr>

2. Consider three quantum states for a qubit.
	1. $\ket{\psi} = \sqrt{\dfrac{16}{25}}\ket{X^+}+\sqrt{\dfrac{9}{25}}\ket{X^-}$
	2. $\ket{\phi} = \sqrt{\dfrac{1}{2}}\ket{Z^+}+i\sqrt{\dfrac{1}{2}}\ket{Z^-}$
	3. $\ket{\gamma} = \sqrt{\dfrac{4}{5}}\ket{Z^+}-i\sqrt{\dfrac{1}{5}}\ket{Z^-}$

a) *Write each states in a matrix form.*
$\ket{\psi} = \dfrac{1}{\sqrt{25}}\begin{bmatrix}4\\3\end{bmatrix}_{X} = \dfrac{1}{\sqrt{2}}\begin{bmatrix}1\\1\end{bmatrix}_{Z}$
$\ket{\phi} = \dfrac{1}{\sqrt{2}}\begin{bmatrix}1\\i\end{bmatrix}_{Z}$
$\ket{\gamma} = \dfrac{1}{\sqrt{5}}\begin{bmatrix}2\\-i\end{bmatrix}_{Z}$

b) *Using Bra-Ket notation, evaluate the inner product $\langle\phi|\gamma\rangle$.*
$$\begin{align}
\langle\phi|\gamma\rangle &= \left(\sqrt{\dfrac{1}{2}}\bra{Z^+}-i\sqrt{\dfrac{1}{2}}\bra{Z^-}\right)\left(\sqrt{\dfrac{4}{5}}\ket{Z^+}-i\sqrt{\dfrac{1}{5}}\ket{Z^-}\right) \\
&= \sqrt{\dfrac{4}{10}} +i^2\sqrt{\dfrac{1}{10}} = \boxed{\sqrt{\dfrac{1}{10}}}
\end{align}$$
c) *Repeat part b using matrix notation.*
$$\begin{align}
\langle\phi|\gamma\rangle &= \sqrt{\dfrac{1}{10}}\begin{bmatrix}1&-i\end{bmatrix}_{Z}\begin{bmatrix}2\\-i\end{bmatrix}_{Z} \\
&= \sqrt{\dfrac{1}{10}}\left(2+i^2\right) = \boxed{\sqrt{\dfrac{1}{10}}}
\end{align}$$
d) *Using whichever notation you prefer, evaluate the inner products $\langle\phi|\psi\rangle$ and $\langle\gamma|\phi\rangle$.*
$$\begin{align}
\langle\phi|\psi\rangle &= \dfrac{1}{2}\begin{bmatrix}1&-i\end{bmatrix}_{Z}\begin{bmatrix}1\\1\end{bmatrix}_{Z} = \boxed{\dfrac{1}{2}\left(1-i\right)}
\end{align}$$
$$\begin{align}
\langle\gamma|\phi\rangle &= \sqrt{\dfrac{1}{10}}\begin{bmatrix}2&i\end{bmatrix}_{Z}\begin{bmatrix}1\\i\end{bmatrix}_{Z} = \sqrt{\dfrac{1}{10}}\left(2-i^2\right) = \boxed{\sqrt{\dfrac{1}{10}}}
\end{align}$$

<hr>

3. *Spin ½ qubits are prepared in the quantum state $\ket{\psi_\text{in}} = \sqrt{\dfrac{16}{41}}\ket{Z^+} + \sqrt{\dfrac{25}{41}}\ket{Z^-}$ and sent through the sequence of analyzers show below.*

a) $p(X^+|\psi_\text{in}) = 50\%, \ \ \ p(X^-|\psi_\text{in}) = 50\%$

b) $p(X^+,X^+|\psi_\text{in}) = 50\%$

c) $p(X^+,X^+,Z^-|\psi_\text{in}) = 25\%$

<hr>

4. *Spin ½ qubits are prepared in the quantum state $\ket{\psi} = \sqrt{\dfrac{4}{13}}\ket{Z^+}-\sqrt{\dfrac{9}{13}}\ket{Z^-}$.*

a) *Let’s say you were gambling based on your ability to predict whether a given qubit sent through a Stern Gerlach Analyzer leaves the top or bottom port. Without doing any calculations, would you be able to win (guess the correct outcome) more often with an X-analyzer or a Z-analyzer? Explain your choice.*

Measuring in Z: 4:9 Odds.
Measuring in X: 1:1 Odds.
The chance of winning with either state is equal since the odds are known before your guess is made, so long as you guess Z-up and Z-down with the same weighting as the wavefunction coefficients squared. 

b) *Evaluate the expectation value $\langle\sigma_x\rangle$ to find the average value for measurements with an X-analyzer.*
$$\begin{align}
\langle\sigma_x\rangle &= \bra{\psi}\sigma_x\ket{\psi} \\
&= \dfrac{1}{13}\begin{bmatrix}2&-3\end{bmatrix}_Z\begin{bmatrix}0&1\\1&0\end{bmatrix}\begin{bmatrix}2\\-3\end{bmatrix}_Z \\
&= \dfrac{1}{13}\begin{bmatrix}2&-3\end{bmatrix}\begin{bmatrix}-3\\2\end{bmatrix} = \boxed{-\dfrac{12}{13}}
\end{align}$$
$$\begin{align}
\langle\sigma_z\rangle &= \bra{\psi}\sigma_z\ket{\psi} \\
&= \dfrac{1}{13}\begin{bmatrix}2&-3\end{bmatrix}_Z\begin{bmatrix}1&0\\0&-1\end{bmatrix}\begin{bmatrix}2\\-3\end{bmatrix}_Z \\
&= \dfrac{1}{13}\begin{bmatrix}2&-3\end{bmatrix}\begin{bmatrix}2\\3\end{bmatrix} = \boxed{-\dfrac{5}{13}}
\end{align}$$
c) *Evaluate the variance to find the uncertainty associated with measurements with an X-analyzer.*
$$\begin{align}
\langle(\Delta\sigma_x)^2\rangle &= \bra{\psi} \sigma_x^2 \ket{\psi} - \langle{\sigma}_x\rangle^2 = 1 - \langle{\sigma}_x\rangle^2\\
&= 1-\left(\dfrac{12}{13}\right)^2 = \boxed{\dfrac{25}{169}}
\end{align}$$
$$\begin{align}
\langle(\Delta\sigma_z)^2\rangle &= \bra{\psi} \sigma_z^2 \ket{\psi} - \langle{\sigma}_z\rangle^2 = 1 - \langle{\sigma}_z\rangle^2\\
&= 1-\left(\dfrac{5}{13}\right)^2 = \boxed{\dfrac{144}{169}}
\end{align}$$
d) *Does your calculated answer to part c agree with your reasoning in part a? Why or why not?*

It doesn't match at all, which is concerning. Like, given the information about the wavefunction's state, you should have no difference in winning/losing so long as you guess Z up or Z down with the same probabilities as the coefficients squared.

The variance does make sense though, since deviations from 50/50 odds tend to produce more extreme jumps in final answers.