
## Prelab: Linear w/o Intercept
$$ s + \delta s = (0.513 \pm 0.024)\tfrac{cm}{g} $$
$$ k = \dfrac{g}{s} = \dfrac{980 \frac{cm}{s^2}}{0.513 \tfrac{cm}{g}} = 1.91\tfrac{N}{m}$$
$$ \delta k = \left|\dfrac{\partial k}{\partial s} \delta s\right| = \dfrac{g}{s^2}\delta s = \dfrac{980 \tfrac{cm}{s^2}}{(0.513\tfrac{cm}{g})^2} (0.024 \tfrac{cm}{g}) =  0.0893\tfrac{N}{m}$$
$$ k + \delta k = (1.91 \pm 0.09)\tfrac{N}{m}$$



## Prelab: Linear w/ Intercept
$$ s + \delta s = (0.408 \pm 0.009)\tfrac{cm}{g} $$
$$ y_0 + \delta y_0 = (4.58 \pm 0.345)cm $$
$$ k = \dfrac{g}{s} = \dfrac{980 \frac{cm}{s^2}}{0.408 \tfrac{cm}{g}} = 2.40\tfrac{N}{m}$$
$$ \delta k = \left|\dfrac{\partial k}{\partial s} \delta s\right| = \dfrac{g}{s^2}\delta s = \dfrac{980 \tfrac{cm}{s^2}}{(0.408\tfrac{cm}{g})^2} (0.009 \tfrac{cm}{g}) =  0.0530\tfrac{N}{m} $$
$$ k + \delta k = (2.40 \pm 0.06)\tfrac{N}{m}$$
$$ m_{eff}=\frac{k}{g}y_0 = \frac{0.0240\tfrac{N}{cm}}{9.8 \frac{m}{s^2}}(4.58 cm) = 0.0112kg = 11.2g$$
$$ \delta m_{eff} = \left|\dfrac{\partial m_{eff}}{\partial k} \delta k\right| = \dfrac{y_0}{g}\delta k = \dfrac{4.58cm}{9.8\tfrac{m}{s^2}}(0.0530\tfrac{N}{m}) = 0.248g$$
$$ m_{eff} + \delta m_{eff} = (11.2 \pm 0.3)\tfrac{N}{m}$$
$$ m_{eff} = \dfrac{y_0}{s} \implies \delta m_{eff}^2 = \left(\dfrac{\partial m_{eff}}{\partial y_0} \delta y_0\right)^2 + \left(\dfrac{\partial m_{eff}}{\partial s} \delta s\right)^2
$$
$$\delta m_{eff}^2 = \left(\dfrac{1}{s} \delta y_0\right)^2 + \left(-\dfrac{y_0}{s^2} \delta s\right)^2 \implies \delta m_{eff} = 0.881g $$
$$ m_{eff} + \delta m_{eff} = (11.2 \pm 0.9)g$$




## Main Lab
$$ \dfrac{d^2 \theta}{dt^2} - \dfrac{g}{L} \theta = 0 \implies \omega^2 = \dfrac{g}{L} \implies T = 2\pi \sqrt{\dfrac{L}{g}}$$
$$ \delta(T^2) = \left|\dfrac{\partial (T^2)}{\partial T} \delta T\right| = 2T\delta T $$
$$ \delta((5T)^2) = \left|\dfrac{\partial ((5T)^2)}{\partial (5T)} \delta (5T)\right| = 10T \dfrac{1}{5}\delta T = 2T\delta T$$
$$ s + \delta s = (0.955 \pm 0.018)\tfrac{s^2}{cm} $$
$$ T_0 + \delta T_0 = (-0.253 \pm 0.453)s^2 $$
$$ g = \dfrac{100\pi^2}{s} = \dfrac{100\pi^2}{0.955 \tfrac{s^2}{cm}} = 1030 \tfrac{cm}{s^2} = 10.3 \tfrac{m}{s^2}$$$$ \delta g = \left|\dfrac{\partial g}{\partial s} \delta s\right| = \dfrac{100 \pi^2}{s^2}\delta s = \dfrac{100\pi^2 }{(0.955\tfrac{s^2}{cm})^2} (0.018\tfrac{s^2}{cm}) =  0.195\tfrac{m}{s^2} $$$$ g + \delta g = (10.3 \pm 0.2)\tfrac{m}{s^2}$$


$$ \delta T = 5 \cdot \delta(5T) = 5\cdot \dfrac{s_{5T}}{\sqrt{5}} = \sqrt{5} \cdot 0.127 = 0.284 s$$


$$ \lim_{L \rightarrow 0} T(L) = \lim_{L \rightarrow 0} 2\pi \sqrt{\dfrac{L}{g}} = 0$$