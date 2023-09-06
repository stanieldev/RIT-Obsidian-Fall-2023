### Dirac Notation (ket notation)
$$\ket{0}, \ket{1}$$
#### Inner Product
$$ \braket{x|y}  = \displaystyle\sum x_i^* y_i $$
Where
$$ \bra{x} = \ket{y}^\dagger = \left(\ket{y}^T\right)^*$$

#### Outer Product
$$ \ket{x} \bra{y} = \displaystyle\sum_{i \ne j} \left(x_iy_j^*\right) \ket{e_i} \bra{e_j} $$
$\ket{0}\bra{0} = \begin{bmatrix} 1 & 0 \\ 0 & 0 \end{bmatrix}$, $\ket{0}\bra{1} = \begin{bmatrix} 0 & 1 \\ 0 & 0 \end{bmatrix}$, $\ket{1}\bra{0} = \begin{bmatrix} 0 & 0 \\ 1 & 0 \end{bmatrix}$, $\ket{1}\bra{1} = \begin{bmatrix} 0 & 0 \\ 0 & 1 \end{bmatrix}$

Identity Gate:  $I = \ket{0}\bra{0} + \ket{1}\bra{1} = \begin{bmatrix} 1 & 0 \\ 0 & 0 \end{bmatrix} + \begin{bmatrix} 0 & 0 \\ 0 & 1 \end{bmatrix} = \begin{bmatrix} 1 & 0 \\ 0 & 1 \end{bmatrix}$
C-NOT Gate:  $X = \ket{0}\bra{1} + \ket{1}\bra{0}  = \begin{bmatrix} 0 & 1 \\ 0 & 0 \end{bmatrix} + \begin{bmatrix} 0 & 0 \\ 1 & 0 \end{bmatrix} = \begin{bmatrix} 0 & 1 \\ 1 & 0 \end{bmatrix}$
Hadamard Gate:  $H = \dfrac{1}{\sqrt{2}}\left(\ket{0}\bra{0} + \ket{0}\bra{1} + \ket{1}\bra{0} - \ket{1}\bra{1}\right) = \dfrac{1}{\sqrt{2}}\begin{bmatrix} 1 & 1 \\ 1 & -1 \end{bmatrix}$





### Matrix Notation
$$ \ket{0} = \begin{bmatrix} 1 \\ 0 \end{bmatrix}, \ket{1} = \begin{bmatrix} 0 \\ 1 \end{bmatrix} $$
#### Dot Product
$$ \vec{x} \cdot \vec{y} = \displaystyle\sum x_i y_i $$

### Quantum Basis
#### Orthonormality
$$ \braket{\psi_i|\psi_j} = \delta_{ij}$$

### Example
$\ket{\psi} = \dfrac{3}{5}\ket{0} - \dfrac{4}{5}e^{\frac{\pi}{6}i}\ket{1}$

$\braket{\psi|\psi} = \left(\dfrac{3}{5}\right)^2 + \left(\dfrac{4}{5}\right)^2 e^{\frac{\pi}{6}i} e^{-\frac{\pi}{6}i} = 1 \ \ \blacksquare$

$H\ket{x} = \dfrac{1}{\sqrt{2}}\begin{bmatrix} 1 & 1 \\ 1 & -1 \end{bmatrix} \begin{bmatrix} \alpha \\ \beta \end{bmatrix} = \alpha \ket{+} + \beta \ket{-}$

#### For the sake of not going insane:
$$ -1 = e^{i \pi} $$
#### The Hadamard Basis:
$\ket{+} = \dfrac{1}{\sqrt{2}}\ket{0} + \dfrac{1}{\sqrt{2}}e^{i0}\ket{1}$
$\ket{-} = \dfrac{1}{\sqrt{2}}\ket{0} + \dfrac{1}{\sqrt{2}}e^{i\pi}\ket{1}$
