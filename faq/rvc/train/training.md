---
expanded: false
order: A
---


# How to train

!!!warning Important!
Training is only for NVDIA GPUs.
!!!

### Step 1: Dataset Preparation
1. Create a folder with the desired name inside `Applio-RVC-Fork/datasets/`.
2. Download the audio files intended for training into this folder.

### Step 2: Dataset Processing
1. Open Applio and navigate to the "Train" tab.
2. Give your model a name.
3. Click on "Update list" in the interface.
4. Select the folder created in Step 1.
5. Click on the "Process Data" button and wait for the "End Preprocess" message.

### Step 3: Feature Extraction
1. Choose the desired f0 that suits your needs.
2. Click on the "Extract Features" button.
3. Wait for the "All-Feature-Done" message to confirm the completion of feature extraction.

### Step 4: Model Training
1. Configure the training parameters according to your needs.
    - Save Frequency: Set this value between 10 and 50 to determine how often the model's state is saved during training.
    - Training Epochs: The number of epochs needed varies based on your dataset. Monitor progress using TensorBoard; typically, models perform well around 200-400 epochs.
    - Batch Size: Adjust based on your GPU's VRAM. For 8 GB VRAM, use a batch size between 6 and 8. Consider CUDA cores when experimenting with higher batch sizes.
2. Click the "Train Model" button to initiate training.
3. Monitor progress in the Applio console with each epoch.

### Final Step: Model Saving and Index File Generation
1. Once training is completed, generate the index file by clicking the "Train Feature Index" button.
2. If you followed the steps correctly, it should resemble the provided example.
3. To save your model, select a preferred saving method and click the corresponding button. The .zip file containing your model will be located inside `Applio-RVC-Fork/logs/finished/` folder.

How to use the tensorboatd? Check out the [Tensorboard](./tensorboard.md) section.