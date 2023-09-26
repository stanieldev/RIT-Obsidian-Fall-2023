### Standard Binary
$$\ket{0} = \begin{bmatrix} 1 \\ 0 \end{bmatrix}, \ \ket{1} = \begin{bmatrix} 0 \\ 1 \end{bmatrix}$$
### Hadamard Binary
$$\ket{+} = \dfrac{1}{\sqrt{2}}\ket{0} + \dfrac{1}{\sqrt{2}}e^{i0}\ket{1}, \ \ket{-} = \dfrac{1}{\sqrt{2}}\ket{0} + \dfrac{1}{\sqrt{2}}e^{i\pi}\ket{1}$$
### Imaginary Diagonal Binary
$$\ket{i} = \dfrac{1}{\sqrt{2}} \begin{bmatrix} 1 \\ i \end{bmatrix}, \ \ket{-i} = \dfrac{1}{\sqrt{2}} \begin{bmatrix} 1 \\ -i \end{bmatrix}$$
### Pauli Bivector + Pseudoscalar Basis
Since the Pauli matrices are a representation of a 3D vector as a 2x2 matrix, multiplying by the unit pseudoscalar on these vectors leads to the bivectors:
$$\begin{align}
I &= i \mathbb{I}, \ \hat{\Sigma}_x = i\sigma_x, \ \hat{\Sigma}_y = i\sigma_y, \ \hat{\Sigma}_z = i\sigma_z \\
R_i(\theta) &= e^{\hat{\Sigma}_i \left(\tfrac{\theta}{2}\right)} = \cos\left(\dfrac{\theta}{2}\right) + \hat{\Sigma}_i\sin\left(\dfrac{\theta}{2}\right)\\
R_i^\dagger(\theta) &= e^{-\hat{\Sigma}_i \left(\tfrac{\theta}{2}\right)} = \cos\left(\dfrac{\theta}{2}\right) - \hat{\Sigma}_i\sin\left(\dfrac{\theta}{2}\right)
\end{align}$$
Where the square of each element is
$$ \hat{E}_\mathbb{I}^2 = \hat{E}_x^2 = \hat{E}_y^2 = \hat{E}_z^2 = -1 $$
as opposed to the Pauli Vector + Identity
$$ \mathbb{I}^2 = \sigma_x^2 = \sigma_y^2 = \sigma_z^2 = +1 $$
