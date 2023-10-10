<hr>

1. Use Euler's Equation for the following
a) $e^{i\phi}+e^{-i\phi} = \cos(\phi) + i\sin(\phi) + \cos(\phi) - i\sin(\phi) = 2 \cos(\phi)$
b) $e^{i\phi}-e^{-i\phi} = \cos(\phi) + i\sin(\phi) - \cos(\phi) + i\sin(\phi) = 2i \sin(\phi)$
c) $\left|1+e^{i\phi}\right|^2 = \left(1+e^{i\phi}\right)\left(1+e^{-i\phi}\right) = 2 + e^{-i\phi}+e^{i\phi} = 2 + 2\cos(\phi) = 4 \cos^2\left(\dfrac{\phi}{2}\right)$
d) $\left|1-e^{i\phi}\right|^2 = \left(1-e^{i\phi}\right)\left(1-e^{-i\phi}\right) = 2 -e^{-i\phi}-e^{i\phi} = 2 - 2\cos(\phi) = 4 \sin^2\left(\dfrac{\phi}{2}\right)$
<hr>

2. Consider the quantum states
$$\begin{align}
\ket{\psi_1} &= \sqrt{\dfrac{1}{3}} \ket{+} + i\sqrt{\dfrac{2}{3}} \ket{-}&
\bra{\psi_1} &= \sqrt{\dfrac{1}{3}} \bra{+} - i\sqrt{\dfrac{2}{3}} \bra{-} \\
\ket{\psi_2} &= \sqrt{\dfrac{1}{5}} \ket{+} - \sqrt{\dfrac{4}{5}} \ket{-}&
\bra{\psi_2} &= \sqrt{\dfrac{1}{5}} \bra{+} - \sqrt{\dfrac{4}{5}} \bra{-} \\
\ket{\psi_3} &= \sqrt{\dfrac{1}{2}} \ket{+} + \sqrt{\dfrac{1}{2}}e^{i\tfrac{\pi}{4}}\ket{-}&
\bra{\psi_3} &= \sqrt{\dfrac{1}{2}} \bra{+} + \sqrt{\dfrac{1}{2}}e^{-i\tfrac{\pi}{4}}\bra{-}\end{align}
$$
$$\begin{align} 
\langle \psi_1 | \psi_2 \rangle &= \left(\sqrt{\dfrac{1}{3}} \bra{+} - i\sqrt{\dfrac{2}{3}} \bra{-}\right)\left(\sqrt{\dfrac{1}{5}} \ket{+} - \sqrt{\dfrac{4}{5}} \ket{-}\right) \\ &= \sqrt{\dfrac{1}{15}} \langle+|+\rangle - i\sqrt{\dfrac{2}{15}} \langle-|+\rangle - \sqrt{\dfrac{4}{15}} \langle+|-\rangle + i\sqrt{\dfrac{8}{15}} \langle-|-\rangle \\
&= \sqrt{\dfrac{1}{15}} + i\sqrt{\dfrac{8}{15}}
\end{align}$$
$$\begin{align}
\langle \psi_2 | \psi_1 \rangle &= \left(\sqrt{\dfrac{1}{5}} \bra{+} - \sqrt{\dfrac{4}{5}} \bra{-}\right) \left(\sqrt{\dfrac{1}{3}} \ket{+} + i\sqrt{\dfrac{2}{3}} \ket{-}\right) \\
&= \sqrt{\dfrac{1}{15}} \langle+|+\rangle + i\sqrt{\dfrac{2}{15}} \langle-|+\rangle - \sqrt{\dfrac{4}{15}} \langle+|-\rangle - i\sqrt{\dfrac{8}{15}} \langle-|-\rangle \\
&= \sqrt{\dfrac{1}{15}} - i\sqrt{\dfrac{8}{15}}
\end{align}$$
$$\begin{align}
\langle \psi_3 | \psi_1 \rangle &= \left(\sqrt{\dfrac{1}{2}} \bra{+} + \sqrt{\dfrac{1}{2}}e^{-i\tfrac{\pi}{4}}\bra{-}\right)\left(\sqrt{\dfrac{1}{3}} \ket{+} + i\sqrt{\dfrac{2}{3}} \ket{-}\right) \\
&= \sqrt{\dfrac{1}{6}} \langle+|+\rangle + \sqrt{\dfrac{1}{6}}e^{-i\tfrac{\pi}{4}}\langle-|+\rangle + i\sqrt{\dfrac{2}{6}} \langle+|-\rangle + i\sqrt{\dfrac{2}{6}}e^{-i\tfrac{\pi}{4}}\langle-|-\rangle \\
&= \sqrt{\dfrac{1}{6}} + i\sqrt{\dfrac{2}{6}}e^{-i\tfrac{\pi}{4}}
\end{align}$$
$$\langle \psi_3 | \psi_3 \rangle = \left(\sqrt{\dfrac{1}{2}}\right)^2 + \left(\sqrt{\dfrac{1}{2}}\right)^2 = 1$$
$$|\langle \psi_3 | \psi_1 \rangle|^2 = \left(\sqrt{\dfrac{1}{6}}\right)^2 + \left(\sqrt{\dfrac{2}{6}}\cos(\tfrac{\pi}{4})\right)^2 = \dfrac{5}{6} = 83.3\% $$
$$\begin{align}
|\langle \psi_2 | \psi_3 \rangle|^2 &= \left|\left(\sqrt{\dfrac{1}{5}} \bra{+} - \sqrt{\dfrac{4}{5}} \bra{-}\right)\left(\sqrt{\dfrac{1}{2}} \ket{+} + \sqrt{\dfrac{1}{2}}e^{i\tfrac{\pi}{4}}\ket{-}\right)\right|^2 \\
&= \left|\sqrt{\dfrac{1}{10}} \langle+|+\rangle - \sqrt{\dfrac{4}{10}} \langle-|+\rangle + \sqrt{\dfrac{1}{10}}e^{i\tfrac{\pi}{4}} \langle+|-\rangle - \sqrt{\dfrac{4}{10}}e^{i\tfrac{\pi}{4}} \langle-|-\rangle \right|^2 \\
&= \left|\sqrt{\dfrac{1}{10}} - \sqrt{\dfrac{4}{10}}e^{i\tfrac{\pi}{4}}\right|^2 \\
&= \left(\sqrt{\dfrac{1}{10}}\right)^2 + \left(\sqrt{\dfrac{4}{10}}\cos(\tfrac{\pi}{4})\right)^2 = 2 - \sqrt{2} \approx 59\%
\end{align}$$
<hr>

