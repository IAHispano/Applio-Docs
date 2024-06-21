---
order: C
icon: typography
---

# TTS

- We need to go to the **TTS** section in Applio.

- Select our **model with its respective index**.

- Select the **model of TTS** depending on the language you want and enter the text or add a **txt file** in the box below to convert.

- Select the **TTS Speed** (increase or decrease TTS speed).

- Finally we click on **convert** and wait for the result
-![](/assets/TTS.png)-

==- **Advanced Settings**
- **Export Format:** Select the format to export the audio.
- **Split Audio:** Basically cuts the audio into parts to make the inference by parts and then joins them together.
- **Autotune:** Apply a soft autotune to your inferences, recommended for singing conversions.
- **Clean Audio:** Clean your audio output using noise detection algorithms, recommended for speaking audios.
- **Upscale Audio:** Upscale the audio to a higher quality, recommended for low-quality audios.
- **Clean Strenght:** The more you increase it the more it will clean up, but it will be more compressed.
- **Pitch:** Adjust the tone of the model, for male it is - and female it is +. For male to female is -12 and female to male is +12. 
- **Filter Radius:** Applies respiration filtering to the results, the value represents the filter radius and respiration reduction to avoid artifacts.
- **Search Feature Ratio:** It is the one in charge of controlling the index, the larger the ratio, the more single the dataset but it can result in artifacts, so it is better to leave it as it is by default.
- **Volume Envelope:** Substitute or blend with the volume envelope of the output.
- **Protec Voiceless Consonants:** Safeguard distinct consonants and breathing sounds to prevent electro-acoustic tearing and other artifacts.
- **Hop Length:** Denotes the duration it takes for the system to transition to a significant pitch change. Smaller hop lengths require more time for inference and training but tend to yield higher pitch accuracy.
- **Pitch extraction algorithm:** Select between [rvmpe, crepe or other](https://docs.applio.org/faq/rvc/#f0-extraction-methods)
- **(optional) Embedder Model:** select the Embedder model (contentvec, japanese-hubert-base, chinese-hubert-large or custom).
==- 

- Applio also features ElevenLabs TTS. Check the [Plugins section](/get-started/plugins.md) for more information.