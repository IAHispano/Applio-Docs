---
expanded: false
icon: rocket
order: C
---

# RVC

Questions about RVC.

==- What is RVC?
RVC (Retrieval-Based Voice Conversion) is a technology that is used to clone the voice of a person/character or replace that voice with another one.
==- 
==- What are the requirements for RVC/Applio?
The minimum required for local training is an Nvidia RTX series 20 graphics card with 8GB of VRAM to train models, in the case of inference you only need to have a decent CPU and at least 4GB of VRAM. If you have a Celeron processor, it would be better to look at [other alternatives](/get-started\Alternatives.md).
==- 
==-  Can I use RVC/Applio on a Mac?
Yes, but only for inference. besides, the installation should be done as if it were on Linux.
==- 
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
==- Pitch extraction differences
- **pm:** It provides a quick but inefficient result and is less faithful to the voice model.

- **Harvest:** It offers a better replication of tones from our Acapella but is slower and often gives errors initially.

- **Dio:** Possibly used for moments when our Acapella has rapid word pronunciation, such as in rap.

- **Crepe:** It provides better word pronunciation results.

- **Crepe-tiny:** Similar to crepe, it processes faster but with less aggressiveness.

- **Mangio-crepe:** It provides better results in terms of breaths and performs the same as crepe, but it is slower and sometimes yields poorer results.

- **Mangio-crepe-tiny:** Similar to mangio-crepe, it's faster but with less aggressiveness.

- **Rmvpe:** It is a combination of pm and crepe but is fast for both training and inference. It is the most faithful to the voice model (currently the best option).

- **Fcpe:** It takes less context from the audios because it is faster, it is less sensitive but it can also lose information.
==-
==- Hybrids pitch extraction 
It makes the inference by comparing both models and takes the best of both with an approximate pitch. The following combinations exist:
- hybrid [rmvpe - fcpe]
- hybrid [crepe - rmvpe]
- hybrid [crepe - fcpe]
- hybrid [crepe - rmvpe - fcpe]
==-
==- Batch Size
The batch size is the amount of GPU that will be used to train the model. The larger the batch size, the shorter the training duration. It is recommended to use multiples of 4 as the batch size, although the most common is 8, as it gives the AI time to learn correctly without rushing.
==-
==- Inference
is the process where an audio is transformed by the voice model.
==- 
==- Artifacting
Is when the inference output sounds robotic, distorted, with background noise and with fails when trying to modulate words.
==- 
==- Pretrained
It is a model trained with several sets of long-duration audios that will serve as a basis for training the models in RVC.
==-
==- Overtraining
It’s when the TensorBoard graph starts to rise and never comes back down. An overtrained model will sound robotic, muffled, and won’t be able to articulate words well. For more information check the [Tensorboard section](/get-started\tensorboard.md).
==- 
==- G and D
They are responsible for storing the training data of the model.
Generative learns to replicate results similar to the original.
Discriminator tries to distinguish real data from those created by the generator.
==- 