The [**quantum Fourier transform**](https://en.wikipedia.org/wiki/Quantum_Fourier_transform) is an analogue of the discrete Fourier transform for qubits.
Compared to the classical algorithm, which takes $O(n2^n)$ gates to implement, the QFT only takes $O(n^2)$ gate.

### Intuition
The classical Fourier transform acts on a vector $x \in T_p\mathbb{C}^N$ that maps to a vector $y \in T_p\mathbb{C}^N$ by the formula:
$$y_k \equiv \dfrac{1}{\sqrt{N}}\displaystyle\sum_{j=0}^{N-1}x_j e^{\tfrac{i2\pi jk}{N}}$$
The quantum Fourier transform acts on a vector $x \in T_p\mathbb{C}^N$ that maps to a vector $y \in T_p\mathbb{C}^N$ by the formula:
$$\ket{x} \rightarrow \dfrac{1}{\sqrt{N}}\displaystyle\sum_{k=0}^{N-1}e^{\tfrac{i2\pi xk}{N}}\ket{k}$$
### Definition
The operator that acts as the Quantum Fourier Transform:
$$F = \left(\dfrac{1}{\sqrt{N}}\displaystyle\sum_{k=0}^{N-1}e^{\tfrac{i2\pi jk}{N}}\right)\ket{k}\bra{j} = F^k_j\ket{k}\bra{j}$$