3. Qubits are prepared to be in the state vector: $\ket{\psi} = 1\ket{+}+3i\ket{-}$
$$\langle \psi | \psi \rangle = 1^2+(3i)(-3i) = 10 \ne 1$$
$$\ket{\psi} = \sqrt{\dfrac{1}{10}} \ket{+} + i\sqrt{\dfrac{9}{10}} \ket{-}, \ \ \ \bra{\psi} = \sqrt{\dfrac{1}{10}} \ket{+} - i\sqrt{\dfrac{9}{10}} \ket{-}$$
<hr>

4. Consider a general state $\ket{\psi} = a\ket{+} + b\ket{-}$
a) Only 2 numbers are required for the state, since 
$$\ket{\psi} = a\ket{+} + \sqrt{1-a^2}e^{i\phi}\ket{-}$$
b) My state vector is normalized by the definition of a,b I chose.
c) *2 Real Numbers* are required to specify a single qubit system.
   *3 Real Numbers* are needed if we need to incorporate a global phase, since $a$ would be a complex number instead of a singular real number.
<hr>

5. A source produces a beam of spin ½ qubits in the state $\ket{\psi} = \sqrt{\dfrac{9}{34}}\ket{+} +  \sqrt{\dfrac{25}{34}}e^{i\tfrac{\pi}{4}}\ket{-}$
a) Find the probability of spin up and spin down in the z-direction
$$\begin{align}
|\langle + | \psi \rangle|^2 = \left(\sqrt{\dfrac{9}{34}}\right)^2 = \dfrac{9}{34} \approx 26.47\% \\
|\langle - | \psi \rangle|^2 = \left(\sqrt{\dfrac{25}{34}}\right)^2 = \dfrac{25}{34} \approx 73.53\%
\end{align}$$
b) The output of X will be exactly 50/50 from the Z, so:
$$\begin{align}
P(x_T) = 50\% \cdot 73.53\% = 36.765\% \\
P(x_B) = 50\% \cdot 73.53\% = 36.765\%
\end{align}$$
c) Schematic of the analyzer
![[hw2q5c.jpg]]

<hr>

6. A source produces a beam of spin ½ qubits that are each prepared to be in the state $\ket{\psi} = \sqrt{\dfrac{4}{13}}\ket{X^+} + i\sqrt{\dfrac{9}{13}}\ket{X^-}$.
a) Since the probability is equal between $\ket{X^+}$ and $\ket{X^-}$ for the Z-analyzer:
$$p_{Top} = 50\% , \ \ \ p_{Bottom} = 50\%$$
b) X-Analyzer:
$$\begin{align}
|\langle X^+ | \psi \rangle|^2 &= \left(\sqrt{\dfrac{4}{13}}\right)^2 = \dfrac{4}{13} \approx 30.77\% \\
|\langle X^- | \psi \rangle|^2 &= \left|\sqrt{\dfrac{9}{13}}\right|^2 = \dfrac{9}{13} \approx 69.23\%
\end{align}$$
<hr>

7. Suppose $\ket{\psi_I} = I_+\ket{\uparrow} + I_-\ket{\downarrow}$

a) For (Alice = Z, Bob = Z):
$$\ket{\psi} =  A_+B_+ \ket{\uparrow\uparrow} + A_+B_- \ket{\uparrow\downarrow} + A_-B_+ \ket{\downarrow\uparrow} + A_-B_- \ket{\downarrow\downarrow}$$
b) For (Alice = X, Bob = Z):
$$\ket{\psi} = \left(\dfrac{\ket{\uparrow} + \ket{\downarrow}}{\sqrt{2}}\right)(B_+ \ket{\uparrow} + B_- \ket{\downarrow}) = \left(\dfrac{\ket{\uparrow} + \ket{\downarrow}}{\sqrt{2}}\right) \ket{\psi_B}$$
The rationale behind this is that, if a particle with spin up/down goes through an X gate, and then has the result decomposed back into up/down spin, the probabilities get reset to 50%/50%.

c) Recalling our result from part A, there are 4 different possible output states, resulting from the set of:   $\{\ket{\uparrow}, \ket{\downarrow}\} \times \{\ket{\uparrow}, \ket{\downarrow}\} = \{\ket{\uparrow}, \ket{\downarrow}\}^2 = \{\ket{\uparrow\uparrow}, \ket{\uparrow\downarrow}, \ket{\downarrow\uparrow}, \ket{\downarrow\downarrow}\}$
