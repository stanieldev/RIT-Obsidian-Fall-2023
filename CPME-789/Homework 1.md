**Latex Snippets**
$$\sigma_x = \begin{bmatrix} 0 & 1 \\ 1 & 0 \end{bmatrix}, \ \sigma_y = \begin{bmatrix} 0 & -i \\ i & 0 \end{bmatrix}, \ \sigma_z = \begin{bmatrix} 1 & 0 \\ 0 & -1 \end{bmatrix}, \ H = \dfrac{1}{\sqrt{2}}\begin{bmatrix} 1 & 1 \\ 1 & -1 \end{bmatrix}$$
$$\ket{i} = \dfrac{1}{\sqrt{2}} \begin{bmatrix} 1 \\ i \end{bmatrix}, \ \ket{-i} = \dfrac{1}{\sqrt{2}} \begin{bmatrix} 1 \\ -i \end{bmatrix}, \ \ket{+} = \dfrac{1}{\sqrt{2}} \begin{bmatrix} 1 \\ 1 \end{bmatrix}, \ \ket{-} = \dfrac{1}{\sqrt{2}} \begin{bmatrix} 1 \\ -1 \end{bmatrix}$$


1. What is the inner product between the real vectors $(0,1)$ and $(1,1)$? What is the inner product between the states $\ket{01}$ and $\ket{11}$? Show your work.

$\begin{bmatrix} 0 \\ 1 \end{bmatrix} \cdot \begin{bmatrix} 1 \\ 1 \end{bmatrix} = 0 \cdot 1 + 1 \cdot 1 = \fbox{1}, \ \ \ \ket{01} \cdot \ket{11} = \begin{bmatrix} 0 \\ 1 \\ 0 \\ 0 \end{bmatrix} \cdot \begin{bmatrix} 0 \\ 0 \\ 0 \\ 1\end{bmatrix} = 0 \cdot 0 + 1 \cdot 0 + 0 \cdot 0 + 0 \cdot 1 = \fbox{0}$


2. Compute the result of applying the Hadamard operand to qubits $\ket{0} \otimes \ket{1}$in two ways: $(H\ket{0}) \otimes (H\ket{1})$ and $(H \otimes H)(\ket{0} \otimes \ket{1})$. How show that both are equivalent.
$$\begin{align} (H\ket{0}) \otimes (H\ket{1}) &= \left(\dfrac{1}{\sqrt{2}}\begin{bmatrix} 1 & 1 \\ 1 & -1 \end{bmatrix}\begin{bmatrix} 1 \\ 0 \end{bmatrix}\right) \otimes \left(\dfrac{1}{\sqrt{2}}\begin{bmatrix} 1 & 1 \\ 1 & -1 \end{bmatrix} \begin{bmatrix} 0 \\ 1 \end{bmatrix}\right) \\ &= \dfrac{1}{2}\left(\begin{bmatrix} 1 \\ 1 \end{bmatrix} \otimes\begin{bmatrix} 1 \\ -1 \end{bmatrix}\right) = \dfrac{1}{2}\begin{bmatrix} 1 \cdot \begin{bmatrix} 1  \\ -1 \end{bmatrix} \\ 1 \cdot \begin{bmatrix} 1 \\ -1 \end{bmatrix} \end{bmatrix} = \dfrac{1}{2}\begin{bmatrix} 1  \\ -1 \\ 1 \\ -1 \end{bmatrix} \\ &= \dfrac{1}{2} (\ket{00} - \ket{01} + \ket{10} - \ket{11}) \end{align}$$
$$\begin{align} (H \otimes H)(\ket{0} \otimes \ket{1}) &= \left(\dfrac{1}{\sqrt{2}}\begin{bmatrix} 1 & 1 \\ 1 & -1 \end{bmatrix} \otimes \dfrac{1}{\sqrt{2}}\begin{bmatrix} 1 & 1 \\ 1 & -1 \end{bmatrix}\right)\left(\begin{bmatrix} 1 \\ 0 \end{bmatrix} \otimes \begin{bmatrix} 0\\ 1 \end{bmatrix}\right) \\ &= \dfrac{1}{2}\begin{bmatrix} 1 \cdot \begin{bmatrix} 1 & 1 \\ 1 & -1 \end{bmatrix} & 1 \cdot \begin{bmatrix} 1 & 1 \\ 1 & -1 \end{bmatrix} \\ 1 \cdot \begin{bmatrix} 1 & 1 \\ 1 & -1 \end{bmatrix} & -1 \cdot \begin{bmatrix} 1 & 1 \\ 1 & -1 \end{bmatrix} \end{bmatrix} \begin{bmatrix} 1 \cdot \begin{bmatrix} 0\\ 1 \end{bmatrix} \\ 0 \cdot \begin{bmatrix} 0\\ 1 \end{bmatrix} \end{bmatrix} \\ &= \dfrac{1}{2}\begin{bmatrix} 1 & 1 & 1 & 1 \\ 1 & -1 & 1 & -1 \\ 1 & 1 & -1 & -1 \\ 1 & -1 & -1 & 1\end{bmatrix} \begin{bmatrix}0\\1\\0\\0\end{bmatrix} = \dfrac{1}{2} \begin{bmatrix} 1 \\ -1 \\ 1 \\ -1 \end{bmatrix} \\ &= \dfrac{1}{2} (\ket{00} - \ket{01} + \ket{10} - \ket{11})\end{align} $$
$$\psi = \dfrac{1}{\sqrt{4}}\ket{00} - \dfrac{1}{\sqrt{4}}\ket{01} + \dfrac{1}{\sqrt{4}}\ket{10} - \dfrac{1}{\sqrt{4}}\ket{11}$$

