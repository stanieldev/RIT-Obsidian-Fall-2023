
### Question 1
Given the state (q1 is the left qubit, q0 is the one on the right): $$\ket{\psi} = \sqrt{\dfrac{3}{10}}\ket{00} + \sqrt{\dfrac{1}{10}}\ket{01} + \sqrt{\dfrac{5}{10}}\ket{10} + \sqrt{\dfrac{1}{10}}\ket{11}$$a) *What is the probability of measuring qubit 1 in state $\ket{1}$?*
$$p(\ket{1,x}) = \left(\sqrt{\dfrac{5}{10}}\right)^2+\left(\sqrt{\dfrac{1}{10}}\right)^2 = 60\%$$
b) *What is the state of the system after the measurement?*
$$\ket{\psi'} = \sqrt{\dfrac{5}{6}}\ket{10} + \sqrt{\dfrac{1}{6}}\ket{11}$$
### Question 2
Which pairs of quantum states represent the same state?

a) $\ket{\psi} = \dfrac{1}{\sqrt{2}}(\ket{0}-\ket{1})$ and $\ket{\phi} = \dfrac{1}{\sqrt{2}}(\ket{1}-\ket{0})$
$\ket{\psi} = e^{i\pi}\ket{\phi}$, so they are identical ignoring a global phase. Their relative phase stays intact.

b) $\ket{\psi} = \ket{0}$ and $\ket{\phi} = -\ket{0}$
$\ket{\psi} = e^{i\pi}\ket{\phi}$, so they are identical ignoring a global phase. Their relative phase stays intact.

c) $\ket{\psi} = \dfrac{1}{\sqrt{2}}\left(\ket{0}+e^{i\tfrac{\pi}{4}}\ket{1}\right)$ and $\ket{\phi} = \dfrac{1}{\sqrt{2}}\left(e^{-i\tfrac{\pi}{4}}\ket{0}+\ket{1}\right)$
$\ket{\psi} = e^{i\tfrac{\pi}{2}}\ket{\phi}$, so they are identical ignoring a global phase. Their relative phase stays intact.

d) $\ket{\psi} = \ket{i}$ and $\ket{\phi} = \ket{+}$
$\ket{i} = \dfrac{1}{\sqrt{2}} (\ket{0} + i\ket{1}), \ \ \ \ket{+} = \dfrac{1}{\sqrt{2}}(\ket{0} + \ket{1})$
There is no rotor transform that converts between $\ket{i}$ and $\ket{+}$,
They are not the same since the phase of $\ket{1}$ changes by itself.

### Question 3
Prove that $X R_y(\theta) X = R_y(-\theta)$
$$\begin{align}
R_k(\theta) &= e^{(i\sigma_k) \tfrac{\theta}{2}} = \cos\left(\tfrac{\theta}{2}\right)\mathbb{1} + (i\sigma_k)\sin\left(\tfrac{\theta}{2}\right) \\
\sigma_x R_k(\theta) \sigma_x &= \sigma_x (\cos\left(\tfrac{\theta}{2}\right)\mathbb{1} + (i\sigma_k)\sin\left(\tfrac{\theta}{2}\right)) \sigma_x \\
&= \sigma_x^2\cos\left(\tfrac{\theta}{2}\right)\mathbb{1} - \sigma_x^2(i\sigma_k)\sin\left(\tfrac{\theta}{2}\right) \\
&= \cos\left(-\tfrac{\theta}{2}\right)\mathbb{1} + (i\sigma_k)\sin\left(-\tfrac{\theta}{2}\right) \\
&= R_k(-\theta) \\
\implies R_k(-\theta) &= \sigma_x R_k(\theta) \sigma_x, \ \ \ k \in \{x,y,z\} \\
\implies R_y(-\theta) &= \sigma_x R_y(\theta) \sigma_x, \ \ \ R_z(-\theta) = \sigma_x R_z(\theta) \sigma_x
\end{align}$$

### Question 4
$$H \otimes H = H^{\otimes2} = \dfrac{1}{2}\begin{bmatrix} 1 & 1 & 1 & 1 \\ 1 & -1 & 1 & -1 \\ 1 & 1 & -1 & -1 \\ 1 & -1 & -1 & 1 \end{bmatrix}, \ \ \ \text{c-}X = \begin{bmatrix}1&0&0&0\\0&1&0&0\\0&0&0&1\\0&0&1&0\end{bmatrix}$$
$$U = H^{\otimes2}(\text{c-}X)H^{\otimes2} = \begin{bmatrix}1&0&0&0\\0&0&0&1\\0&0&1&0\\0&1&0&0\end{bmatrix}, \ \ \ \ket{\psi} \rightarrow U\ket{\psi}$$
$$\ket{++} = \dfrac{1}{2}\begin{bmatrix}1\\1\\1\\1\end{bmatrix} \implies U\ket{++} = \dfrac{1}{2}\begin{bmatrix}1&0&0&0\\0&0&0&1\\0&0&1&0\\0&1&0&0\end{bmatrix}\begin{bmatrix}1\\1\\1\\1\end{bmatrix} = \dfrac{1}{2}\begin{bmatrix}1\\1\\1\\1\end{bmatrix} = \ket{++}$$
![[hw2q4.png]]

### Question 5
![[hw2q5.png]]
$$\begin{align}
\ket{\Psi_0} &= \dfrac{1}{\sqrt{2}}(\ket{0}\ket{+}\ket{-}+\ket{1}\ket{+}\ket{-}) \\
\ket{\Psi_1} &= \dfrac{1}{\sqrt{2}}(\ket{0}\ket{+}\ket{-}+\ket{1}\ket{-}\ket{+}) \\
\ket{\Psi_2} &= \dfrac{1}{\sqrt{2}}\dfrac{1}{\sqrt{2}}(\ket{0}\ket{+}\ket{-}+\ket{1}\ket{+}\ket{-}+\ket{0}\ket{-}\ket{+}-\ket{1}\ket{-}\ket{+}) \\
&= \ket{0}\left(\dfrac{\ket{+}\ket{-} + \ket{-}\ket{+}}{2}\right) + \ket{1}\left(\dfrac{\ket{+}\ket{-} - \ket{-}\ket{+}}{2}\right)
\end{align}$$
Why would I use the decomposition when I can use the direct swap relation with my states?
Also since they're orthonormal states, then the measured probability comes to be
$$||\langle0|\Psi\rangle||^2 = 50\%, \ \ \ ||\langle1|\Psi\rangle||^2 = 50\%$$
for the output classical measurement at Q0.

### Question 6
![[hw2q6.png]]
