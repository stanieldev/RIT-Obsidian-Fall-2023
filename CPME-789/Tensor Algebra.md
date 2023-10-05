Let a vector space $V = \{\ket{0}, \ket{1}\}$ be an orthonormal basis
$$T(V) = \displaystyle\bigoplus_{k=0}^\infty T^kV = K \oplus V \oplus (V \otimes V) \oplus (V \otimes V \otimes V) \oplus \ldots$$



### Pauli Basis
Instead, lets have a Vector Space of Pauli Vectors
Let a vector space $V = \{\sigma_x, \sigma_y, \sigma_z\}$
$$ T(V) = 1 + \sigma_i + \sigma_i\sigma_j + \sigma_i\sigma_j\sigma_k+\ldots$$
Using the property that $\sigma_i^2 = +1$ and $\sigma_i\sigma_j = -\sigma_j\sigma_i$
$$\begin{align}
T(V) &= 1 + \sigma_x + \sigma_y + \sigma_z \\
&+\sigma_x\sigma_y + \sigma_y\sigma_z + \sigma_z\sigma_x \\
&+ \sigma_x\sigma_y\sigma_z
\end{align}$$
So we can also express the tensor field as
$$\begin{align}
T(V) &= 1 + \vec{\sigma} + i\vec{\sigma} + i \\
&= 1 + \vec{\sigma} + \vec{\Sigma} + i
\end{align}$$
$$ 1^2 = \sigma_x^2 = \sigma_y^2 = \sigma_z^2 = +1$$
$$ i^2 = \Sigma_x^2 = \Sigma_y^2 = \Sigma_z^2 = -1$$
### Euler's Equations
$$\begin{align}
e^{1\theta} &= \cosh{\theta} + \sinh{\theta} \\
e^{\sigma_k\theta} &= \cosh{\theta} + \sigma_k\sinh{\theta} \\
e^{\Sigma_k\theta} &= \cos{\theta} + \Sigma_k\sin{\theta} \\
e^{i\theta} &= \cos{\theta} + i\sin{\theta} \\
\end{align}$$
