---
slide: 05-conceptual-framework 
---

<div style="text-align: left">
    <mark style="background-color: #ab2333!important"> 
        Image-To-Image
    </mark> 
</div>

```python
def text_to_image(text_prompt:str) -> Image: 
    embeddings = word_embeddings(text_prompt)
    latents = latent_representation(embeddings)
    return decode_latent(latents)
```
