---
slide: 06-algorithm 
---

<div style="text-align: left">
    <mark style="background-color: #ab2333!important"> 
        Diffusion Model Loss Function 
    </mark> 
</div>
---

<div style="text-align: left">
    DDPM Loss Function
</div>


$$
\mathcal{L}_{DM} := \mathbb{E}_{x,\epsilon \sim \mathcal{N}(0,1),t} \big[ ||\epsilon - \epsilon_{\theta}(x,t) ||^2_2 \big]
$$

<div style="text-align: left">
    Latent-space Diffusion Model (LDM) Loss Function
</div>

$$
\mathcal{L}_{LDM} := \mathbb{E}_{\varepsilon(x), \epsilon \sim \mathcal{N}(0,1),t} \big[ ||\epsilon - \epsilon_{\theta}(z_t,t) ||^2_2 \big]
$$