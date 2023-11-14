Stanley Goodwin, 11/12/2023
<hr>

![[hw3q1.png]]
1. *The figure above is a portion of one of the versions or Grover’s algorithm. 
	Show what search is being implemented based on this oracle.*

| $\ket{\psi_0}$ | $\ket{\psi_1}$ | $\ket{\psi_2}$ |
| --- | ---  | --- |
| $\ket{000}$ | $\ket{000}$ | $\ket{000}$ |
| $\ket{001}$ | $\ket{001}$ | $\ket{001}$ |
| $\ket{010}$ | $\ket{010}$ | $\ket{010}$ |
| $\ket{011}$ | $\ket{011}$ | $-\ket{011}$ |
| $\ket{100}$ | $\ket{100}$ | $\ket{100}$ |
| $\ket{101}$ | $-\ket{101}$ | $-\ket{101}$ |
| $\ket{110}$ | $\ket{110}$ | $\ket{110}$ |
| $\ket{111}$ | $-\ket{111}$ | $\ket{111}$ |

This oracle selects for the $\ket{011}$ and $\ket{101}$ states by inverting their phase relative to the rest of the possible states.
Interestingly, the order of the controlled Z gates don't have an effect on the output of the oracle.


<hr>

2. *The $\sqrt{Z}$ gate can be represented as a matrix in where each component is square rooted.
a) Represent $\sqrt{Z}$ and $C - \sqrt{Z}$.* 
$$Z = \sqrt{\begin{bmatrix}1&0\\0&-1\end{bmatrix}} = \begin{bmatrix}1&0\\0&i\end{bmatrix}$$
$$C-\sqrt{Z} = \sqrt{\begin{bmatrix}1&0&0&0\\0&1&0&0\\0&0&1&0\\0&0&0&-1\end{bmatrix}} = \begin{bmatrix}1&0&0&0\\0&1&0&0\\0&0&1&0\\0&0&0&i\end{bmatrix}$$
*b) What effect does $C - \sqrt{Z}$ have on a generic superposition of two qubits $\ket{\psi} = \alpha_0\ket{00}+\alpha_1\ket{01}+\alpha_2\ket{10}+\alpha_3\ket{11}$.*
$$\begin{align}
\left(C-\sqrt{Z}\right)\ket{\psi} &= \begin{bmatrix}1&0&0&0\\0&1&0&0\\0&0&1&0\\0&0&0&i\end{bmatrix}\begin{bmatrix}\alpha_0\\\alpha_1\\\alpha_2\\\alpha_3\end{bmatrix} = \begin{bmatrix}\alpha_0\\\alpha_1\\\alpha_2\\i\alpha_3\end{bmatrix} \\
&= \alpha_0\ket{00}+\alpha_1\ket{01}+\alpha_2\ket{10}+i\alpha_3\ket{11}
\end{align}$$

*c) What angle rotation on $\varphi$ does it represent?*
The phase of $\sqrt{Z}$ has a phase change of $\pi$, so a square-root has a the effect of $\dfrac{\pi}{2}$.
Therefore, the $\sqrt{Z}$ is equivilent of the $S$ gate or a $P$ gate of $+90\deg$.


<hr>

3. *Using Qiskit, implement a QFT for the 2 qubit case. This should result on something like in Table 1.*

| n | CB | QFT (State) | QFT (qubits $q_1,q_0$) |
| --- | ---  |  ----------- |  ----------- |
| $0$ | $\ket{00}$ | $\ket{00}+ \ \ket{01}+\ket{10}+ \ \ket{11}$ | $(\ket{0}+\ket{1}) \ (\ket{0}+ \ \ket{1})$ | 
| $1$ | $\ket{01}$ | $\ket{00}+i\ket{01}-\ket{10}-i\ket{11}$ | $(\ket{0}-\ket{1}) \ (\ket{0}+i\ket{1})$ | 
| $2$ | $\ket{10}$ | $\ket{00}- \ \ket{01}+\ket{10}- \ \ket{11}$ | $(\ket{0}+\ket{1}) \ (\ket{0}- \ \ket{1})$ | 
| $3$ | $\ket{11}$ | $\ket{00}-i\ket{01}-\ket{10}+i\ket{11}$ | $(\ket{0}-\ket{1}) \ (\ket{0}-i\ket{1})$ | 
Table 1: Quantum Fourier Transform breakdown for two qubit case.

NOTE: Circuit may be backwards since I used $\ket{\text{q[0]}, \text{q[1]}}$. I keep forgetting if the standard is little endian or big endian.
### $\ket{00}$ State
![[hw3q3_00.png]]
### $\ket{01}$ State
![[hw3q3_01.png]]
### $\ket{10}$ State
![[hw3q3_10.png]]
### $\ket{11}$ State
![[hw3q3_11.png]]


<hr>

4. *Looking at this table:
	a) How would you implement an adder using QFT? 
	b) Using Qiskit, implement a 2 qubit adder. 
	Note: Show your results paying special attention to the phase representation in the Qiskit environment.*

The simplest way to add using a QFT is to do the following:
$$\ket{a} \overset{QFT}{\rightarrow} \text{QFT}\ket{a} \overset{???}{\rightarrow} \text{QFT}\ket{a + b} \overset{QFT^\dagger}{\rightarrow} \ket{a + b}$$
The final result of the computation would then be like:
$$\ket{b}\ket{a} \rightarrow \ket{b}\ket{a + b}$$
The section with ??? is where the addition is done. Using controlled rotations based on the index of the bits of $b$ rotate the Fourier transformed $a$ only where the bit of $b$ is 1.
### $a=\ket{00}, b=\ket{01}$ State (b is Q3,Q2 and a is Q1,Q0)
![[hw3q4.png]]

| $\ket{b}$ | $\ket{a}$ | ->  | $\ket{b}$ | $\ket{a+b}$ | 
| -- | -- | -- | -- | -- |
| 01 | 01 |  | 01 | 00 |
| 00 | 01 |  | 00 | 01 |
| 01 | 00 |  | 01 | 01 |
| 00 | 00 |  | 00 | 00 |
I'm not 100% sure where I went wrong. The math of the QFT and addition is pretty clear to me, but the circuit implementation is definitely wrong. The first bit of the $\ket{a+b}$ is right, but for the 01,01 case it should be $10$ instead of $00$.

I do find it a little weird we're using the QFT for addition, but I can see why since it would take less computational steps and qubit space to do so. As for multiplication, I can definitely see a use since it's cousin DFT was used to make the least time complex multiplication algorithm for classical bits.


<hr>

5. Follow up on the previous example:
	Transform things from the phase representation back to the computational basis.

Transformations from phase to computational requires an inverse QFT transform.
It can be represented as the Hermitian conjugate of the operator, represented as $QFT^\dagger$.

Based on its matrix representation, all the powers of omega get their coefficient inverted, since the values of the roots of unity invert after a complex conjugation (rotation inverse to the original rotation).
