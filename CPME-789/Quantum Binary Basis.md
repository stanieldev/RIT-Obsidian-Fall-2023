### Standard Binary
$$\ket{0} = \begin{bmatrix} 1 \\ 0 \end{bmatrix}, \ \ket{1} = \begin{bmatrix} 0 \\ 1 \end{bmatrix}$$
### Hadamard Binary
$$\ket{+} = \dfrac{1}{\sqrt{2}}\ket{0} + \dfrac{1}{\sqrt{2}}e^{i0}\ket{1}, \ \ket{-} = \dfrac{1}{\sqrt{2}}\ket{0} + \dfrac{1}{\sqrt{2}}e^{i\pi}\ket{1}$$
### Imaginary Diagonal Binary
$$\ket{i} = \dfrac{1}{\sqrt{2}} \begin{bmatrix} 1 \\ i \end{bmatrix}, \ \ket{-i} = \dfrac{1}{\sqrt{2}} \begin{bmatrix} 1 \\ -i \end{bmatrix}$$
### Pauli Bivector Basis
$$\begin{align}
\hat{E}_0 &= i I, \ \hat{E}_1 = i\sigma_x, \ \hat{E}_2 = i\sigma_y, \ \hat{E}_3 = i\sigma_z \\
R_i(\theta) &= e^{\hat{E_i} \left(\tfrac{\theta}{2}\right)} = \cos\left(\dfrac{\theta}{2}\right) + \hat{E_i}\sin\left(\dfrac{\theta}{2}\right)\\
R_i^\dagger(\theta) &= e^{-\hat{E_i} \left(\tfrac{\theta}{2}\right)} = \cos\left(\dfrac{\theta}{2}\right) - \hat{E_i}\sin\left(\dfrac{\theta}{2}\right)
\end{align}$$