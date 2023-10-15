<hr>

### Question 1
Consider two quantum states:
$$\begin{align}
\ket{\psi_1} &= \sqrt{\dfrac{1}{3}}\ket{Z^+} + i\sqrt{\dfrac{2}{3}}\ket{Z^-} \\
\ket{\psi_2} &= \sqrt{\dfrac{1}{3}}\ket{X^+} - i\sqrt{\dfrac{2}{3}}\ket{X^-} \\
&= \left(\sqrt{\dfrac{1}{6}} - i\sqrt{\dfrac{2}{6}}\right)\ket{Z^+} + \left(\sqrt{\dfrac{1}{6}} - i\sqrt{\dfrac{2}{6}}\right)\ket{Z^-}
\end{align}$$
a) *Write each vector and covector in matrix form in the Z basis*
$$\begin{align}
\ket{\psi_1} &= \dfrac{1}{\sqrt{3}}\begin{bmatrix}1\\i\sqrt{2}\end{bmatrix} \\
\bra{\psi_1} &= \dfrac{1}{\sqrt{3}}\begin{bmatrix}1&-i\sqrt{2}\end{bmatrix} \\
\ket{\psi_2} &= \dfrac{1}{\sqrt{6}}\begin{bmatrix}1-i\sqrt{2}\\1-i\sqrt{2}\end{bmatrix} \\
\bra{\psi_2} &= \dfrac{1}{\sqrt{6}}\begin{bmatrix}1+i\sqrt{2}&1+i\sqrt{2}\end{bmatrix} \\
\end{align}$$
b) *Use the matrix representations to evaluate the cross inner products*
$$\begin{align}
\langle\psi_1|\psi_2\rangle &= \dfrac{1}{\sqrt{3}}\dfrac{1}{\sqrt{6}}\begin{bmatrix}1&-i\sqrt{2}\end{bmatrix} \begin{bmatrix}1-i\sqrt{2}\\1-i\sqrt{2}\end{bmatrix} \\
&= \dfrac{1}{\sqrt{18}}\left((1)(1-i\sqrt{2})+(-i\sqrt{2})(1-i\sqrt{2})\right) \\
&= \dfrac{1}{\sqrt{18}}\left(-1-2i\sqrt{2})\right) = -\sqrt{\dfrac{1}{18}}-i\sqrt{\dfrac{8}{18}} \\
\langle\psi_2|\psi_1\rangle &= \dfrac{1}{\sqrt{6}}\dfrac{1}{\sqrt{3}}\begin{bmatrix}1+i\sqrt{2}&1+i\sqrt{2}\end{bmatrix} \begin{bmatrix}1\\i\sqrt{2}\end{bmatrix} \\
&= \dfrac{1}{\sqrt{18}}\left((1+i\sqrt{2})(1)+(1+i\sqrt{2})(i\sqrt{2})\right) \\
&= \dfrac{1}{\sqrt{18}}\left(-1+2i\sqrt{2}\right) = -\sqrt{\dfrac{1}{18}}+i\sqrt{\dfrac{8}{18}}
\end{align}$$
c) *Find the matrix form of the cross outer product*
$$\begin{align}
\ket{\psi_2}\bra{\psi_1} &= \dfrac{1}{\sqrt{6}} \dfrac{1}{\sqrt{3}}\begin{bmatrix}1-i\sqrt{2}\\1-i\sqrt{2}\end{bmatrix} \begin{bmatrix}1&-i\sqrt{2}\end{bmatrix} \\
&= \dfrac{1}{\sqrt{18}}\begin{bmatrix}(1-i\sqrt{2})(1)&(1-i\sqrt{2})(-i\sqrt{2})\\(1-i\sqrt{2})(1)&(1-i\sqrt{2})(-i\sqrt{2}) \end{bmatrix} \\
&= \dfrac{1}{\sqrt{18}}\begin{bmatrix}1-i\sqrt{2}&-i\sqrt{2}-2\\1-i\sqrt{2}&-i\sqrt{2}-2 \end{bmatrix}
\end{align}$$

