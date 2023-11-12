In the [Deutsch–Jozsa problem](https://en.wikipedia.org/wiki/Deutsch%E2%80%93Jozsa_algorithm), we are given a black box quantum computer known as an [oracle](https://en.wikipedia.org/wiki/Oracle_machine "Oracle machine") that implements some function:
$$f: \{0,1\}^n \rightarrow \{0, 1\}$$
The function takes n-bit binary values as input and produces either a 0 or a 1 as output for each such value. We are [promised](https://en.wikipedia.org/wiki/Promise_problem "Promise problem") that the function is either *constant* (0 on all inputs or 1 on all inputs) or _balanced_ (1 for exactly half of the input [domain](https://en.wikipedia.org/wiki/Function_domain "Function domain") and 0 for the other half). The task then is to determine if $f$ is constant or balanced by using the oracle.

### Algorithm
Step 0: Initialization
$$\ket{\psi_0} = \ket{0}^{\otimes n} \ket{1} = \ket{x}\ket{y}$$
Step 1: Hadamard Transform
$$\begin{align}
&\ket{\psi} \rightarrow H^{\otimes(n+1)}\ket{\psi} \\
&\ket{\psi_1} = \dfrac{1}{\sqrt{2^{n+1}}} \displaystyle\sum_{x=0}^{2^n-1} \ket{x}(\ket{0}-\ket{1})
\end{align}$$
Step 2: Oracle Transformation
The oracle $U_f$ maps it's input state $\ket{x}\ket{y} \rightarrow \ket{x}\ket{y \oplus f(x)}$
$$\begin{align}
\ket{\psi_2} &= \dfrac{1}{\sqrt{2^{n+1}}} \displaystyle\sum_{x=0}^{2^n-1} \ket{x}(\ket{0 \oplus f(x)}-\ket{1 \oplus f(x)}) \\
&= \dfrac{1}{\sqrt{2^{n+1}}} \displaystyle\sum_{x=0}^{2^n-1} (-1)^{f(x)}\ket{x}(\ket{0}-\ket{1}) \\
\ket{\psi_2} &= \dfrac{1}{\sqrt{2^n}} \displaystyle\sum_{x=0}^{2^n-1} \ket{x} \ \ \ \text{Last Qubit is Irrelevant}
\end{align}$$
Step 3: Hadamard Transform
$$\begin{align}
&H^{\otimes n}\ket{k} = \dfrac{1}{2^{n}} \displaystyle\sum_{y=0}^{2^n-1}\displaystyle\sum_{x=0}^{2^n-1} \left[(-1)^{f(x)}(-1)^{x\cdot y}\right]\ket{y}
\end{align}$$
### Consequences
The probability of measuring the state $\ket{k}$ to be measured is
$$\begin{align}
&H^{\otimes n}\ket{k} = \left|\dfrac{1}{2^{n}} \displaystyle\sum_{x=0}^{2^n-1} (-1)^{f(x)}(-1)^{x\cdot k}\right|^2
\end{align}$$
The probability of measuring $k=0$, corresponding to $\ket{0}^{\otimes n}$, is
$$\begin{align}
&H^{\otimes n}\ket{0} = \left|\dfrac{1}{2^{n}} \displaystyle\sum_{x=0}^{2^n-1} (-1)^{f(x)}\right|^2 = \begin{cases}1 \rightarrow f(x)\text{ is balanced}\\0 \rightarrow f(x)\text{ is constant}\end{cases}
\end{align}$$
