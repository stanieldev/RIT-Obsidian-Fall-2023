$$\begin{align}
\dfrac{T}{T_0} = \left(\dfrac{R}{R_0}\right)^c &\implies T = T_0 \left(\dfrac{R}{R_0}\right)^c \\
&\implies \ln(T) = \ln(T_0) + c \ln\left(\dfrac{R}{R_0}\right)
\end{align}$$
$$\dfrac{\partial T}{\partial c} = \dfrac{\partial}{\partial c}\left(T_0 \left(\dfrac{R}{R_0}\right)^c\right) =  T_0 \left(\dfrac{R}{R_0}\right)^c \ln\left(\dfrac{R}{R_0}\right) = T \ln\left(\dfrac{R}{R_0}\right)$$
$$\dfrac{\partial T}{\partial R} = \dfrac{\partial}{\partial R}\left(T_0 \left(\dfrac{R}{R_0}\right)^c\right) = T_0 \left(\dfrac{R}{R_0}\right)^c \cdot cR^{-1} = TcR^{-1}$$
$$\begin{align}
\delta T &= \sqrt{T^2 \ln\left(\dfrac{R}{R_0}\right)^2 (\delta c)^2 + T^2\dfrac{c^2}{R^2} (\delta R)^2} \\
&= T\sqrt{\ln\left(\dfrac{R}{R_0}\right)^2 (\delta c)^2 + c^2 \left(\dfrac{\delta R}{R}\right)^2}
\end{align}$$
$$c \pm \delta c = 0.822787 \pm 0.000681 \approx 5/6 \pm 6.81 \cdot 10^{-4}$$
$$R = \dfrac{V}{I}, \delta R = R\sqrt{\left(\dfrac{\delta V}{V}\right)^2 + \left(\dfrac{\delta I}{I}\right)^2} $$



### Do when class starts
$$ \begin{align}
R_0 &\pm \delta R_0 = a + b\\
T_0 &\pm \delta T_0 \ = c + d
\end{align}$$
$$ \begin{align}
V_{\tilde{} \ 1/2} &\pm \delta V_{\tilde{} \ 1/2} = a + b\\
I_{\ \tilde{} \ 1/2} &\pm \delta I_{\ \tilde{} \ 1/2} = c + d\\
R &\pm \delta R \ \ \ \ \ = e + f \\
\end{align}$$
$$ T = T_0 \left(\dfrac{R}{R_0}\right)^c = K \cdot \left(\dfrac{\Omega}{\Omega}\right)^{\tfrac{5}{6}} = K $$
$$\delta T = \dfrac{T}{x} \sqrt{\left(x\ln x\right)^2 (6.81\cdot10^{-4})^2 + (\tfrac{5}{6})^2 \left(\delta x\right)^2} = K$$




### Week 1 Check-In
$$R = \dfrac{V}{I}, \ \ \ \delta R = R\sqrt{\left(\dfrac{\delta V}{V}\right)^2 + \left(\dfrac{\delta I}{I}\right)^2} $$
> Convert all the V's and I's into R's. They are no longer needed after that

$$T = T_0 \left(\dfrac{R}{R_0}\right)^c, \ \ \ \delta T = T\sqrt{\left(\ln \dfrac{R}{R_0}\right)^2 (\delta c)^2 + c^2 \left(\dfrac{\delta R}{R}\right)^2}$$

$$\ln(T) = \ln\left(\dfrac{T_0}{{R_0}^c}\right) + c \ln R $$
$$\delta (\ln T) = \sqrt{\left(\ln \dfrac{R}{R_0}\right)^2 (\delta c)^2 + c^2 \left(\dfrac{\delta R}{R}\right)^2}$$
$$\delta (\ln(x)) = \dfrac{\partial (\ln(x))}{\partial x} \delta x = \dfrac{\delta x}{x} $$

$$P = \overline{P}, \ \ \ \delta P = \dfrac{s_P}{\sqrt{N}}$$

$$\ln P = \ln\overline{P}, \ \ \ \delta(\ln P) = \dfrac{\delta P}{\overline{P}}$$


$$P = \left(\sigma A_s \dfrac{\Omega}{4\pi}\right)(T^4-T_0^4)$$
$$\left(\sigma A_s \dfrac{\Omega}{4\pi}\right)=s \implies \sigma = \dfrac{4 \pi}{A_s \Omega}s, \ \ \ \delta\sigma = \dfrac{4 \pi}{A_s \Omega}\delta s$$

$$\ln P \approx \ln \left(\sigma A_s \dfrac{\Omega}{4\pi}\right) + 4\ln(T)$$
$$\ln \left(\sigma A_s \dfrac{\Omega}{4\pi}\right) = b  \implies \sigma = \dfrac{4 \pi}{A_s \Omega}e^b, \ \ \ \delta\sigma = \dfrac{4 \pi}{A_s \Omega}e^b\delta s$$