<hr>
### Question 2
The identity is a special operator
$$\mathbb{I} = \begin{bmatrix}1&0\\0&1\end{bmatrix}$$
a) *Show the Identity operator can be expressed in the Z-basis as* $\ket{Z^+}\bra{Z^+}+\ket{Z^-}\bra{Z^-}$.
$$\ket{Z^+} = \begin{bmatrix}1\\0\end{bmatrix}, \ \ \
\bra{Z^+} = \begin{bmatrix}1&0\end{bmatrix}, \ \ \
\ket{Z^-} = \begin{bmatrix}0\\1\end{bmatrix}, \ \ \
\bra{Z^-} = \begin{bmatrix}0&1\end{bmatrix}$$
$$\begin{align}
U &= \ket{Z^+}\bra{Z^+}+\ket{Z^-}\bra{Z^-} \\
&= \begin{bmatrix}1\\0\end{bmatrix}\begin{bmatrix}1&0\end{bmatrix} + \begin{bmatrix}0\\1\end{bmatrix}\begin{bmatrix}0&1\end{bmatrix} \\
&= \begin{bmatrix}1&0\\0&0\end{bmatrix}+\begin{bmatrix}0&0\\0&1\end{bmatrix} \\
&= \begin{bmatrix}1&0\\0&1\end{bmatrix} = \mathbb{I}
\end{align}$$
b) *Show the identity operator can be expressed in the X-basis as* $\ket{X^+}\bra{X^+}+\ket{X^-}\bra{X^-}$.
The usage of Z can be seen to be a dummy variable, and so can be switched to be $Z = X$, leading to the same relation as part A.

c) *What does this tell you about how the identity operator relates to a set of basis kets?*
The identity is independent of the basis that makes it up.


<hr>
### Question 3
Using a Y-Analyzer measurements

a) *If you send a particle in the $\ket{Z^+}$ state into the y-analyzer, what is the probability of the particle leaving the top and bottom ports?*
$$p_{bottom} = 50\%, \ \ \ p_{top} = 50\%$$
b) *If you send a particle in the $\ket{X^+}$ state into the y-analyzer, what is the probability of the particle leaving the top and bottom ports?*
$$p_{bottom} = 50\%, \ \ \ p_{top} = 50\%$$
Since these 2 other directions are independent of the y-axis, the probability is a uniform binary.

c) *Verify that $\ket{Y^+}$ and $\ket{Y^-}$ are eigenvectors of $\sigma_y$*.
$$\sigma_y=\begin{bmatrix}0&-i\\i&0\end{bmatrix}, \ \ \ \det\left({\begin{bmatrix}0&-i\\i&0\end{bmatrix}}-\lambda\mathbb{I}\right) = 0, \ \ \ \lambda^2-1=0 \implies \lambda = \pm 1$$
For $\lambda = 1$:
$$\begin{bmatrix}0&-i\\i&0\end{bmatrix}\begin{bmatrix}a\\b\end{bmatrix} = \begin{bmatrix}-ib\\ai\end{bmatrix} = \pm\begin{bmatrix}a\\b\end{bmatrix}$$
Leading to the relationship $b = \pm ia$
$$\ket{\lambda_{\pm1}} = \dfrac{1}{\sqrt{2}}\begin{bmatrix}1\\\pm i\end{bmatrix} \rightarrow \left\{Y^+, Y^-\right\}$$
d) *Write $\sigma_y$ as an outer product.*
$$\begin{align}
U &= i\ket{Z^-}\bra{Z^+} - i\ket{Z^+}\bra{Z^-}\\
&= i\begin{bmatrix}0\\1\end{bmatrix}\begin{bmatrix}1&0\end{bmatrix} - i\begin{bmatrix}1\\0\end{bmatrix}\begin{bmatrix}0&1\end{bmatrix}\\
&= i\begin{bmatrix}0&0\\1&0\end{bmatrix}-i\begin{bmatrix}0&1\\0&0\end{bmatrix} \\
&= \begin{bmatrix}0&-i\\i&0\end{bmatrix} = \sigma_y
\end{align}$$
e) *Use the Y-basis to check parts A and B*
Let $\ket{\psi} = \ket{Z^+}$
$$\begin{align}
\langle Y^+|\psi\rangle &=\langle Y^+|Z^+\rangle=\dfrac{1}{\sqrt2}\\
|\langle Y^+ | \psi \rangle|^2 &= \left(\dfrac{1}{\sqrt2}\right)^2 = 50\% \\
\langle Y^-|\psi\rangle &=\langle Y^-|Z^+\rangle=i\dfrac{1}{\sqrt2}\\
|\langle Y^- | \psi \rangle|^2 &= \left(\dfrac{i}{\sqrt2}\right)\left(\dfrac{-i}{\sqrt2}\right) = 50\% \\
\end{align}$$
Let $\ket{\psi} = \ket{X^+}$
$$\begin{align}
|\langle Y^+ | \psi \rangle|^2 &= \left|\dfrac{1}{\sqrt2}\right|^2 = 50\% \\
|\langle Y^- | \psi \rangle|^2 &= \left|\dfrac{1}{\sqrt2}\right|^2 = 50\% \\
\end{align}$$

