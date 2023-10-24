### Velocity Equations
$$v = \dfrac{1}{M} \dfrac{\Delta y}{\Delta t}, \ \ \ \delta v = v \sqrt{\left(\dfrac{\delta M}{M}\right)^2 +\left(\dfrac{\delta (\Delta y)}{\Delta y}\right)^2+\left(\dfrac{\delta (\Delta t)}{\Delta t}\right)^2}$$
$$\begin{aligned}
&v_g = \dfrac{1}{M} \dfrac{\Delta y}{\Delta t_g} = \dfrac{1}{2.04} \dfrac{1\text{ mm}}{15.92\text{ s}} \\
&\boxed{v_g = 3.079\cdot10^{-5}\text{ m/s}}
\end{aligned}$$
$$\begin{aligned}
&v_V = \dfrac{1}{M} \dfrac{\Delta y}{\Delta t_V} = \dfrac{1}{2.04} \dfrac{1\text{ mm}}{6.82\text{ s}} \\
&\boxed{v_V = 7.188\cdot10^{-5}\text{ m/s}}
\end{aligned}$$
$$\begin{aligned}
&\delta v_g = v_g \sqrt{\left(\dfrac{\delta M}{M}\right)^2 +\left(\dfrac{\delta (\Delta y)}{\Delta y}\right)^2+\left(\dfrac{\delta (\Delta t_g)}{\Delta t_g}\right)^2} \\
& \ \ \ \ \ = (3.079\cdot10^{-5}\text{ m/s}) \sqrt{\left(\dfrac{0.05}{2.04}\right)^2 +\left(\dfrac{\delta (\Delta y)}{1\text{ mm}}\right)^2+\left(\dfrac{\delta (\Delta t_g)}{15.92\text{ s}}\right)^2} \\
& \ \ \ \ \ = (3.079\cdot10^{-5}\text{ m/s})(2.451\cdot10^{-2}) \\
&\boxed{\delta v_g = 0.076\cdot10^{-5}\text{ m/s}}
\end{aligned}$$
$$\begin{aligned}
&\delta v_V = v_V \sqrt{\left(\dfrac{\delta M}{M}\right)^2 +\left(\dfrac{\delta (\Delta y)}{\Delta y}\right)^2+\left(\dfrac{\delta (\Delta t_V)}{\Delta t_V}\right)^2} \\
& \ \ \ \ \ = (7.188\cdot10^{-5}\text{ m/s}) \sqrt{\left(\dfrac{0.05}{2.04}\right)^2 +\left(\dfrac{\delta (\Delta y)}{1\text{ mm}}\right)^2+\left(\dfrac{\delta (\Delta t_V)}{6.82\text{ s}}\right)^2} \\
& \ \ \ \ \ = (7.188\cdot10^{-5}\text{ m/s})(2.451\cdot10^{-2}) \\
&\boxed{\delta v_V = 0.177\cdot10^{-5}\text{ m/s}}
\end{aligned}$$
$$\begin{aligned}
&\text{Final Velocity Results}\\
&\boxed{v_g \pm \delta v_g = \left(3.079\cdot10^{-5} \pm 0.076\cdot10^{-5}\right)\text{ m/s}}
\\
&\boxed{v_V \pm \delta v_V = \left(7.188\cdot10^{-5} \pm 0.177\cdot10^{-5}\right)\text{ m/s}}
\end{aligned}$$

### Radius Equations
$$\begin{aligned}
&\text{Let } K = \dfrac{9\eta}{2(\rho_\text{oil}-\rho_\text{air})g} = 9.745\cdot10^{-9} \text{ m}\cdot\text{s} \\
&r = \sqrt{Kv_g} \iff r^2 = K v_g  \\
&\delta r = \dfrac{K}{2r}\delta v_g \iff 2r\delta r = K\delta v_g 
\end{aligned}$$
$$\begin{aligned}
&r = \sqrt{Kv_g} = \sqrt{(9.745\cdot10^{-9} \text{ m}\cdot\text{s})(3.079\cdot10^{-5}\text{ m/s})} \\
&\boxed{r = 5.478\cdot10^{-7}\text{ m}}
\end{aligned}$$
$$\begin{aligned}
&\delta r = \dfrac{K}{2r}\delta v_g = \dfrac{9.745\cdot10^{-9} \text{ m}\cdot\text{s}}{2(5.478\cdot10^{-7}\text{ m})}\cdot 0.076\cdot10^{-5}\text{ m/s}\\
&\boxed{\delta r = 0.068\cdot10^{-7}\text{ m}}
\end{aligned}$$
$$\begin{aligned}
&\text{Final Radius Results}\\
&\boxed{r \pm \delta r= \left(5.478\cdot10^{-7} \pm 0.068\cdot10^{-7}\right)\text{ m}} \\
\end{aligned}$$

