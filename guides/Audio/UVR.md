---
order: A
icon: device-desktop
---

# UVR

Here you will learn how to Separate the Vocals and the Instrumental of songs with UVR.

+++ Local
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
  - UVR-MDX-NET Crowd HQ 1 (to remove crowd from vocals)
- **VR Arch models**
  - UVR-DeEcho-DeReverb (to remove reverb from vocals)
  - UVR-BVE-4B_SN-44100-1 (to separate 2 or more voices singing at the same time)
  - 5_Hp-Karaoke-UVR (to remove choruses from vocals)
  - UVR-DeNoise (to remove noise from vocals)
:::

4. **Select** the audio or song as input and **choose** the output folder for the instrumental or final vocals.
!!!info 
You can change the **type of wav or the MP3 bitrate** in **Additional settings**, in **Audio Format Settings**.
!!!
5. Choose **Process Method** select the type of models you need to use (MDX-Net or VR Arch) after that select the model and click **Start Processing**. 
!!!info Before Processing
- You can select if you only want the **Vocals Only**, **Instrumental Only**, the vocals with **No Reverb Only**, **No Crowd Only**, **No Noise Only** or with those effects.
!!!

6. Finally, look for your processed audio in the location you selected as output.
+++ Google Colab

1. First, we go to the [UVR Colab](https://colab.research.google.com/github/Eddycrack864/Ultimate-Vocal-Remover-5.6-for-Google-Colab/blob/main/Ultimate_Vocal_Remover_5_6_for_Google_Colab.ipynb)
!!!warning Warning
It should be noted that Gradio is banned from Colab, so it is preferable to use a secondary or new account to avoid a possible ban. Also, some models don't work. Additionally, it is possible that Colab may disconnect after a few hours due to Google’s limitations.
!!!
2. Run the 2 cells. You can check the **vip_models** option if you wish to use them.

3. Then a public link will be given to us where we can enter the interface.
!!!info 
You can change the **type of wav or the MP3 bitrate** in **Additional settings**, in **Settings**.
!!!

4. Drag or choose the audio or song to the **input audio** section and place the name it will have in **input filename**.

5. Choose **Process Method** select the type of models you need to use (MDX-Net or VR Arch) after that select the 
model and click **Start Processing**.

:::

- **MDX-NET models**
  - UVR-MDX-NET Inst HQ 4 (the best to remove the instrumental and vocals, but this may leave additional noise)
  - UVR-MDX-NET Voc FT (to remove the instrumental and vocals)
  - UVR-MDX-NET Crowd HQ 1 (to remove crowd from vocals)
- **VR Arch models**
  - UVR-DeEcho-DeReverb (to remove reverb from vocals)
  - 5_Hp-Karaoke-UVR (to remove choruses from vocals)
  - UVR-DeNoise (to remove noise from vocals)
:::

!!!info Before Processing
- You can select the **windows size** and the **aggression setting** in case of **VR Arc** and the **batch size** and the **volume compensation** for **MDX-NET**. 
- You should check the **GPU conversion** option. Additionally, 
- You can select if you only want the **Vocals Only**, **Instrumental Only**, the vocals with **No Reverb Only**, **No Crowd Only**, **No Noise Only** or with those effects.
!!!
6. Finally, download the processed audio.
+++
