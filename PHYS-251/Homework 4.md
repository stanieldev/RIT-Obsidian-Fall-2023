Stanley Goodwin, 11/10/2023
<hr>

### Question 1: Bell States
In class, we learned about the four Bell states:
$$\begin{aligned}
\ket{\Phi^\pm} &= \dfrac{\ket{H_1H_2}\pm\ket{V_1V_2}}{\sqrt{2}} \\
\ket{\Psi^\pm} &= \dfrac{\ket{H_1V_2}\pm\ket{V_1H_2}}{\sqrt{2}} 
\end{aligned}$$
a) *Evaluate the inner product of $\ket{\Phi^-}$ with each of the four Bell states.*
$$\begin{aligned}
\langle\Phi^+|\Phi^-\rangle &= \dfrac{\bra{H_1H_2}+\bra{V_1V_2}}{\sqrt{2}}\dfrac{\ket{H_1H_2}-\ket{V_1V_2}}{\sqrt{2}} \\
&= \dfrac{1}{2}\left(\langle H_1H_2|H_1H_2 \rangle-\langle H_1H_2|V_1V_2\rangle+\langle V_1V_2|H_1H_2\rangle-\langle V_1V_2|V_1V_2\rangle\right) \\
&= \dfrac{1}{2}(1-0+0-1) = \boxed{0}
\end{aligned}$$
$$\begin{aligned}
\langle\Phi^-|\Phi^-\rangle &= \dfrac{\bra{H_1H_2}-\bra{V_1V_2}}{\sqrt{2}}\dfrac{\ket{H_1H_2}-\ket{V_1V_2}}{\sqrt{2}} \\
&= \dfrac{1}{2}\left(\langle H_1H_2|H_1H_2 \rangle-\langle H_1H_2|V_1V_2\rangle-\langle V_1V_2|H_1H_2\rangle+\langle V_1V_2|V_1V_2\rangle\right) \\
&= \dfrac{1}{2}(1-0-0+1) = \boxed{1}
\end{aligned}$$
$$\begin{aligned}
\langle\Psi^+|\Phi^-\rangle &= \dfrac{\bra{H_1V_2}+\bra{V_1H_2}}{\sqrt{2}}\dfrac{\ket{H_1H_2}-\ket{V_1V_2}}{\sqrt{2}} \\
&= \dfrac{1}{2}\left(\langle H_1V_2|H_1H_2 \rangle-\langle H_1V_2|V_1V_2\rangle+\langle V_1H_2|H_1H_2\rangle-\langle V_1H_2|V_1V_2\rangle\right) \\
&= \dfrac{1}{2}\left(\dfrac{1}{2}-\dfrac{1}{2}+\dfrac{1}{2}-\dfrac{1}{2}\right) = \boxed{0}
\end{aligned}$$
$$\begin{aligned}
\langle\Psi^-|\Phi^-\rangle &= \dfrac{\bra{H_1V_2}-\bra{V_1H_2}}{\sqrt{2}}\dfrac{\ket{H_1H_2}-\ket{V_1V_2}}{\sqrt{2}} \\
&= \dfrac{1}{2}\left(\langle H_1V_2|H_1H_2 \rangle-\langle H_1V_2|V_1V_2\rangle-\langle V_1H_2|H_1H_2\rangle+\langle V_1H_2|V_1V_2\rangle\right) \\
&= \dfrac{1}{2}\left(\dfrac{1}{2}-\dfrac{1}{2}-\dfrac{1}{2}+\dfrac{1}{2}\right) = \boxed{0}
\end{aligned}$$
b) *Do the Bell states form a complete basis for representing any two-qubit state? Why or why not?*

Since each basis is a uniform choice of each permutation of 2 states between 2 particles, as well as the inner product of each basis being the Kronecker delta, then it follows that it is a complete basis for any two-qubit state.


Interim) *Let pairs of photons prepared in the $\ket{\Psi^-}$ state travel to two different people, Alice and Bob, who can independently measure the polarization of the photon they receive in the HV (like a Z analyzer) representation or the DA (like a X analyzer) representation. Recall that:*
$$\begin{aligned}
\ket{D} &= \dfrac{\ket{H}+\ket{V}}{\sqrt{2}} \\
\ket{A} &= \dfrac{\ket{H}-\ket{V}}{\sqrt{2}} 
\end{aligned}$$
c) *What is the probability Alice measures her photon to be horizontally polarized? What is the probability she measures her photon to be diagonally polarized?*

For horizontally polarized, we get 50%. There is no reason to believe that Alice is getting a photon preferentially, so her measuring the photon who is horizontally polarized is 50:50.
For diagonally polarized, again, no photon is preferential, and so the odds if 50:50.

d) *If Alice measures her photon in the DA basis and gets the D outcome, what is the probability Bob will also get the D outcome if he makes the same type of measurement?*
$$\ket{\Psi^-} = \dfrac{\ket{H_1V_2}-\ket{V_1H_2}}{\sqrt{2}} = \dfrac{\ket{AD}-\ket{DA}}{\sqrt{2}}$$
Since the only non-zero states are when she measures D when it is D, then the result 100% of the time is $\ket{A}$ at Bob's end. Therefore, the probability that Bob sees $\ket{D}$ is 0.


<hr>

### Question 2: Sacrifices we make for QKD
*Alice and Bob use a single-photon, polarization-based QKD system to securely share a random bit string (the key). Alice has a single photon source which can prepare a photon to be in either the |𝐻⟩, |𝑉⟩, |𝐷⟩, or |𝐴⟩ polarization states. For each photon, Alice chooses one of the four states and sends the photon to Bob through a fiber optic cable. Bob uses a half-waveplate and polarizing beam-splitter to choose to measure each arriving photon in the HV or DA basis and gets an outcome for each measurement*. 

a) *Draw a diagram/schematic of the setup described above.*






2b) 1/4^2, 1/4^10, 1/4^100, 1/4^1000.

2c) If there is sources of error in transport, so long as it's less than 25%, they will just have to sacrifice more bits to have the same level of confidence than the case where there is no error.

3a) We cannot clone using information that we didn't initially install into the qubit itself. No cloning just means no replicating without knowledge of replication.

3b) Since we must know the information ahead of time to create an identical qubit, and since we cannot communicate information faster than the speed of light, then we cannot send messages FTL solely because of that cloning condition.

3c) It can at most travel at the speed of causality, and so no backwards communication.


4a) Due to the nature of the crystal. It has to split the photon in half, and so even a singular photon going in must create 2 photons out.

4b) I don't get what you mean by "in terms of photons" energy is conserved because energy is conserved.

4c) By definition it "makes" a single photon by detecting the other one? What am I supposed to say here?

4d) It is probabilistic so I'd argue it's not an on-demand source. However, for how easy it is to fire it up and eventually get one, it is an on-demand source. Depends on your definition of "on demand."