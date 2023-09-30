### Pauli Matrices
[Pauli Matrices Wikipedia](https://en.wikipedia.org/wiki/Pauli_matrices)
$$I = \begin{bmatrix} 1 & 0 \\ 0 & 1 \end{bmatrix}, \ \sigma_x = \begin{bmatrix} 0 & 1 \\ 1 & 0 \end{bmatrix}, \ \sigma_y = i\begin{bmatrix} 0 & -1 \\ 1 & 0 \end{bmatrix}, \ \sigma_z = \begin{bmatrix} 1 & 0 \\ 0 & -1 \end{bmatrix}$$
## Single-Qubit Gates
Single-qubit gates are linear transform matrices that preserve Unitary and Hermitian properties.
All gates can be expressed as a sum of tensor products of degree N with the basis of states.
### Hadamard Gate
$$H = \dfrac{1}{\sqrt{2}}\begin{bmatrix} 1 & 1 \\ 1 & -1 \end{bmatrix}$$
### Outer Product Form
$$\begin{align}
I &= \ \ \ \ket{0}\bra{0} + \ket{1}\bra{1} = \ \ \ \ \ket{00} + \ket{11}\\
\sigma_x &= \ \ \ \ket{0}\bra{1} + \ket{1}\bra{0} = \ \ \ \ \ket{10} + \ket{01} \\
\sigma_y &= i(\ket{1}\bra{0} -\ket{0}\bra{1}) = i(\ket{10} - \ket{01}) \\
\sigma_z &= \ \ \ \ket{0}\bra{0} - \ket{1}\bra{1} = \ \ \ \ \ket{00} - \ket{11} \\
H &= \dfrac{1}{\sqrt{2}}\left(\ket{0}\bra{0} + \ket{0}\bra{1} + \ket{1}\bra{0} - \ket{1}\bra{1}\right)
\end{align}$$
### Rotors
$$\begin{align}
R_x(\theta) = e^{(i\sigma_x) \tfrac{\theta}{2}} = \cos\left(\tfrac{\theta}{2}\right)\mathbb{1} + (i\sigma_x)\sin\left(\tfrac{\theta}{2}\right) \\
R_y(\theta) = e^{(i\sigma_y) \tfrac{\theta}{2}} = \cos\left(\tfrac{\theta}{2}\right)\mathbb{1} + (i\sigma_y)\sin\left(\tfrac{\theta}{2}\right) \\
R_z(\theta) = e^{(i\sigma_z) \tfrac{\theta}{2}} = \cos\left(\tfrac{\theta}{2}\right)\mathbb{1} + (i\sigma_z)\sin\left(\tfrac{\theta}{2}\right)
\end{align}$$
## Multi-Qubit Gates
Multi-qubit gates can be constructed from single-qubit gates using the [[Tensor Product\|tensor product]] or by manually evaluating inputs and outputs.
### Controlled X
$$\text{c-}X = \begin{bmatrix}1&0&0&0\\0&1&0&0\\0&0&0&1\\0&0&1&0\end{bmatrix}$$
### Controlled U
$$\text{c-}U = \begin{bmatrix}1&0&0&0\\0&1&0&0\\0&0&u_{00}&u_{01}\\0&0&u_{10}&u_{11}\end{bmatrix}$$
