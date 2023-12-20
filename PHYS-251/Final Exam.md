<hr>

### Question 1
1. (15pts) **Consider two state vectors for a spin ½ qubit**
$$\begin{align}
\ket{\psi_1} &= \ket{+} + (3+i)\ket{-} \\
\ket{\psi_2} &= i\ket{+} + 2e^{i\pi}\ket{-} = i\ket{+} - 2\ket{-}
\end{align}$$
#### State 1
a. *Is it a valid quantum state? If not, find a valid quantum state that represents the same physical system.*
$$\begin{align}
\ket{\psi_1} &= \begin{bmatrix}1\\3+i\end{bmatrix}_Z, \ \ \ \bra{\psi_1} = \begin{bmatrix}1&3-i\end{bmatrix}_Z \\
\langle\psi_1|\psi_1\rangle &= \begin{bmatrix}1&3-i\end{bmatrix}\begin{bmatrix}1\\3+i\end{bmatrix} \\
&= 1 + (3+i)(3-i) = 1+9+1 = \boxed{11 \ne 1}
\end{align}$$
To normalize $\psi_1$, we would have to divide by $\sqrt{11}$.

b. *If an ensemble of particles are prepared in the given state and sent through a x-oriented Stern-Gerlach Analyzer, what is the probability a particle will be observed leaving the $X^+$ port of the analyzer. What about the $X^-$ port?*
$$\begin{align}
\ket{\psi_1} &= \dfrac{1}{\sqrt{11}}\begin{bmatrix}1\\3+i\end{bmatrix}_Z = \dfrac{1}{\sqrt{22}}\begin{bmatrix}1&1\\1&-1\end{bmatrix}^Z_X\begin{bmatrix}1\\3+i\end{bmatrix}_Z = \dfrac{1}{\sqrt{22}}\begin{bmatrix}4+i\\-2-i\end{bmatrix}_X \\
\langle X^+|\psi_1\rangle &= \dfrac{1}{\sqrt{22}}\begin{bmatrix}1&0\end{bmatrix}\begin{bmatrix}4+i\\-2-i\end{bmatrix} = \dfrac{4+i}{\sqrt{22}}\\
P(X^+|\psi_1) &= \left(\dfrac{4-i}{\sqrt{22}}\right)\left(\dfrac{4+i}{\sqrt{22}}\right) = \boxed{P(X^+|\psi_1) = \dfrac{17}{22}} \\
\langle X^-|\psi_1\rangle &= \dfrac{1}{\sqrt{22}}\begin{bmatrix}0&1\end{bmatrix}\begin{bmatrix}4+i\\-2-i\end{bmatrix} = -\dfrac{2+i}{\sqrt{22}}\\
P(X^-|\psi_1) &= \left(-\dfrac{2-i}{\sqrt{22}}\right)\left(-\dfrac{2+i}{\sqrt{22}}\right) = \boxed{P(X^-|\psi_1) = \dfrac{5}{22}} \\
\end{align}$$
.
#### State 2
a. *Is it a valid quantum state? If not, find a valid quantum state that represents the same physical system.*
$$\begin{align}
\ket{\psi_2} &= \begin{bmatrix}i\\-2\end{bmatrix}_Z, \ \ \ \bra{\psi_2} = \begin{bmatrix}-i&-2\end{bmatrix}_Z \\
\langle\psi_2|\psi_2\rangle &= \begin{bmatrix}-i&-2\end{bmatrix}\begin{bmatrix}i\\-2\end{bmatrix} \\
&= -i^2+4 = \boxed{5 \ne 1}
\end{align}$$
To normalize $\psi_2$, we would have to divide by $\sqrt{5}$.

