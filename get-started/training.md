---
icon: zap
expanded: false
order: C
---


# Training

!!!warning Important!
Training is only for **NVDIA GPUs.**
!!!
- [Don't know how to create a dataset?, check the create dataset section](/Datasets\Create-Datasets.md)

||| Step 1: Dataset Preparation
1. Prepare a folder to place your audio, it can have any name you like and place it in your favorite place
2. Copy the path of the folder containing your dataset and paste it in the **'dataset path'** box
|||


---
||| Step 2: Dataset Processing
1. Once the model is named and the dataset path is pasted press "Prepocess Dataset".
|||

!!!
**Recommendation:** select one of the 3 available frequencies according to the audio frequency of your dataset `(38k, 40k, 48k)` this will help to avoid filtering out more artifacts or background noise.
!!!

--- 
||| Step 3: Feature Extraction
1. Select an F0 method that suits your needs.
2. **(optional)** modify Hop lenght, lower value, higher smoothness of pitch change but slower training and vice versa.
|||

---
||| Step 4: Model Training
Configure the training parameters according to your needs.

 ![](/assets/training_example.png)
|||
---
- **Save Every Epoch:** Set this value between 10 and 50 to determine how often the model's state is saved during training.

- **Total Epochs:** The number of epochs needed varies based on your dataset. Monitor progress using TensorBoard; typically, models perform well around 200-400 epochs.

-  **Batch Size:** Adjust based on your GPU's VRAM. For 8 GB VRAM, use a batch size between 6 and 8. Consider CUDA cores when experimenting with higher batch sizes.

### Other Options

- **Pitch Guidance:** Just like the name, gives variation of pitch.
- **Pretrained:** Uses the existing RVC pretrained.
- **Save Only Latest:** Save a single .pth file (final model)
- **Save Every Weights:** Saves a .pth file of the process when a cycle of **'Save Every Epoch'** is completed.
- **Custom Pretrained:** just like the name, uses the Custom Pretrained that are loaded in applio.
- **GPU Settings:** Select which of your GPUs you are going to use (only for users who have more than one GPU).

---
Once configured, press **_'Start training'_** to start the process, everything is registered in the **applio CMD.**

---
||| Final Step: Model Saving and Index File Generation
1. Once training is completed, generate the index file by clicking the "Train Feature Index" button.
|||

How to use the Tensorbard? Check out the [Tensorboard](./tensorboard.md) section.

!!!secondary Retrainig
In case you want to retrain your model, just put the name of your model and the same settings from step 4, please note that you will have to specify the number of epochs you want your model to reach and start training.
!!!

!!!info Info
Your trained model will be found in a folder with your model name inside the logs folder and the pth files that are saved during the training in the folder named zips.
!!!