3. Implement the circuit above in Qiskit’s circuit composer (show a capture of the circuit) and show the result in the probability distribution and block spheres.
![[hw1q3.png]]


4. Show that the spectral decomposition of $\sigma_y$  is $\sigma_y = \ket{i}\bra{i} - \ket{-i}\bra{-i}$
$$\begin{align} \sigma_y &= \dfrac{1}{\sqrt{2}} \begin{bmatrix} 1 \\ i \end{bmatrix} \dfrac{1}{\sqrt{2}} \begin{bmatrix} 1 \\ i \end{bmatrix}^\dagger - \dfrac{1}{\sqrt{2}} \begin{bmatrix} 1 \\ -i \end{bmatrix} \dfrac{1}{\sqrt{2}} \begin{bmatrix} 1 \\ -i \end{bmatrix}^\dagger \\ &= \dfrac{1}{2}\left(\begin{bmatrix} 1 \\ i \end{bmatrix} \begin{bmatrix} 1 & -i \end{bmatrix} - \begin{bmatrix} 1 \\ -i \end{bmatrix} \begin{bmatrix} 1 & i \end{bmatrix}\right) \\ &= \dfrac{1}{2}\left(\begin{bmatrix} 1 & -i \\ i & 1 \end{bmatrix} - \begin{bmatrix} 1 & i \\ -i & 1 \end{bmatrix}\right) \\ &= \dfrac{1}{2}\begin{bmatrix} 1-1 & -i-i \\ i+i & 1-1 \end{bmatrix} = \dfrac{1}{2}\begin{bmatrix} 0 & -2i \\ 2i & 0 \end{bmatrix} = \begin{bmatrix} 0 & -i \\ i & 0 \end{bmatrix} \end{align}$$

5. Show that the Pauli matrices are unitary and Hermitian.
Unitary: $U^\dagger U = I$, \ \ \ Hermitian: $A^\dagger = A$

Hermitian Proofs:
$\sigma_x^\dagger = \begin{bmatrix} 0 & 1 \\ 1 & 0 \end{bmatrix}^\dagger = \begin{bmatrix} 0 & 1 \\ 1 & 0 \end{bmatrix} = \sigma_x$
$\sigma_y^\dagger = \begin{bmatrix} 0 & -i \\ i & 0 \end{bmatrix}^\dagger = \begin{bmatrix} 0 & i \\ -i & 0 \end{bmatrix}^T = \begin{bmatrix} 0 & -i \\ i & 0 \end{bmatrix} = \sigma_y$
$\sigma_z^\dagger = \begin{bmatrix} 1 & 0 \\ 0 & -1 \end{bmatrix}^\dagger = \begin{bmatrix} 1 & 0 \\ 0 & -1 \end{bmatrix} = \sigma_z$

Unitary Proofs:
$\sigma_x^\dagger \sigma_x = \sigma_x^2 = \begin{bmatrix} 0 & 1 \\ 1 & 0 \end{bmatrix}^2 = \begin{bmatrix} 0\cdot0+1\cdot1 & 0\cdot1 + 1\cdot0 \\ 1\cdot0+0\cdot1 & 1\cdot1+0\cdot0 \end{bmatrix} = \begin{bmatrix} 1 & 0 \\ 0 & 1 \end{bmatrix} = I$
$\sigma_y^\dagger \sigma_y = \sigma_y^2 = \begin{bmatrix} 0 & -i \\ i & 0 \end{bmatrix}^2 = \begin{bmatrix} 0\cdot0+(-i)\cdot i & 0\cdot (-i) + (-i)\cdot0 \\ i\cdot0+0\cdot i & i\cdot(-i)+0\cdot0 \end{bmatrix} = \begin{bmatrix} 1 & 0 \\ 0 & 1 \end{bmatrix} = I$
$\sigma_z^\dagger \sigma_z = \sigma_z^2 = \begin{bmatrix} 1 & 0 \\ 0 & -1 \end{bmatrix}^2 = \begin{bmatrix} 1\cdot1+0\cdot0 & 1\cdot0+0\cdot(-1) \\ 0\cdot1 + (-1)\cdot0 & 0\cdot0+1\cdot1 \end{bmatrix} = \begin{bmatrix} 1 & 0 \\ 0 & 1 \end{bmatrix} = I$
