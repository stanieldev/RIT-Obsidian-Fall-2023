

The [**quantum Fourier transform**](https://en.wikipedia.org/wiki/Quantum_Fourier_transform) is an analogue of the discrete Fourier transform for qubits.
Compared to the classical algorithm, which takes $O(n2^n)$ gates to implement, the QFT only takes $O(n^2)$ gate.

### Definition
The classical Fourier transform acts on a vector $x \in L_p\mathbb{C}^N$ that maps to a vector $y \in L_p\mathbb{C}^N$ by the formula:
$$y_k=\dfrac{1}{\sqrt{N}}\displaystyle\sum_{n=0}^{N-1}x_n\omega^{-nk}_N$$
