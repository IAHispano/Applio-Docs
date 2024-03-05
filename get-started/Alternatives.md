---
order: L
icon: cloud
---

# Other Alternatives
Thanks to our team, we were able to bring Applio to other places for your convenience

+++ Cloud
 !!!warning Warning
 It should be noted that Gradio is banned from Colab, so it is preferable to use a secondary or new account to avoid a possible ban.
 !!!
 1. Enter [Applio Colab](https://colab.research.google.com/github/iahispano/applio/blob/master/assets/Applio.ipynb) and just **run the 2 cells**. 
 ![](../assets/Colab.png)

 2. Then a **public link** will be given to us where we can enter the interface.

 ### Extra cell
 In this section, you will find the following options:

 - **Mount Drive:** Connects Colab to our Google Drive for performing backups.
 - **AutoBackup:** Saves our trained model to our drive. Drive needs to be mounted first.
 - **LoadBackup:** Used to load our model if we want to retrain it. Drive must be mounted.
 - **Download Custom Pretrains:** Allows direct downloading of custom pretrains to Applio.

 ![](../assets/ExtraColab.png)

 3. You can [train](/get-started\training.md/) models, do [inference](/get-started\inferencing.md/), or use [TTS](/get-started\tts.md/)

 4. Your trained model is located in the logs/model folder, and the .pth files are in the logs/zips folder. If you want to save your model folder in your Drive, you just need to run the Mount Drive and AutoBackup cell before Start Applio.

 -  (If you want to retrain place the name of your model and run the LoadBackup cell and enter a higher number of epochs.)
+++ Huggingface
 1. First you need to create a huggingface account.

 2. Then enter [Applio Hugginface Space](https://huggingface.co/spaces/IAHispano/Applio) and duplicate the space, that is all. If you don't want to use huggingface you can use  [Applo playground](https://applio.org/playground).
 
 ![](../assets/Duplicate.png)
 
 !!!warning Warning
 You can't train models here.
 !!!
+++
