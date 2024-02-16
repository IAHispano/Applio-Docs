---
icon: unmute
expanded: true
order: B
---

# Infer & Download models

- Downloading a model is as simple as going to the **"download"** tab.

![**Manual loading alternative:** unzip the downloaded .zip file and **drag the two files into the corresponding box below.**](/assets/download_models.png)

!!!warning
Downloading files from mega may fail!, this is due to malfunction of the dependency.
!!!

---

# How to infer

- When we have the model ready we will go back to the **'inference'** section.

1. **Upload your audio and select it**, make sure it is only vocals
2. Click the **'refresh'** button at the top right and select the downloaded/uploaded files in the **_Voice model_** and **_index file_** box.
3. Press **convert** and you will have your inference done!

- **Recommendation:** having a **'clean acapella'** helps to get better results. but if the model downloaded in its name mentions the words **rvmpe, crepe or mangio-crepe** click on the **advanced options box** and select the right method, this will help to have more acurrate pitch control.

!!!primary What should I do if my output audio sounds robotic?
 - Look for better quality audio
 - Your voice model needs more [training](/get-started\training.md) or is [overtraining](/get-started\tensorboard.md).
 - Remove the reverb, double vocals and noise from your acapella, check the [UVR 5 guide](/Audio\UVR.md) or [MCSEP guide](/Audio\MVSEP.md).
 - The dataset of your model contained noise, you need to [clean the dataset](/Datasets\Create-Datasets.md).
!!!