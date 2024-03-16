---
order: C
expanded: true
icon: mirror
---

# KaraFan

Here you will learn how to Separate the Vocals and the Instrumental of songs with KaraFan.

+++ Local
## How To Install?

!!!warning Important!
Its is only for **NVDIA GPUs.**
!!!
1. On your PC where you wish to store the **KaraFan project** and Go inside it.
2. First, we have to download and install [Python](https://www.python.org/ftp/python/3.11.0/python-3.11.0-amd64.exe).

3. Donwload:
- [Install.exe](https://github.com/Captain-FLAM/KaraFan/wiki/Data/Install.exe) <-- The easiest way! **(auto-extract the BAT)**.
- [Intall.zip](https://github.com/Captain-FLAM/KaraFan/wiki/Data/Install.zip) <-- Bypass the Browser Security
- [Install.bat](https://github.com/Captain-FLAM/KaraFan/wiki/Data/Install.bat) <-- Click to show, save it and rename to **Install.bat**.

!!!primary 
If you have installed Python 3.11 before WITHOUT using this Install.bat, you must uninstall it before !
Even those installed with the Microsoft Store !
!!!
!!!secondary Important
On Windows 11, you must allow first the execution of the **BAT file**:

- Right-click on the file
- Choose « Properties »
- In the « General » tab, click on the « Unlock » button
- Click on the « OK » button
!!!
4. You must execute it with **Administrator Rights**.

5. Run **Setup.py** by double-clicking on it. 

6. Now, you can launch **KaraFan.pyw** by double-clicking on it.

## How To Update?
Simply **Run the Setup.py** file !

### STRUCTURE 📂
After installation, you'll find new folders at the root of the folder you have chosen with the following structure :

Folder                      | Function
---                         | ---
/ KaraFan                   | The main application
/ KaraFan_user              | Where config file & FFmpeg executable are saved
/ KaraF/ KaraFan_user       | Where all the models are stored
/ KaraFan_user / Multi_Song | If you want to test SDR with your own recipes
/ Music                     | Here you can put your audio files (or choose another one)
/ Results                   | Here you will find your extracted audio files (or another one)

## How To Use?
1. Place your audio in the **music folder** and copy the **path of your song** that you want to separate and the path of the **folder** where the separated song will be stored.

2. Now place the settings you want to apply, try the ones you want the most, but if you want to effectively separate the instrumental or sounds from the vocals, I recommend the following settings:

||| To effectively separate the instrumental from the vocals
![](/../assets\Musica.png)
||| In case you want to separate the voice from a YouTuber’s video or other typoe of video
![](/../assets/Youtuber.png)
|||

3. We click on **Start** and it will begin to separate the chosen song. At the end of the process, the message **Processing DONE** will appear at the end of the interface.

4. Now we go to the **Vocals** folder and we will find a folder with the name of our song or audio. There we will find a list of audios, we download the audio with the name **Vocal Final**, in case you want the instrumental one that says **Music Final**.

For more information, visit the [GitHub repository](https://github.com/Captain-FLAM/KaraFan).
+++ Google Colab
1. In our Google Drive, we created the folder **Music** where we will put our songs to separate, and **Vocals** where our already separated song will be stored

!!!warning Warning
The Colab only lasts 30 minutes in execution. Additionally, it is possible that Colab may disconnect after a few hours due to Google’s limitations.
!!!
2. First, we go to the [Google Colab](https://colab.research.google.com/github/Eddycrack864/KaraFan/blob/master/KaraFan_Improved_Version.ipynb).

3. Run the cell by clicking on the white :icon-play: button. So that the repository can start to be cloned.

4. Then we click on the next cell **This is it!** to load the KaraFan interface.

5. Now we have to copy **the path of your song** that you want to separate and the path of the **folder** where the separated song will be stored. 

6. Now place the settings you want to apply, try the ones you want the most, but if you want to effectively separate the instrumental or sounds from the vocals, I recommend the following settings:

||| To effectively separate the instrumental from the vocals
![](/../assets\Musica.png)
||| In case you want to separate the voice from a YouTuber’s video or other typoe of video
![](/../assets/Youtuber.png)
|||

7. We click on **Start** and it will begin to separate the chosen song. At the end of the process, the message **Processing DONE** will appear at the end of the interface.

!!!info Info
The first time you use it, it will start downloading the models you have selected in your drive in the **KaraFan_user** folder. If you keep this folder for the next time you want to use it, you will not need to download it again.
!!!

8. Now we go to the **Vocals** folder and we will find a folder with the name of our song or audio. There we will find a list of audios, we download the audio with the name **Vocal Final**, in case you want the instrumental one that says **Music Final**.

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
+++



