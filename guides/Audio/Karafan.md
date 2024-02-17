---
order: C
expanded: true
icon: cloud
---

# KaraFan Guide 

How to Separate the Vocals and the Instrumental of songs with KaraFan (Colab Version)

1. In our Google Drive, we created the folder **Music** where we will put our songs to separate, and **Vocals** where our already separated song will be stored

!!!warning Warning
It should be clarified that there is a small chance that your Google account may be banned, therefore it is preferable to use a secondary or new account. In addition, the Colab only lasts 30 minutes in execution.
!!!

2. First, run the cell by clicking on the white :icon-play: button. So that the repository can start to be cloned.

3. Then we click on the next cell **This is it!** to load the KaraFan interface.

4. Now we have to copy **the path of your song** that you want to separate and the path of the **folder** where the separated song will be stored. 

5. Now place the settings you want to apply, try the ones you want the most, but if you want to effectively separate the instrumental or sounds from the vocals, I recommend the following settings:

||| To effectively separate the instrumental from the vocals
![](/../assets\Musica.png)
||| In case you want to separate the voice from a YouTuber’s video or other typoe of video
![](/../assets/Youtuber.png)
|||

6. We click on **Start** and it will begin to separate the chosen song. At the end of the process, the message **Processing DONE** will appear at the end of the interface.

!!!info Info
The first time you use it, it will start downloading the models you have selected in your drive in the **KaraFan_user** folder. If you keep this folder for the next time you want to use it, you will not need to download it again.
!!!

7. Now we go to the **Vocals** folder and we will find a folder with the name of our song or audio. There we will find a list of audios, we download the audio with the name **Vocal Final**, in case you want the instrumental one that says **Music Final**.

### Code to be afk

To run this code in Colab, we have to press the keys **Ctrl + Shift + i** to open the **developer tools** option and the following window will open. In case another window is displayed, we can locate it by selecting the **Console** option, so in this way Colab will not disconnect during the separation process. First, we put **Allow pasting**, then we press enter and only then it will let us enter the code.

``` js
function ClickConnect() {
var iconElement = document.getElementById("toggle-header-button");
if (iconElement) {
var clickEvent = new MouseEvent ("click", {
bubbles: true, cancelable: true,
view: window
});
iconElement.dispatchEvent (clickEvent);
}
}
setInterval(ClickConnect, 6000);
```



