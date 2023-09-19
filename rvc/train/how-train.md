# Train a model

Actually training a model is a simple and easy to learn procedure

- *First  create a folder with the name of your choice inside Applio-RVC-Fork > datasets and upload the audio inside it.*

## steps to follow in the interface
- **Step 1 (process dataset)**

   Once in Applio, name the model, next click on refresh dataset list and select the previously created folder, click the 'process data' step until you receive the 'end prepocess' output message.

- **Step 2  (Extract feature of the extraction method)**

  Select the desired extraction method, click the 'extract features' step and wait for the 'all-feature-done' message.

- **Step 3 (Train model)**

  The values of the configurations are applied depending on your needs
  ![](https://github.com/Maville-07/Applio-Docs/blob/18ca7a11bb6ac0246175b4bfef09d5dca1bb388a/assets/train%20example.png)

  **Save frequency:** it is recommended to set a number from 10 to 50, this option will save the state of the model every time it completes a cycle of the selected value *(it is useful to go back to a previous point in case of overtraining).*


  **Training epochs:** it is not possible to estimate a value of epochs to train a model, as each dataset is extended differently regardless of whether they have the same audio duration, for this step it is recommended to set the value that seems right for your model and keep an eye on the state of it through the tensorboard (although models from 100 - 200 epochs start to listen decently).

  
  **Batch size:** This is the amount of audios that will be processed at the same time to form an epoch, a higher value is equivalent to a faster training time, but at a cost that consumes more graphic resources (VRAM), this value is set depending on the vram of your graphics card, for Example: if you have 8gb of vram a value between 6 - 8 is set *(although the cuda cores of your graphics card compensate in part the batch size, so you can try with a little higher values).*

***once everything is set up, click on the train model button and wait for an epoch to form in the applio console.***
 
  ## Final Step (Save model and generate index file)

  when the training of our model is finished, we proceed to generate the index file by clicking the 'Train Feature Index' button, if the step was done correctly it should look something like this.
  
  ![](https://github.com/Maville-07/Applio-Docs/blob/986c7874cfce53579ea72f3cc87d75378c66951d/assets/index.png)

  **once everything is done, select a save method and click on the button, the zip file with the model will be found inside the folder 'finished/backup' inside 'logs' in Applio-RVC-Fork.**
