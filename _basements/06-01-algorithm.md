---
slide: 06-algorithm 
---

<div style="text-align: left">
    <mark style="background-color: #ab2333!important"> 
        Backpropagation
    </mark> 
</div>
---

1. Initialize weights from a random source $w \sim \mathcal{X}$
2. Compute the loss in $\mathcal{L}(\vec{w}^{(l)}, \vec{y})$. 
3. For each layer:
	1. Compute gradient with respect to previous layer $\nabla_{a^l}\mathcal{L}(\vec{w}^{(l)}, \vec{y})$. 
	2. Find the most sensitive node with respect to the input.
	3. Re-initialize initial weights $w_1$ parameter
4. Repeat until $\min \mathcal{L}(\vec{w}, \vec{y})$.