---
icon: zap
expanded: false
order: C
---


# Training

!!!warning Important!
Training is only for **NVDIA GPUs**, If you don’t have a compatible GPU, the Training tab will be disabled.
!!!

How to use the Tensorboard for correct training? Check out the [Tensorboard](./tensorboard.md) section.
||| Step 1: Dataset Preparation
1. upload your audio in .wav format using the **Dataset Maker** or setup it manually to `applio/assets/datasets` creating inside a folder for the program to read it.
|||
- [don't know how to create a dataset?, check the dataset section](/guides\Datasets\Create-Datasets.md)

---
||| Step 2: Dataset Processing
1. Once the model is named and the dataset selected press **"Prepocess Dataset"** and wait for the message in the CMD.
|||
!!!info Make sure your dataset consists of single audio file or if you split it, ensure that each audio segment has a duration of 10 to 15 seconds per audio.
!!!

- you can select one of the **3 available frequencies** according to the audio `(38k, 40k, 48k)`, this will help to avoid filtering out more artifacts or background noise.

- [don't know how to check sample rate?, check the sample rate section](/guides\Datasets\Sample-Rate.md)

--- 
||| Step 3: Feature Extraction
1. Select an [F0 method](https://docs.applio.org/faq/rvc/#pitch-extraction-differences) that suits your needs.
2. **(optional)** modify [Hop lenght](https://docs.applio.org/get-started/inferencing/#advanced-settings), lower value, higher smoothness of pitch change but slower training and vice versa.
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

- **Pitch Guidance:** Gives variation of pitch.
- [Pretrained:](https://docs.applio.org/faq/rvc/#pretrained) Uses the [RVC](https://docs.applio.org/faq/rvc/#what-is-rvc) pretrained.
- **Save Only Lates:** Save a single file with information.
- **Save Every Weights:** Saves a D/G file of the process when a cycle of **'Save Every Epoch'** is completed.
- [Custom Pretrained:](/get-started\pretrained.md) Uses the Custom Pretrained that are loaded.
- **GPU Settings:** Allows to choose GPUs (only for users who have more than one GPU).

---
Once configured, press **_'Start training'_** to start the process, everything is registered in the **CMD.**
- [don’t forget to check TensorBoard while training your model., check the tensorboard section](/get-started\tensorboard.md)
---
||| Final Step: Model Saving and Index File Generation
1. Once training is completed, generate the index file by clicking the "Train Feature Index" button.
|||


- (If you want to retrain, enter the same name of the model and locate in which stage the save files are left, enter a higher number of [epoch](https://docs.applio.org/faq/rvc/#epoch).)

- Your trained model is located in the logs/model folder, and the [.pth](https://docs.applio.org/faq/rvc/#pth) files are in the logs/zips folder.

- [If you don’t have an NVIDIA GPU, you can try Applio Colab. Check the other alternatives section.](/get-started\Alternatives.md)
