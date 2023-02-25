---
slide: 05-conceptual-framework 
---

<div style="text-align: left">
    <mark style="background-color: #ab2333!important"> 
        Image-To-Image
    </mark> 
</div>


```python
def image_2_image(text_prompt:str, img:Image) -> Image:
    embedding = text_embedding(NMT(text_prompt))
    latents = latent_representation(embedding, encode_latent(image))
    return decode_latent(latents)
```