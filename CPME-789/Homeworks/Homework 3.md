<hr>

![[hw3q1.png]]
1. *The figure above is a portion of one of the versions or Grover’s algorithm. 
	Show what search is being implemented based on this oracle.*





<hr>
2. *The $\sqrt{Z}$ gate can be represented as a matrix in where each component is square rooted.
	a) Represent this matrix and that of $C - \sqrt{Z}$. 
	b) What effect does $C - \sqrt{Z}$ have on a generic superposition of two qubits $\ket{\psi} = \alpha_0\ket{00}+\alpha_1\ket{01}+\alpha_2\ket{10}+\alpha_3\ket{11}$.
	c) What angle rotation on $\varphi$ does it represent?*





<hr>
3. *Using Qiskit, implement a QFT for the 2 qubit case. This should result on something like in Table 1.*

| n | CB | QFT (State) | QFT (qubits $q_1,q_0$) |
| --- | ---  |  ----------- |  ----------- |
| $0$ | $\ket{00}$ | $\ket{00}+ \ \ket{01}+\ket{10}+ \ \ket{11}$ | $(\ket{0}+\ket{1}) \ (\ket{0}+ \ \ket{1})$ | 
| $1$ | $\ket{01}$ | $\ket{00}+i\ket{01}-\ket{10}-i\ket{11}$ | $(\ket{0}-\ket{1}) \ (\ket{0}+i\ket{1})$ | 
| $2$ | $\ket{10}$ | $\ket{00}- \ \ket{01}+\ket{10}- \ \ket{11}$ | $(\ket{0}+\ket{1}) \ (\ket{0}- \ \ket{1})$ | 
| $3$ | $\ket{11}$ | $\ket{00}-i\ket{01}-\ket{10}+i\ket{11}$ | $(\ket{0}-\ket{1}) \ (\ket{0}-i\ket{1})$ | 
Table 1: Quantum Fourier Transform breakdown for two qubit case.





<hr>
4. Looking at this table:
	a) How would you implement an adder using QFT? 
	b) Using Qiskit, implement a 2 qubit adder. 
	Note: Show your results paying special attention to the phase representation in the Qiskit environment.





<hr>
5. Follow up on the previous example:
	Transform things from the phase representation back to the computational basis.




