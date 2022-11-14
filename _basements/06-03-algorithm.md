---
slide: 06-algorithm 
---

<div style="text-align: left">
    <mark style="background-color: #ab2333!important"> 
        Transformers: Multi-Head Attention Layers 
    </mark> 
</div>
---

**Multi-Head Attention Algorithm**
$$
\begin{aligned}
						d_k = d_v = \frac{D}{h} \ | D &= d_{\text{model}}  \\
						W^O &\in \mathbb{R}^{D \times D} \\
						W^Q &\in \mathbb{R}^{D \times d_k} \\
						W^K &\in \mathbb{R}^{D \times d_k} \\
						W^V &\in \mathbb{R}^{D \times d_v} \\ \\
\text{MultiHead(Q,K,V)} &= \text{Concat}(h_i,...,h_h)W^O \\
						h &= \text{Attention}(QW_i^Q,KW_i^K,VW_i^V) \\
\end{aligned}
$$