### Charge Equations
$$q = 6\pi\eta d\dfrac{(v_g + v_V)r}{V}, \ \delta q = q \sqrt{\left(\dfrac{\delta d}{d}\right)^2+\left(\dfrac{\delta v_g+\delta v_V}{v_g+v_V}\right)^2+\left(\dfrac{\delta r}{r}\right)^2+\left(\dfrac{\delta V}{V}\right)^2}$$
$$\begin{aligned}
&q = 6\pi\eta d \cdot\dfrac{(v_g + v_V)r}{V} \\
& \ \ = 6\pi(1.85\cdot10^{-5}\text{ Pa}\cdot\text{s})(5.91\text{ mm}) \cdot\dfrac{(10.267\cdot10^{-5}\text{ m/s})(5.478\cdot10^{-7}\text{ m})}{500\text{ V}}\\
&\boxed{q = 2.318\cdot10^{-19}\text{ C}}
\end{aligned}$$
$$\begin{aligned}
&\delta q = q \sqrt{\left(\dfrac{\delta d}{d}\right)^2+\left(\dfrac{\delta v_g+\delta v_V}{v_g+v_V}\right)^2+\left(\dfrac{\delta r}{r}\right)^2+\left(\dfrac{\delta V}{V}\right)^2} \\
& \ \ \ \ = (2.318\cdot10^{-19}\text{ C}) \sqrt{8.329\cdot10^{-4}+\left(\dfrac{\delta V}{500\text{ V}}\right)^2} \\
&\boxed{\delta q = 0.067\cdot10^{-19}\text{ C}}
\end{aligned}$$
$$\begin{aligned}
&\text{Final Charge Results}\\
&\boxed{q \pm \delta q= \left(2.318\cdot10^{-19} \pm 0.067\cdot10^{-19}\right)\text{ C}} \\
\end{aligned}$$

### Corrected Charge Equations
$$q_c = q\cdot\left(1+\dfrac{A}{r}\right)^{-\tfrac{3}{2}}, \ \ \ \delta q_c = q_c \sqrt{\left(\dfrac{\delta q}{q}\right)^2 + \left(\dfrac{3}{2}\dfrac{A}{A+r}\right)^2\left( \dfrac{\delta r}{r}\right)^2}$$
$$\begin{aligned}
&q_c = q\cdot\left(1+\dfrac{A}{r}\right)^{-\tfrac{3}{2}} = (2.318\cdot10^{-19} \text{ C})\cdot\left(1+\dfrac{7.776\cdot10^{-8}\text{ m}}{5.478\cdot10^{-7} \text{ m}}\right)^{-\tfrac{3}{2}}\\
&\boxed{q_c = 1.900\cdot10^{-19}\text{ C}}
\end{aligned}$$
$$\begin{aligned}
&\delta q_c = q_c \sqrt{\left(\dfrac{\delta q}{q}\right)^2 + \left(\dfrac{3}{2}\dfrac{A}{A+r}\right)^2\left( \dfrac{\delta r}{r}\right)^2} \\
& \ \ \ \ \ = (1.890\cdot10^{-19}\text{ C}) \sqrt{\left(\dfrac{0.067}{2.318}\right)^2 + \left(\dfrac{0.233}{1.251}\right)^2\left( \dfrac{6.8\text{ nm}}{547.8\text{ nm}}\right)^2}\\
&\boxed{\delta q_c = 0.055\cdot10^{-19}\text{ C}}
\end{aligned}$$
$$\begin{aligned}
&\text{Final Corrected Charge Results}\\
&\boxed{q_c \pm \delta q_c= \left(1.900\cdot10^{-19} \pm 0.055\cdot10^{-19}\right)\text{ C}} \\
\end{aligned}$$


### Elementary Charge (n\*e)
$$n = \dfrac{q_c}{e}, \ \ \ \delta n = n \left(\dfrac{\delta q_c}{q_c}\right)$$
$$\begin{aligned}
&n = \dfrac{q_c}{e} = \dfrac{1.900\cdot10^{-19}\text{ C}}{1.602176634\cdot10^{-19}\text{ C}}\\
&\boxed{n = 1.186}
\end{aligned}$$
$$\begin{aligned}
&\delta n = n \left(\dfrac{\delta q_c}{q_c}\right) = (1.186) \left(\dfrac{0.055\cdot10^{-19}\text{ C}}{1.900\cdot10^{-19}\text{ C}}\right)\\
&\boxed{\delta n = 0.035}
\end{aligned}$$
$$\begin{aligned}
&\text{Final Charge Results}\\
&\boxed{n \pm \delta n = \left(1.186\pm 0.035\right)\text{ e}^-} \\
\end{aligned}$$

