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
- You can choose the **output format** format of your separate audio.
- You can select if you only want the **Vocals Only**, **Instrumental Only**, the vocals with **No Reverb Only**, **No Crowd Only**, **No Noise Only** or with those effects.
- If you wish, you can change the **Segment Size** and the **Overlap** in case of **MDX23C** and **MDX-NET**, the **windows size** and the **aggression setting** for **VR Arc** to your preference or leave it as it is.
!!!

6. Finally, look for your processed audio in the location you selected as output.
+++ Google Colab
1. First, we go to the [UVR Colab](https://colab.research.google.com/github/Eddycrack864/UVR5-NO-UI/blob/main/UVR5_NO_UI.ipynb).

2. In our Google Drive, we created the folder **Separar** where we will put our songs to separate, and **Vocales** where our already separated song will be stored.
!!!info
Now you can download the music that you want to separate from Colab, go to the **YouTube Audio Downloader for Separation** cell, just place the link of the song in **video_url** and song name in **audio_name**, then run that cell. Your song will be stored in the **Separar** folder that you created in your Drive.
!!!
3. Run the **Installation** cell to start cloning the repository to the colab and mount drive.

4. Run the cell of your choice: **BS Reformer, MDX23C, MDX-NET, VR ARCH, Demucs**.

:::

- **BS Reformer**
  - BS-Reformer-Viperx-1297 (the best to remove instrumental and vocals)
- **MDX23C**
  - MDX23C 8KFFT instVoc HQ2 (one of the best to remove the instrumental and vocals)
  - MDX23C 8KFFT InstVoc HQ (one of the best to remove vocals and instrumental)
- **MDX-NET models**
  - UVR-MDX-NET Voc FT (to remove the instrumental and vocals)
  - UVR-MDX-NET Crowd HQ 1 (to remove crowd from vocals)
- **VR Arch models**
  - UVR-DeEcho-DeReverb (to remove reverb from vocals)
  - 5_Hp-Karaoke-UVR (to remove choruses from vocals)
  - UVR-DeNoise (to remove noise from vocals)
- **Demucs**
  - htdemucs_ft (to remove instrumental, vocals, drums, bass and other)
  - htdemucs (to remove instrumental, vocals, drums, bass and other)

!!!info Before Processing
- You can choose the **output format** format of your separate audio.
- If you wish, you can change the **Segment Size** and the **Overlap** in case of **MDX23C** and **MDX-NET**, the **windows size** and the **aggression setting** for **VR Arc** to your preference or leave it as it is.
!!!

5. Now we go to the **Vocales folder**, there we find our separate audios, we download the audio with the name of the **song-Vocals**, in case you want the instrumental is **song-Instrumental**.
:::
+++ 
