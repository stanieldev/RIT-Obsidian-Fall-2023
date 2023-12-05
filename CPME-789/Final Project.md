- First thing to decide is the topic of your project, which is due on November 15th.


### Grover's Algorithm Time Complexity

Suppose $N=2^n$ states and $K$ solutions ($n$ is the number of Qubits in the system).
 - Let $p$, $q$ be the probability amplitude for non-solutions and solutions respectively.
 - Let $\alpha$ be the number of iterations of oracle and diffusion steps.
 - Let $r$ be the ratio of $K$ to $N$.

Base Case: After creating a uniform distribution of states, the probability amplitudes for the states are:
$$p(0)=\dfrac{1}{\sqrt{N}} \ \ \& \ \ q(0)=\dfrac{1}{\sqrt{N}}$$
Diffusion: After each use of the oracle, the probability amplitudes for the states are adjusted to accordingly:
$$\mu(\alpha) = (1-r)\cdot p(\alpha)-r\cdot q(\alpha)$$
$$\begin{align}
p(\alpha+1) &= 2\mu(\alpha) - p(\alpha) = (1-2r)\cdot p(\alpha) + (0-2r)\cdot q(\alpha)\\
q(\alpha+1) &= 2\mu(\alpha) + q(\alpha) = (2-2r)\cdot p(\alpha) + (1-2r)\cdot q(\alpha)
\end{align}$$
So it can be written as the following matrix:
$$\begin{bmatrix}p(\alpha+1)\\q(\alpha+1)\end{bmatrix}=\begin{bmatrix}1-2r&-2r\\2-2r&1-2r\end{bmatrix}\begin{bmatrix}p(\alpha)\\q(\alpha)\end{bmatrix}$$
Using the base case as our $\alpha=0$, the final result can be expressed as:
$$\begin{bmatrix}p(\alpha)\\q(\alpha)\end{bmatrix}=\dfrac{1}{\sqrt{N}}\begin{bmatrix}1-2r&-2r\\2-2r&1-2r\end{bmatrix}^\alpha\begin{bmatrix}1\\1\end{bmatrix}$$
Writing the matrix in diagonalized form and solving, the final values for each are:
$$\begin{align}
p(\alpha) &= \dfrac{-1}{\sqrt{N-K}}\sin(\omega\alpha - \phi)\\
q(\alpha) &= \dfrac{1}{\sqrt{K}}\cos(\omega\alpha - \phi)\\
\omega &= \tan^{-1}\left(\dfrac{\sqrt{K(N-K)}}{\tfrac{N}{2}-K}\right)\\
\phi &= \tan^{-1}\left(\dfrac{\sqrt{K(N-K)}}{K}\right)
\end{align}$$
The value where error is minimized is when:
$$\alpha = \dfrac{\phi}{\omega} \ \ \ \lim_{N\rightarrow\infty} \alpha = \dfrac{\pi}{4}\sqrt{\dfrac{N}{K}}$$

Total Time Complexity of the System is:
$$O(\text{Hadamard}) + \left(\tfrac{\pi}{4}\sqrt{\tfrac{N}{K}}\right)\cdot O(\text{Oracle}) + \left(\tfrac{\pi}{4}\sqrt{\tfrac{N}{K}}\right)\cdot O(\text{Diffuser})$$
$$\text{Time Complexity: } O\left(\sqrt{\tfrac{N}{K}}\right)$$
