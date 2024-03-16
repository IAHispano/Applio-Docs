---
order: L
icon: cloud
---

# Other Alternatives
Thanks to our team, we were able to bring Applio to other places for your convenience

+++ Google Colab
 !!!warning Warning
 It should be noted that Gradio is banned from Colab, so it is preferable to use a secondary or new account to avoid a possible ban. Additionally, it is possible that Colab may disconnect after a few hours due to Google’s limitations.
 !!!
 1. Enter [Applio Colab](https://colab.research.google.com/github/iahispano/applio/blob/master/assets/Applio.ipynb) and just **run the 2 cells**. 
 ![](../assets/Colab.png)

 2. Then a **public link** will be given to us where we can enter the interface.

 ### Extra cells
 In this section, you will find the following options:

 - **Mount Drive:** Connects Colab to our Google Drive for performing backups.
 - **AutoBackup:** Saves our trained model to our drive. Drive needs to be mounted first.
 - **Load a Backup:** Used to load our model if we want to retrain it. Drive must be mounted.
 - **Download Custom Pretrains:** Allows direct downloading of custom pretrains to Applio.

 ![](../assets/ExtraColab.png)

 3. You can [train](/get-started\training.md/) models while checking [Tensorboard](/get-started\tensorboard.md), do [inference](/get-started\inferencing.md/), or use [TTS](/get-started\tts.md/)

 !!!info In case you want to **train**, you should run the **Extra cells** before run **Start Applio** cell. Otherwise, simply run the **Install Applio** and **Start Applio** cells.
 !!!

 ### How to upload my dataset in Colab?
 To load your dataset in Colab, there are two ways to do it:

 - Place your audio in a folder on your Google Drive, run the **Mount Drive** cell in Colab and Click on :file_folder: in Colab. Then navigate to your dataset folder, copy the path, it should look like this `/content/drive/MyDrive/dataset folder` and paste it into the **dataset path**.

 - Upload your audio in .wav format using the **Dataset Maker** or click on :file_folder: and setup it manually to `program/assets/datasets` creating inside a folder for the program to read it.

 4. Your trained model is located in the logs/model folder, and the .pth files are in the logs/zips folder. If you want to save your model folder in your Drive, you just need to run the **Mount Drive** and **AutoBackup** cell before run **Start Applio** cell.

 -  (If you want to retrain place the name of your model in the **Load a Backup** cell and run it. Then, insert the name of your model and enter a higher number of epochs.)
+++ Huggingface
 1. First you need to create a huggingface account.

 2. Then enter [Applio Huggingface Space](https://huggingface.co/spaces/IAHispano/Applio) and duplicate the space, that is all. If you don't want to use huggingface you can use  [Applo playground](https://applio.org/playground).
 
 ![](../assets/Duplicate.png)
 
 !!!warning Warning
 You can't train models here.
 !!!
+++
