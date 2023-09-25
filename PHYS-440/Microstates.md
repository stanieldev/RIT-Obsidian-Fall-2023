Why are irreversible macroscopic states are overwhelmingly probable?
 - Microstates described by specific configurations of the system with definite values of physical properties (position, momentum, energy of individual particles) of constituents.

### Multiplicity
$$\Omega = \dfrac{N!}{n_1!n_2!n_3!...} = \dfrac{N!}{\prod_i n_i!}$$
### Entropy
$$S \equiv k_b \log \Omega$$
$$\Omega = \Omega_A \Omega_B \implies S = S_A + S_B$$
### Sterling Approximation
$$N! = N^N e^{-N} \sqrt{2\pi N}$$


### Problem Example
A binary state of $10^{23}$ elementary dipoles with a system net energy of 0.

$$\begin{align} W = \dfrac{N!}{\left({\tfrac{N}{2}}\right)!\left({\tfrac{N}{2}}\right)!} &\approx \dfrac{N^N e^{-N} \sqrt{2\pi N}}{\left((\tfrac{N}{2})^\tfrac{N}{2} e^{-\tfrac{N}{2}} \sqrt{2\pi \tfrac{N}{2}}\right)\left((\tfrac{N}{2})^\tfrac{N}{2} e^{-\tfrac{N}{2}} \sqrt{2\pi \tfrac{N}{2}}\right)} \\ &= \dfrac{N^N e^{-N} \sqrt{2\pi N}} {N^N e^{-N} \cdot \pi 2^{-N} N} = \sqrt{\dfrac{2}{N\pi}} \cdot 2^N\end{align}$$
Compared to all unique states $2^N$, the ratio of available microstates is $2.523\cdot10^{-12}$.
Another way is to say that Available : Unique States is $1$ : $\approx 4\cdot 10^{11}$.
