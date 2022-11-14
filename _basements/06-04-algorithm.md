---
slide: 06-algorithm 
---

<div style="text-align: left">
    <mark style="background-color: #ab2333!important"> 
        Diffusion-based Generative Model
    </mark> 
</div>
---

$$
\begin{aligned}
	q(x_t | x_{t-1}) &= \mathcal{N_{\theta}}\left(x_t\right) \\ 
	q(x_{1:T}|x_0) &= \prod_{t=1}^T q(x_t | x_{t-1})
		
\end{aligned}
$$

___
The noise kernel $\mathcal{N}$ is usually a Gaussian noise as it has an additive property for samples 
$x_t$ drawn as $t\to ∞$ results to standard Gaussian distribution. 
