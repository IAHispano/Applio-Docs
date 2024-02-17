---
order: A
icon: device-desktop
---

# UVR Guide

How to Separate the Vocals and the Instrumental of songs with UVR locally

1. **Download** and **install** [Ultimate Vocal Remover](https://github.com/Anjok07/ultimatevocalremovergui/releases/tag/v5.6).

!!!info Info
In case you get a Windows message, just click on **More information** and then on **Run anyway**.
!!!

2. **Download** the video of the song you want to use as a basis for creating the dataset or the AI cover:

!!!secondary
**For Youtube** : copy the song link from the search bar and paste it onto [Cobalt](https://cobalt.tools/).
!!!

3. **Open** Ultimate Vocal Remover and download the models, with which you can separate the voices and the instrumental parts into separate audios. For that, you will have to click here :wrench: and we go to the **Download Center** section.

:::

- **MDX-NET models**
  - MDX23C-InstVoc HQ (the best to remove the instrumental and vocals)
  - UVR-MDX-NET Voc FT (to remove the instrumental and vocals)
- **VR Arch models**
  - UVR-DeEcho-DeReverb (to remove reverb from vocals)
  - UVR-BVE-4B_SN-44100-1 (to separate 2 or more voices singing at the same time)
  - 5_Hp-Karaoke-UVR (to remove choruses from vocals)
    :::

4. **Select** the video or song as input and **choose** the output folder for the instrumental or final vocals.

5. **Choose Process Method** select the type of models you need to use (MDX-Net or VR Arch) after that select the model and click **Start Processing**. 
