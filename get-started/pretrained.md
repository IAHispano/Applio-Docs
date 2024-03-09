---
icon: sliders
order: E
---
# Custom Pretraineds

- In the training tab check the **'Custom Pretrained' box**, upload the files and select it in the **Pretrained G/D Path boxes**.

 ![](/assets/load_pretrained.png)

## What are custom pretraineds?
Those are pretraineds trained by AI enthusiasts, unlike the original pretraineds, were created using long higher-quality datasets. Additionally, they yield better results in models.

### Download [Ov2Super](https://huggingface.co/ORVC/Ov2Super/tree/main) by SimPLClup
### Download [RIN_E3](https://huggingface.co/MUSTAR/RIN_E3/tree/main) by mustar22

!!!info Things you should know:
- **Ov2Super** works well for small datasets. Additionally, it allows models to train with very few epochs compared to regular pretrains. This only supports 32k and 40k sample rates 
- **RIN_E3** yields good results with clean datasets, but it is more sensitive to noise, this only support 40k 
sample rate.
- Make sure to select the sample rate according to the sample rate of the custom pretraineds.
!!!