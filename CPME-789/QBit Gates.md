### Pauli Matrices
[Pauli Matrices Wikipedia](https://en.wikipedia.org/wiki/Pauli_matrices)
$$I = \begin{bmatrix} 1 & 0 \\ 0 & 1 \end{bmatrix}, \ \sigma_x = \begin{bmatrix} 0 & 1 \\ 1 & 0 \end{bmatrix}, \ \sigma_y = \begin{bmatrix} 0 & -i \\ i & 0 \end{bmatrix}, \ \sigma_z = \begin{bmatrix} 1 & 0 \\ 0 & -1 \end{bmatrix}$$
### Hadamard Gate
$$H = \dfrac{1}{\sqrt{2}}\begin{bmatrix} 1 & 1 \\ 1 & -1 \end{bmatrix}$$
### Outer Product Form
$$\begin{align}
I &= \ket{0}\bra{0} + \ket{1}\bra{1} \\
\sigma_x &= \ket{0}\bra{1} + \ket{1}\bra{0} \\
\sigma_y &= -i\ket{0}\bra{1} + i\ket{1}\bra{0} \\
\sigma_z &= \ket{0}\bra{0} - \ket{1}\bra{1} \\
H &= \dfrac{1}{\sqrt{2}}\left(\ket{0}\bra{0} + \ket{0}\bra{1} + \ket{1}\bra{0} - \ket{1}\bra{1}\right)
\end{align}$$
### Rotors
$$\begin{align}
R_x(\theta) = e^{(i\sigma_x) \tfrac{\theta}{2}} = \cos\left(\tfrac{\theta}{2}\right)\mathbb{1} + (i\sigma_x)\sin\left(\tfrac{\theta}{2}\right) \\
R_y(\theta) = e^{(i\sigma_y) \tfrac{\theta}{2}} = \cos\left(\tfrac{\theta}{2}\right)\mathbb{1} + (i\sigma_y)\sin\left(\tfrac{\theta}{2}\right) \\
R_z(\theta) = e^{(i\sigma_z) \tfrac{\theta}{2}} = \cos\left(\tfrac{\theta}{2}\right)\mathbb{1} + (i\sigma_z)\sin\left(\tfrac{\theta}{2}\right)
\end{align}$$



