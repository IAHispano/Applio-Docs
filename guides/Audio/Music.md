---
order: D
expanded: true
icon: cloud
---

# Music Source Separation
Here you will learn how to Separate the Vocals and the Instrumental of songs with Music Source Separation Colab.

1. First, we go to the [Google Colab](https://colab.research.google.com/github/Eddycrack864/Music-Source-Separation-Universal-Colab/blob/main/Music_Source_Separation_Universal_Colab.ipynb).

2. In our Google Drive, we created the folder **Separar** where we will put our songs to separate, and **Vocales** where our already separated song will be stored.

!!!primary Notes
- It only works with audio in **.wav format**.
- Mel-Band RoFormer currently broken.
- Swin Upernet currently broken.
!!!

3. Run the **Setup** cell to start cloning the repository to the colab.

4. Select the model to use, and run the **Separation cell**.

:::
- MDX23C 8KFFT instVoc HQ2 (the best to remove the instrumental and vocals)
- MDX23C 8KFFT InstVoc HQ (vocals, instrumental)
- BanditPlus (SFX, speech, music, effects)
:::

5. Now we go to the **Vocals folder**, there we find our separate audios, we download the audio with the name of the **song-Vocals**, in case you want the instrumental is **song-Instrumental**.
