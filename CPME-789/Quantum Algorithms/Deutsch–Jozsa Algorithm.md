In the Deutsch–Jozsa problem, we are given a black box quantum computer known as an [oracle](https://en.wikipedia.org/wiki/Oracle_machine "Oracle machine") that implements some function:
$$f: \{0,1\}^n \rightarrow \{0, 1\}$$
The function takes n-bit binary values as input and produces either a 0 or a 1 as output for each such value. We are [promised](https://en.wikipedia.org/wiki/Promise_problem "Promise problem") that the function is either [constant](https://en.wikipedia.org/wiki/Constant_function "Constant function") (0 on all inputs or 1 on all inputs) or _balanced_ (1 for exactly half of the input [domain](https://en.wikipedia.org/wiki/Function_domain "Function domain") and 0 for the other half). The task then is to determine if f ![f](https://wikimedia.org/api/rest_v1/media/math/render/svg/132e57acb643253e7810ee9702d9581f159a1c61) is constant or balanced by using the oracle.

### Algorithm
Step 0: Initialization
$$\ket{\psi_0} = \ket{0}^{\otimes n} \ket{1} = \ket{x}\ket{y}$$

Step 1: Hadamard Transform
$$\begin{align}
&\ket{\psi} \rightarrow H^{\otimes(n+1)}\ket{\psi} \\
&\ket{\psi_1} = \dfrac{1}{\sqrt{2^{n+1}}} \displaystyle\sum_{x=0}^{2^n-1} \ket{x}(\ket{0}-\ket{1})
\end{align}$$
Step 2: Oracle Transformation






$$H\ket{\psi_0} = \ket{\psi_1} = $$
The oracle $U$ maps it's input state $\ket{x}\ket{y} \rightarrow \ket{x}\ket{y \oplus f(x)}$
$$\begin{align}
\ket{\psi_2} &= \dfrac{1}{\sqrt{2^{n+1}}} \displaystyle\sum_{x=0}^{2^n-1} \ket{x}(\ket{0 \oplus f(x)}-\ket{1 \oplus f(x)}) \\
&= \dfrac{1}{\sqrt{2^{n+1}}} \displaystyle\sum_{x=0}^{2^n-1} (-1)^{f(x)}\ket{x}(\ket{0}-\ket{1}) \\
\ket{\psi_3} &= \dfrac{1}{\sqrt{2^n}} \displaystyle\sum_{x=0}^{2^n-1} \ket{x}
\end{align}$$

https://en.wikipedia.org/wiki/Deutsch%E2%80%93Jozsa_algorithm

Starts with: $\ket{\psi} = \ket{0}^{\otimes n} \ket{1}$
Hadamard each bit: $\ket{\psi} = \ket{0}^{\otimes n} \ket{1}$