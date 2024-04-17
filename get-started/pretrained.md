---
icon: sliders
order: E
---

# Custom Pretraineds

- In the training tab, check the **'Custom Pretrained'** box, upload the files, and select it in the **Pretrained G/D Path boxes**.

![](/assets/load_pretrained.png)

## What are custom pretraineds?

Those are pretraineds trained by AI enthusiasts, unlike the original pretraineds, were created using long higher-quality datasets. Additionally, they yield better results in models.

### Ov2 Super by SimplCup

Works well for small and English datasets. Additionally, it allows models to train with very few epochs compared to regular pretrains. This only supports **32k and 40k** sample rates.

> https://huggingface.co/ORVC/Ov2Super/tree/main

### RIN E3 by Mustar

Yields good results with clean and English datasets, but it is more sensitive to noise. This only supports **40k** sample rate.

> https://huggingface.co/MUSTAR/RIN_E3/tree/main

### SnowieV3 by Mustar

Works well with Russian datasets and also helps models of other languages to pronounce Russian well. Supports **all the sample rates**.

- **32k**: [SnowieV3.1-32k](https://huggingface.co/MUSTAR/SnowieV3.1-32k/tree/main)
- **40k**: [SnowieV3.1-40k](https://huggingface.co/MUSTAR/SnowieV3.1-40k/tree/main)
- **48k**: [SnowieV3.1-48k](https://huggingface.co/MUSTAR/SnowieV3.1-48k/tree/main)

### SnowieV3 X RIN_E3 by Mustar

Works well with Russian or Japanese language datasets and also helps models of other languages to pronounce Russian or Japanese well. This only supports **40k** sample rate.

Make sure to select the sample rate according to the sample rate of the custom pretraineds.

> https://huggingface.co/MUSTAR/SnowieV3.1-X-RinE3-40K/tree/main