b. *If an ensemble of particles are prepared in the given state and sent through a x-oriented Stern-Gerlach Analyzer, what is the probability a particle will be observed leaving the $X^+$ port of the analyzer. What about the $X^-$ port?*
$$\begin{align}
\ket{\psi_2} &= \dfrac{1}{\sqrt{5}}\begin{bmatrix}i\\-2\end{bmatrix}_Z = \dfrac{1}{\sqrt{10}}\begin{bmatrix}1&1\\1&-1\end{bmatrix}^Z_X\begin{bmatrix}i\\-2\end{bmatrix}_Z = \dfrac{1}{\sqrt{10}}\begin{bmatrix}i-2\\i+2\end{bmatrix}_X\\
\langle X^+|\psi_2\rangle &= \dfrac{1}{\sqrt{10}}\begin{bmatrix}1&0\end{bmatrix}\begin{bmatrix}i-2\\i+2\end{bmatrix}_X = \dfrac{i-2}{\sqrt{10}}\\
P(X^+|\psi_2) &= \left(\dfrac{-i-2}{\sqrt{10}}\right)\left(\dfrac{i-2}{\sqrt{10}}\right) = \boxed{P(X^+|\psi_2) = \dfrac{5}{10}} \\
\langle X^-|\psi_2\rangle &= \dfrac{1}{\sqrt{10}}\begin{bmatrix}0&1\end{bmatrix}\begin{bmatrix}i-2\\i+2\end{bmatrix}_X = \dfrac{i+2}{\sqrt{10}}\\
P(X^-|\psi_2) &= \left(\dfrac{-i+2}{\sqrt{10}}\right)\left(\dfrac{i+2}{\sqrt{10}}\right) = \boxed{P(X^-|\psi_2) = \dfrac{5}{10}} \\
\end{align}$$
<hr>

### Question 2
2. (15pts) **Single-photon Entanglement?**
*Consider sending light into a 50/50 beamsplitter. A complete set of basis kets is $\ket{N_0,N_1}$, where $N_0$ is the number of photons entering port 0 and $N_1$ is the number of photons entering port 1.*

a. *What is a complete set of basis kets for the situation where we send exactly one photon into the system? Write an expression for an arbitrary single photon state using the new notation.*
$$S_1 = \{\ket{01}, \ket{10}\} \ \ \ \ \ \ket{\psi} = \alpha\ket{10} + \beta\ket{01} = \alpha\ket{P_0} + \beta\ket{P_1}$$
Where $\alpha$ is for Port $0$ and $\beta$ is for Port $1$.


b. *In terms of these basis kets, what is the input state where we send one photon into port 0 of the beamsplitter and no photons into port 1?*
$$\ket{\psi} = \ket{10} \ \ \ ( \ \ket{N_0,N_1} \ )$$

c. *What is the quantum state of light leaving the beamsplitter using our new basis kets?*
If a photon comes in from $P_0$ and goes straight through, the light doesn't rotate at all.
If a photon comes in from $P_0$ and reflects off the mirror, the light rotates 90 degrees CCW.
If a photon comes in from $P_1$ and goes straight through, the light doesn't rotate at all.
If a photon comes in from $P_1$ and reflects off the mirror, the light rotates 90 degrees CW.
$$\begin{align}
\ket{P_0} = \ket{10} &\rightarrow \dfrac{1}{\sqrt{2}}\left(\ket{P_2} + i\ket{P_3}\right)\\
\ket{P_1} = \ket{01} &\rightarrow \dfrac{1}{\sqrt{2}}\left(i\ket{P_2} + \ket{P_3}\right)
\end{align}$$
$$\begin{align}
U_\mathrm{BS}\ket{\psi} &= U_\mathrm{BS}\left(\alpha\ket{10} + \beta\ket{01}\right)\\
&= \dfrac{\alpha}{\sqrt{2}}\left(\ket{P_2} + i\ket{P_3}\right) + \dfrac{\beta}{\sqrt{2}}\left(i\ket{P_2} + \ket{P_3}\right) \\
&= \left(\dfrac{\alpha}{\sqrt{2}}+i\dfrac{\beta}{\sqrt{2}}\right)\ket{P_2} + \left(i\dfrac{\alpha}{\sqrt{2}}+\dfrac{\beta}{\sqrt{2}}\right)\ket{P_3}\\
&= \dfrac{1}{2}\left(e^{i\theta}\ket{P_2}+e^{i\left(\tfrac{\pi}{2}-\theta\right)}\ket{P_3}\right), \ \ \ \ \ \theta=\tan^{-1}{\dfrac{\beta}{\alpha}}
\end{align}$$

d. *Why might this output state be described as a "single photon entangled with the vacuum?"*

