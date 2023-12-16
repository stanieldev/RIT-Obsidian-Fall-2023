
<hr>

### Question 1
$$\widehat{U}_{bs} = \dfrac{1}{\sqrt{2}}\begin{bmatrix}1&i\\i&1\end{bmatrix} \ \ \ \ \ \widehat{U} = \dfrac{1}{\sqrt{2}}\begin{bmatrix}1&1\\1&-1\end{bmatrix}$$
a) *Is the “new” beam-splitter operator $\widehat{U}$" a unitary operator?*
$$\begin{align}
\widehat{U}^\dagger\widehat{U} &= \dfrac{1}{\sqrt{2}}\begin{bmatrix}1&1\\1&-1\end{bmatrix}\dfrac{1}{\sqrt{2}}\begin{bmatrix}1&1\\1&-1\end{bmatrix} \\
&= \dfrac{1}{2}\begin{bmatrix}1&1\\1&-1\end{bmatrix}^2 = \dfrac{2}{2}\begin{bmatrix}1&0\\0&1\end{bmatrix} = \boxed{\mathbb{I}}
\end{align}$$
b) *You send a single photon into port $P_0$ of the “new” beam-splitter. What are the probabilities of detecting the photon in output paths 2 and 3 respectively?*
$$\begin{align}
\widehat{U}\ket{\psi_\mathrm{in}} &= \dfrac{1}{\sqrt{2}}\begin{bmatrix}1&1\\1&-1\end{bmatrix}\begin{bmatrix}\alpha\\\beta\end{bmatrix}\\
&= \dfrac{1}{\sqrt{2}}\begin{bmatrix}\alpha+\beta\\\alpha-\beta\end{bmatrix}
\end{align}$$
$$p(\widehat{U}\ket{\psi_\mathrm{in}} = \ket{0}) = (\alpha+\beta)^2$$
$$p(\widehat{U}\ket{\psi_\mathrm{in}} = \ket{1}) = (\alpha-\beta)^2$$
This is already a good indicator that the new operator is not identical to the derived one. There are no points in which you can choose $\alpha$ and $\beta$ that leads to a 50/50 output, only 100% one way or 100% the other way.

c/d) *Construct a balanced interferometer. What's the probability of the photon being on the output paths $P_4$ and $P_5$ for both beam splitters.*
#### New beam splitter
$$\begin{align}
\widehat{U}^2\ket{\psi_\mathrm{in}} &= \dfrac{1}{\sqrt{2}^2}\begin{bmatrix}1&1\\1&-1\end{bmatrix}^2\begin{bmatrix}\alpha\\\beta\end{bmatrix} = \begin{bmatrix}\alpha\\\beta\end{bmatrix}
\end{align}$$
$$p\left(\widehat{U}^2\ket{\psi_\mathrm{in}} = \ket{0}\right) = \alpha^2$$
$$p\left(\widehat{U}^2\ket{\psi_\mathrm{in}} = \ket{1}\right) = \beta^2$$
#### Our beam splitter
$$\begin{align}
\widehat{U}^2_\mathrm{bs}\ket{\psi_\mathrm{in}} &= \dfrac{1}{\sqrt{2}^2}\begin{bmatrix}1&i\\i&1\end{bmatrix}^2\begin{bmatrix}\alpha\\\beta\end{bmatrix}\\
&= \dfrac{2}{2}\begin{bmatrix}0&i\\i&0\end{bmatrix}\begin{bmatrix}\alpha\\\beta\end{bmatrix} = \begin{bmatrix}i\beta\\i\alpha\end{bmatrix}
\end{align}$$
$$p\left(\widehat{U}^2_\mathrm{bs}\ket{\psi_\mathrm{in}} = \ket{0}\right) = (-i\beta)(i\beta) = \beta^2$$
$$p\left(\widehat{U}^2_\mathrm{bs}\ket{\psi_\mathrm{in}} = \ket{1}\right) = (-i\alpha)(i\alpha) = \alpha^2$$
The 2 different beam splitter operators gave me 2 different outputs, where the Hadamard operator had no final effect on the input state, but our Beam Splitter operator swapped the probabilities of the 2 states.

e) Their operator does not represent a way of understanding a beam-splitter. It does not accurately describe phenomenon at hand. 

<hr>

### Question 2

a) *How many basis kets are needed to describe an arbitrary 3-qubit output state?*

The result of the circuit can be represented by 1 bit since it's outputs are the set:
$$\{\ket{000}, \ket{111}\}$$
Taking $\log_2$ of the cardinality of the set, we get that the number of bits to represent the output spaces is $1$.

b) *Write the initialized quantum state using bra-ket notation.*
$$\ket{\psi_0} = \ket{000}$$

c) *Write the quantum state for the qubits after each step in the computation.*
$$\begin{align}
\ket{\psi_1} &= \dfrac{1}{\sqrt{2}}\ket{000}+\dfrac{1}{\sqrt{2}}\ket{100}\\
\ket{\psi_2} &= \dfrac{1}{\sqrt{2}}\ket{000}+\dfrac{1}{\sqrt{2}}\ket{110}\\
\ket{\psi_3} &= \dfrac{1}{\sqrt{2}}\ket{000}+\dfrac{1}{\sqrt{2}}\ket{111}
\end{align}$$
d) *What is the probability of measuring all 3 qubits to be in the zero state after the computation is complete?*
$$p\left(\ket{\psi_3} = \ket{000}\right) = \left(\dfrac{1}{\sqrt{2}}\right)^2 = \dfrac{1}{2}$$
e)  *Is the output state entangled? Why or why not*? 
The output state is very much entangled, since the resultant cannot be factored into non-correlated states (dependent).

<hr>

### Question 3

a)  *Quantum computers are faster than classical computers because they test all solutions to a problem at the same time in parallel universes*. 

Same answer as part B, but I have something to mention: It's not necessarily parallel universes. There are many interpretations to quantum mechanics, and so this answer would depend on your belief of a certain interpretation.


b) *Quantum computers are faster than classical computers because they can test all classical solutions to a problem at the same time (in parallel).*

Depending on the algorithm at hand, this can be a very significant tool, like in the Deutsch-Jozsa algorithm.
In general, Quantum computers aren't *necessarily* faster than classical computers, but there are certain exploits of superposition and entanglement that can have a significant speedup if done properly.


c. Quantum computers are faster than classical computers because they use quantum superposition to try all classical solutions at the same time (in parallel).

Same as Part B. They *can* be faster, but not always.


d. Quantum computers use quantum superposition and interference as a resource to help solve some problems faster than classical computers.

Definitely agreed. Quantum computers can leverage non-signaling correlations that do not exist in classical computing. Ideally, we could have non-signaling correlations that would always produce a right answer, but with quantum mechanics we can only get up to about 85% efficacy (over 75% with classical computers).

Source: *Gamification of bell's theorem* by Udiprod on YouTube.


e. Classical computers can solve any problem quantum computers can.

This depends on what you define "solve" to be. If it's solving at all, without worrying about practicality, the answer is yes. If you mean that all problems can be solved in a reasonable time, the answer is no.

Quantum computers can have algorithmic time complexities in sets lower than classical computers, however that is dependent on the algorithm. For Deutsch-Josza, the speedup is the different between O(2^n) for classical computers and O(log(N)) for quantum computers.


f. This is the first time you the student have heard of the TV show 60 Minutes.  

Same as part G.


g. This the first time you the student have watched any content from the TV show 60 Minutes.

I have heard of it once from one of my wellness classes talking about Maple Syrup storage in Canada and how there was a theft of a LOT of maple syrup in the past.