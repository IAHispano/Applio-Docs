---
expanded: false
icon: rocket
order: C
---

# RVC

Questions about RVC.

==- Dataset
A Dataset is a set of audio files compressed into a .zip file used by RVC for voice training.
==-
==- Is a Dataset the same as a Model?
No, a Dataset is the set of audio used for training, while a Model is the result of that training.
==-
==- Added index
The added index contains the compressed dataset and is responsible for controlling the tones of the model at the time of inference.
==-
==- Pth
It is the one that contains all the data from the trained model that will serve us to make inference.
==-
==- Epoch
An Epoch is the number of iterations performed during training to complete one full cycle of your dataset. For example, if you have a dataset of 200 audio samples and you set a batch_size of 10, 10 audio samples will be processed in each iteration. To process all 200 audio samples, you will need to perform 20 iterations in total. This complete cycle is referred to as one epoch.
==-
==- Hop Length 
Hop Length is used for tonal fluctuations. Lower values are more precise but slower, while higher values are quicker but less accurate.
==-
==- Pitch extraction differences
- **pm:** It provides a quick but inefficient result and is less faithful to the voice model.

- **Harvest:** It offers a better replication of tones from our Acapella but is slower and often gives errors initially.

- **Dio:** Possibly used for moments when our Acapella has rapid word pronunciation, such as in rap.

- **Crepe:** It provides better word pronunciation results.

- **Crepe-tiny:** Similar to crepe, it processes faster but with less aggressiveness.

- **Mangio-crepe:** It provides better results in terms of breaths and performs the same as crepe, but it is slower and sometimes yields poorer results.

- **Mangio-crepe-tiny:** Similar to mangio-crepe, it's faster but with less aggressiveness.

- **Rmvpe:** It is a combination of pm and crepe but is fast for both training and inference. It is the most faithful to the voice model (currently the best option).
==-
==- Batch Size
The batch size is the amount of GPU that will be used to train the model. The larger the batch size, the shorter the training duration. It is recommended to use multiples of 4 as the batch size, although the most common is 8, as it gives the AI time to learn correctly without rushing.
==-
==- Search Feature Ratio
It is the one in charge of controlling the index, the larger the ratio, the more single the dataset but it can result in artifacts, so it is better to leave it as it is by default.
==-
==- Pitch
The pitch is used to adjust the tone of the model so that it can match the original voice and avoid artifacts, for men it is - and women it is +.
==-
==- Split Audio
Basically cuts the audio into parts to make the inference by parts and then joins them together.
==-
==- Pretrained
It is a model trained with several sets of long-duration audios that will serve as a basis for training the models in RVC.
==-
==- Overtraining
It’s when the TensorBoard graph starts to rise and never comes back down. An overtrained model will sound robotic, muffled, and won’t be able to articulate words well. For more information check the [Tensorboard section](/get-started\tensorboard.md).
==- 
