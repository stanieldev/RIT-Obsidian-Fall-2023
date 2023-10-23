Tensor: Collection of Vectors and Covectors combined with the Tensor Product



### Vectors and Covectors
$$\epsilon^i e_j = \delta_j^i$$
A vector is a rank $(1,0)$ tensor (contravariant)
A covector is a rank $(0,1)$ tensor (covariant).



## Tensor Objects

### Vector | Rank (1,0) Tensor
$$v \in V, \ \ \ v = v^i e_i$$
### Covector | Rank (0,1) Tensor
$$\alpha: V \rightarrow \mathbb{R}, \ \ \ \alpha \in V^*, \ \ \ \alpha = \alpha_i \epsilon^i$$
### Linear Map | Rank (1,1) Tensor
$$L: V \rightarrow V, \ \ \ L \in V \otimes V^*, \ \ \ L = L^j_i e_j \epsilon^i$$
### Bilinear Forms | Rank (0,2) Tensor
$$B: V \times V \rightarrow \mathbb{R}, \ \ \ B \in V^* \otimes V^*, \ \ \ B = B_{ij} \epsilon^i \epsilon^j$$
### Metric Tensor | Rank (0,2) Tensor   (SPECIAL)
$$\begin{align}
&g: V \times V \rightarrow \mathbb{R}, \ \ \ g \in V^* \otimes V^*, \ \ \ g = g_{ij} \epsilon^i \epsilon^j \\
& g_{ij} = g_{ji}, \ \ \ g\vec{v}\vec{v} = g_{ij}v^iv^j= ||\vec{v}||^2 \ge 0
\end{align}$$
### General Tensors | Rank (n,m) Tensor
$$T \in V^{\otimes n} \otimes (V^*)^{\otimes m}, \ \ \ T = T^{\overbrace{abc\dots}^\text{n times}}_{\underbrace{ijk\dots}_\text{m times}} \underbrace{e_ae_be_c\dots}_{\text{n vectors}} \  \underbrace{\epsilon^i\epsilon^j\epsilon^k\dots}_{\text{m covectors}}$$
