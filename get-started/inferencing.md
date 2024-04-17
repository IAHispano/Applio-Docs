---
icon: unmute
expanded: true
order: B
---

# Infer & Download models

- Downloading a [voice model](../Voice-Models/Voice-Models.md) is as simple as going to the **Download** tab.

![**Manual loading alternative:** unzip the downloaded .zip file and **drag the two files into the Drop files box**. Now you can search for models from Applio by simply entering the character name to search in the **Search Model** section, then copy the model link or download it.](/assets/download_models.png)

!!!warning
Applio can only download models from Google Drive, Huggingface, [Applio Web](https://applio.org/models), Discord, Yandex, Pixeldrain and Mediafire. Downloading files from mega may fail!, this is due to malfunction of the dependency.
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
- **Recommendation:** having a **clean acapella** helps to get better results. but if the model downloaded in its name mentions the words rvmpe or crepe click on the **advanced options box**. Furthermore, this section has the following:

==- **Advanced Settings**
- **Export Format:** Select the format to export the audio.
- **Split Audio:** Basically cuts the audio into parts to make the inference by parts and then joins them together.
- **Autotune:** Apply a soft autotune to your inferences, recommended for singing conversions.
- **Clean Audio:** Clean your audio output using noise detection algorithms, recommended for speaking audios.
- **Clean Strenght:** The more you increase it the more it will clean up, but it will be more compressed.
- **Pitch:** Adjust the tone of the model, for male it is - and female it is +. For male to female is -12 and female to male is +12. 
- **Filter Radius:** Applies respiration filtering to the results, the value represents the filter radius and respiration reduction to avoid artifacts.
- **Search Feature Ratio:** It is the one in charge of controlling the index, the larger the ratio, the more single the dataset but it can result in artifacts, so it is better to leave it as it is by default.
- **Volume Envelope:** Substitute or blend with the volume envelope of the output.
- **Protec Voiceless Consonants:** Safeguard distinct consonants and breathing sounds to prevent electro-acoustic tearing and other artifacts.
- **Hop Length:** Denotes the duration it takes for the system to transition to a significant pitch change. Smaller hop lengths require more time for inference and training but tend to yield higher pitch accuracy.
- **Pitch extraction algorithm:** Select between [rvmpe, crepe or other](https://docs.applio.org/faq/rvc/#f0-extraction-methods)
==- 

!!!primary What should I do if my output audio sounds [robotic](https://docs.applio.org/faq/rvc/#artifacting)?
 - Look for better quality audio.
 - Your voice model needs more [training](/get-started\training.md) or is [overtraining](https://docs.applio.org/faq/rvc/#overtraining).
 - Remove the reverb, double vocals and noise from your acapella, check the [UVR 5 guide](/guides\Audio\UVR.md) or [MVSEP guide](/guides\Audio\MVSEP.md).
 - The dataset of your model contained noise, you need to [clean the dataset](/guides\Datasets\Create-Datasets.md).
 - Try advanced settings.
!!!