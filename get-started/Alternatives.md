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

 !!!info Info
 You should select the Drive icon, which generates a code that allows you to mount your Drive in Colab. Keep in mind that this will clone the entire repository to your drive.
 !!!
 ![](../assets/Drive.png)

 3. You can [train](/get-started\training.md/) models, do [inference](/get-started\inferencing.md/), or use [TTS](/get-started\tts.md/)

 4. Your trained model is located in the logs/model folder, and the .pth files are in the logs/zips folder. If you want to save your model folder, you just need to move that folder or only the [D and G](https://docs.applio.org/faq/rvc/#g-and-d) pth file and your model’s .pth file to your drive.

 -  (If you want to retrain move that folder or D and G pth to Colab again, enter the same name of the model and locate in which stage the save files are left and enter a higher number of epochs.)
+++ Hugginface
 1. First you need to create a hugginface account.

 2. Then enter [Applio Hugginface Space](https://huggingface.co/spaces/IAHispano/Applio) and duplicate the space, that is all. If you don't want to use huggingface you can use  [Applo playground](https://applio.org/playground).
 
 ![](../assets/Duplicate.png)
 
 !!!warning Warning
 You can't train models here.
 !!!
+++