For the state where $\ket{N_0,N_1}$.
If both N is 0, then there's no photons.
If both N is 1, then the 2 photons have an entanglement.
If one N is 1, then it's "entangled" with the vacuum more as an interesting quirk of naming. The vacuum cannot contribute, and so its entanglement would be equivalent to a singular photon entering. It can also be said that it's "entangled" with a ghost photon.

<hr>

### Question 3
3. (20pts) **Bell State Analyzer**
$$\begin{aligned}
\ket{\Phi^\pm} &= \dfrac{\ket{00}\pm\ket{11}}{\sqrt{2}}\\
\ket{\Psi^\pm} &= \dfrac{\ket{01}\pm\ket{10}}{\sqrt{2}}
\end{aligned}$$
a. Two qubits prepared in the state $\ket{\psi_\mathrm{in}} = \ket{00}$ are sent into the analyzer. What is the probability of getting the outcome associated with the $\ket{\Phi^-}$ Bell state?
$$\begin{aligned}
\bra{\Phi^-} &= \dfrac{\bra{00}-\bra{11}}{\sqrt{2}} \\
\langle\Phi^-|\psi\rangle &= \dfrac{\langle{00}|00\rangle-\langle{11}|00\rangle}{\sqrt{2}} = \dfrac{1}{\sqrt{2}} \\
P(\Phi^-|\psi) &= \left(\dfrac{1}{\sqrt{2}}\right)^2 = \boxed{P(\Phi^-|\psi) = \dfrac{1}{2}}
\end{aligned}$$

b. *Given a state $\ket{\psi} = \dfrac{\ket{00}+\ket{01}}{\sqrt{2}}$, is the state entangled?*
$$\ket{\psi} = \dfrac{\ket{00}+\ket{01}}{\sqrt{2}} = \ket{0}\dfrac{\ket{0}+\ket{1}}{\sqrt{2}}$$
Since the 2-bit state can be decomposed into 2 distinct bits, they are not entangled. Each bit is independent, meaning they cannot be entangled.

c. *What is the probability of getting each of four analyzer outcomes for the Bell state measurement?*
$$\begin{align}
\ket{\psi} &= \dfrac{\ket{00}+\ket{01}}{\sqrt{2}} \\
\dfrac{\ket{00}}{\sqrt{2}} &= \dfrac{\ket{\Phi^+} + \ket{\Phi^-}}{2} \\
\dfrac{\ket{01}}{\sqrt{2}} &= \dfrac{\ket{\Psi^+} + \ket{\Psi^-}}{2} \\
\ket{\psi} &= \dfrac{1}{\sqrt{4}}\left(\ket{\Phi^+} + \ket{\Phi^-}+\ket{\Psi^+} + \ket{\Psi^-}\right)
\end{align}$$
Each component has a magnitude of $\dfrac{1}{2}$, so each probability is $\dfrac{1}{4}$.
$$P(\Phi^+|\psi)=P(\Phi^-|\psi)=P(\Psi^+|\psi)=P(\Psi^-|\psi)= \boxed{\dfrac{1}{4}}$$

d. *Pick Bell states and send them through the circuit. Does the circuit give distinguishable measurement outcomes for your states?*
For the sake of ease, I did all 4 simultaneously.
$$\begin{align}
\ket{\psi_1} &= \psi^{q_0q_1}\ket{q_0}\ket{q_1} \\
\ket{\psi_{1.5}} &= \psi^{q_0q_1}\ket{q_0}\ket{q_0\oplus q_1} \\
\ket{\psi_{2}} &= \psi^{q_0q_1}\left(\dfrac{\ket{0}+(-1)^{q_0}\ket{1}}{\sqrt2}\right)\ket{q_0\oplus q_1}
\end{align}$$
Assuming that each state is equally likely (like from part c).
$$\begin{aligned}
\ket{\Phi^\pm} &= \dfrac{\ket{00}\pm\ket{11}}{\sqrt{2}} = \left(\dfrac{\ket{0}+\ket{1}}{2}\right)\ket{0}\pm\left(\dfrac{\ket{0}-\ket{1}}{2}\right)\ket{0}\\
&= \dfrac{1}{2}\left(\ket{00}+\ket{10}\pm\ket{00}\mp\ket{10}\right)\\
&\rightarrow \boxed{\ket{\Phi^+} = \ket{00}, \ket{\Phi^-} = \ket{10}} \\
\\
\ket{\Psi^\pm} &= \dfrac{\ket{01}\pm\ket{10}}{\sqrt{2}} = \left(\dfrac{\ket{0}+\ket{1}}{2}\right)\ket{1}\pm\left(\dfrac{\ket{0}-\ket{1}}{2}\right)\ket{1}\\
&= \dfrac{1}{2}\left(\ket{01}+\ket{11}\pm\ket{01}\mp\ket{11}\right)\\
&\rightarrow \boxed{\ket{\Psi^+} = \ket{01}, \ket{\Psi^-} = \ket{11}}
\end{aligned}$$
Each outcome wavefunction maps to a unique binary string output, and so it does give distinguishable measurement outcomes.

