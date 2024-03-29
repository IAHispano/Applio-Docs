---
icon: unmute
expanded: true
order: B
---

# Infer & Download models

- Downloading a [voice model](/voice-models) is as simple as going to the **"download"** tab.

![**Manual loading alternative:** unzip the downloaded .zip file and **drag the two files into the corresponding box below.**](/assets/download_models.png)

!!!warning
Downloading files from mega may fail!, this is due to malfunction of the dependency.
!!!

---

# How to infer

- When we have the model ready we will go back to the [inference](https://docs.applio.org/faq/rvc/#inference) section.

+++ Single
1. **Upload your audio and select it**, make sure it is only vocals. 
2. Click the **Refresh** button at the top right and select the downloaded/uploaded files in the **Voice model** and [index](https://docs.applio.org/faq/rvc/#added-index) file box.
3. Press **Convert** and you will have your inference done!
+++ Batch
1. Place your audio files in a folder, copy and paste the path into the **Input Folder**, if you’d like, you can also specify the output path for the converted audios in the **Output Folder**.
2. Click the **Refresh** button at the top right and select the downloaded/uploaded files in the **Voice model** and [index](https://docs.applio.org/faq/rvc/#added-index) file box.
3. Press **Convert** and you will have your inference done!
+++ 

!!!primary Make sure the path and audio name don't contain spaces or special characters.
!!!
- **Recommendation:** having a **clean acapella** helps to get better results. but if the model downloaded in its name mentions the words rvmpe, crepe or mangio-crepe click on the **advanced options box**. Furthermore, this section has the following:

==- **Advanced Settings**
- **Split Audio:** Basically cuts the audio into parts to make the inference by parts and then joins them together.
- **Autotune:** Apply a soft autotune to your inferences, recommended for singing conversions.
- **Clean Audio:** Clean your audio output using noise detection algorithms, recommended for speaking audios.
- **Clean Strenght:** The more you increase it the more it will clean up, but it will be more compressed.
- **Pitch:** Adjust the tone of the model, for male it is - and female it is +. For male to female is -12 and female to male is +12. 
- **Filter Radius:** Applies respiration filtering to the results, the value represents the filter radius and respiration reduction to avoid artifacts.
- **Search Feature Ratio:** It is the one in charge of controlling the index, the larger the ratio, the more single the dataset but it can result in artifacts, so it is better to leave it as it is by default.
- **Volume Envelope:** Substitute or blend with the volume envelope of the output.
- **Protec Voiceless Consonants:** Safeguard distinct consonants and breathing sounds to prevent electro-acoustic tearing and other artifacts.
- **Hop Length:** Denotes the duration it takes for the system to transition to a significant pitch change. Smaller hop lengths require more time for inference but tend to yield higher pitch accuracy.
- **Pitch extraction algorithm:** Select between [rvmpe, crepe, mangio-crepe or other](https://docs.applio.org/faq/rvc/#pitch-extraction-differences)
==- 

!!!primary What should I do if my output audio sounds [robotic](https://docs.applio.org/faq/rvc/#artifacting)?
 - Look for better quality audio.
 - Your voice model needs more [training](/get-started\training.md) or is [overtraining](https://docs.applio.org/faq/rvc/#overtraining).
 - Remove the reverb, double vocals and noise from your acapella, check the [UVR 5 guide](/guides\Audio\UVR.md) or [MCSEP guide](/guides\Audio\MVSEP.md).
 - The dataset of your model contained noise, you need to [clean the dataset](/guides\Datasets\Create-Datasets.md).
 - Try advanced settings.
!!!