<hr>
### Question 4
Particles are prepared to be in the state $\ket{\psi}=\sqrt{\dfrac{1}{5}}\ket{Z^+}+\sqrt{\dfrac{4}{5}}\ket{Z^-}$
a) *Without calculation, that port of a Z-analyzer would you expect the particles to come out of and how confident?*
$p_{bottom}=80\%,\ \ \ p_{top}=20\%$
Under the square root, 4x more particles will come out the bottom.

b) *Repeat but with an X analyzer*.
$p_{bottom}=50\%,\ \ \ p_{top}=50\%$
Regardless of the Z state, the X will be a 50/50 split, so it should be evenly balanced.

c/d) *Find the expected value and uncertainty of $\ket{\psi}$ through gate $\sigma_x$*.
$$\begin{align}
\bra{\psi} \sigma_x \ket{\psi} &= \begin{bmatrix}\sqrt{\dfrac{1}{5}}&\sqrt{\dfrac{4}{5}}\end{bmatrix} \begin{bmatrix}0&1\\1&0\end{bmatrix} \begin{bmatrix}\sqrt{\tfrac{1}{5}}\\\sqrt{\tfrac{4}{5}}\end{bmatrix} \\
\langle\hat{\sigma}_x\rangle&= \begin{bmatrix}\sqrt{\dfrac{1}{5}}&\sqrt{\dfrac{4}{5}}\end{bmatrix}  \begin{bmatrix}\sqrt{\tfrac{4}{5}}\\\sqrt{\tfrac{1}{5}}\end{bmatrix} = \dfrac{4}{5}
\end{align}$$
$$\begin{align}
\bra{\psi} (\Delta \sigma_x)^2 \ket{\psi} &= \langle\hat{\sigma}^2_x\rangle - \langle\hat{\sigma}_x\rangle^2 \\
&= 1 - \left(\dfrac{4}{5}\right)^2 = \dfrac{9}{25}
\end{align}$$
My answers are consistent with part A, but not with part B.

<hr>
### Question 5

a) Millions of detections per second means the light source is high intensity
	The photons are likely statistically random, and so lack quantum entanglement, since there is no change in outcome based on other photons.

b) Since they can only happen on one detector or the other, the photons are in a superposition of states between each direction, and when measured only shows at one detector.

c) Similar to part B, photons are in a superposition of states between each direction, but there are a small few photons that are entangled. Photons who are entangled will always have 1 photon at each detector at the same time.

d) It is possible if our light source only produced entangled-pair photons without any others being sent through the mechanism.