<hr>

### Question 4

a. *Quantum Entanglement lets you communicate faster than light.*
**False**, signaling machines cannot transmit information faster than light.
However, entanglement **does** allow for correlation faster than light, since you gain no information thereof.

b. *Quantum computers solve problems by trying all the possible solutions at the same time.*
**False**. There are algorithms that do utilize superposition for exponential speedup, however they aren't solving each solution every time, as it doesn't measure all solutions. In the end, a quantum computer can only give you 1 state per qubit. Interference is exploited to encourage wanted solutions measured.

c. *Nobody understands quantum physics.*
False, but sorta true? If we're talking about strictly our theory of quantum mechanics, then **False**, we do understand quantum physics. However, if talking about the universe as a whole, and how quantum mechanics in our universe is described, then it's a sorta True, since our model is very good but not perfect (not that it needs to be, mind you).

<hr>

### Part 2 : Mini Project (A)
 - Trapped Ions use Alkali Earth Metals or other atoms that, when 1st ionized, have a singular remaining electron in the orbital (Ytterbium for IonQ).
 - Low pressure and cold environments are used.


1. **How do trapped ion systems physically implement a qubit? Can they scale-up to many qubits?**
 - Trapped ion encode qubits in the ground states of their electron orbitals. The diagram in the seminar looks to be a S-orbital and P-orbital ground states.
 - Each ion has a linear spacing with its neighbor, and so the scale of qubits is directly proportional to the number of ion traps. They can be stored pretty close together as well, helping with scalability.

2. **How do trapped ions perform a single qubit logic gate? How do they perform a two-qubit logic gate?**
 - Microwaves of certain frequencies ($\mu$-waves). Lasers are generally the way to modify the logic gates.
 - Two-Bit systems are performed using lasers like before, but also their electromagnetic coupling in the system to influence each other.

3. **How do trapped ion systems measure, or “read-out,” their qubits?**
 - State-dependent fluorescence using lasers is how IonQ does it. Based on the current state of the system, the number of photons is either a certain value (in the presentation, 30) or 0 since one of the states doesn't resonate with the light they use for measurement.

4. **What is one advantage and one disadvantage trapped ions have versus other quantum platforms we have considered?**
 - The fidelity of each computation seems to be really high and it scales relatively well.
 - However, while the size of the ions are pretty small, the lasers needed to run the system are massive relatively-speaking.


5. **What are some companies that are trying to build quantum computers out of your platform? Describe one example product and/or service.**
 - Taking a look at Honeywell, they claim that Quantum computers can be used for:
	 - Pharmaceuticals (drug design and discovery)
	 - Chemicals (development of new chemicals)
	 - Finance (reduced risk?)
	 - Aerospace & Defense (materials and computer technology)
	 - And a few others I didn't mention.

Pharmaceuticals, Chemicals, and Aerospace & Defense all share a common thread, and it's material science.
Quantum computers will help with the design of materials in the future since there are active efforts on simulating quantum systems using quantum computers, and so should help speed up the process and development of newer materials.

This is related to an internship I applied for over the summer which is related to using Quantum Computers to simulate Quantum Systems in chemistry and physics. I hope that I get the position, since I am very excited to learn more about quantum computing in terms of physics experiments and informational design.