---
icon: zap
expanded: false
order: C
---


# Training

!!!warning Important!
Training is only for **NVDIA GPUs**, If you don’t have a compatible GPU, the Training tab will be disabled.
!!!

- [If you don’t have an NVIDIA GPU, you can try Applio Colab or Applio No UI Colab. Check the other alternatives section.](/get-started/Alternatives.md)

||| Step 1: Dataset Preparation
1. Upload your audio in .wav format using the **Dataset Maker (if it is a single audio)** or setup it manually (various audios) to `applio/assets/datasets` creating inside a folder for the program to read it.
|||
- [don't know how to create a dataset?, check the dataset section](/guides/Datasets/Create-Datasets.md)

---
||| Step 2: Dataset Processing
1. Once the model is named and the dataset selected press **"Prepocess Dataset"** and wait for the message in the CMD.
|||
!!!info Make sure your dataset consists of single audio file or if you split it, ensure that each audio segment has a duration of 10 to 15 seconds per audio.
!!!

- you can select one of the **3 available frequencies** according to the audio `(32k, 40k, 48k)`, this will help to avoid filtering out more artifacts or background noise.

- [don't know how to check sample rate?, check the sample rate section](/guides/Datasets/Sample-Rate.md)

--- 
||| Step 3: Feature Extraction
1. Select an [F0 method](https://docs.applio.org/faq/rvc/#f0-extraction-methods) that suits your needs.
2. **(optional)** modify [Hop lenght](https://docs.applio.org/get-started/inferencing/#advanced-settings), lower value, higher smoothness of pitch change but slower training and vice versa.
3. **(optional)** select the Embedder model (hubert or contentvec)
|||

---
||| Step 4: Model Training
Configure the training parameters according to your needs.

 ![](/assets/Training-Example.png)
|||
---
- **Save Every Epoch:** Set this value between 10 and 50 to determine how often the model's state is saved during training.

- **Total Epochs:** The number of epochs needed varies based on your dataset. Monitor progress using TensorBoard; typically, models perform well around 200-400 epochs.

-  **Batch Size:** Adjust based on your GPU's VRAM. For 8 GB VRAM, use a batch size between 6 and 8. Consider CUDA cores when experimenting with higher batch sizes.

### Other Options

- **Pitch Guidance:** Gives variation of pitch.
- [Pretrained:](https://docs.applio.org/faq/rvc/#pretrained) Uses the [RVC](https://docs.applio.org/faq/rvc/#what-is-rvc) pretrained.
- **Save Only Latest:** Save a single D/G file with information.
- **Save Every Weights:** Save the weights of the model when a cycle of 'Save Every Epoch' is completed.
- [Custom Pretrained:](/get-started/pretrained.md) Uses the Custom Pretrained that are loaded.
- **GPU Settings:** Allows to choose GPUs (only for users who have more than one GPU).
- **Overtraining Detector:** Mark it only if you will train for more than 200 epochs.
- **Overtraining Threshold:** Set the maximum number of epochs you want your model to stop training if no improvement is detected.
!!!info Mark the **Save Only Latest** option before training to prevent it from filling up your storage.
!!! 
---
Once configured, press **_'Start training'_** to start the process, everything is registered in the **CMD.**

- [don't know how to use Tensorboard for correct training? Check out the Tensorboard section](/get-started/tensorboard.md)
---
||| Final Step: Model Saving and Index File Generation
1. Once training is completed, generate the index file by clicking the "Train Feature Index" button.
2. Your trained model is located in the `logs/model folder`, and the [.pth](https://docs.applio.org/faq/rvc/#pth) files are in the `logs/zips` folder.
|||

!!!info
Now you can export your trained model directly from the Applio interface, go to the **Export Model** section in the **train** tab, click on the **Refresh** button and select the **pth and the [added index](https://docs.applio.org/faq/rvc/#added-index)** of the model to export.
!!!
---

||| Optional Step: Resume training
1. Open Applio if you have closed it.
2. Then, in the Applio interface, input your **model name**, use the same **sample rate**, and proceed to the last part of the train tab. Set the same **[batch size](https://docs.applio.org/faq/rvc/#batch-size)**, **[pretrained](https://docs.applio.org/get-started/pretrained/#how-to-use-pretraineds) (if you used)** and increase the number of epochs you want to train.
3. Once configured, press **_'Start training'_** to start the process, everything is registered in the **CMD.**
|||