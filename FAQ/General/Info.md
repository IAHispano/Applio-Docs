---
order: B
icon: search
expanded: false
---


# Info 

Common questions and information about RVC/Applio in general

==- **How to train and infer without the WebUI?**
Link: [Training and Inference without WebUI](https://huggingface.co/lj1995/VoiceConversionWebUI/blob/main/myinfer-v2-0528.py)
==-
==- **How to share a model/How to use others models?**
Share the pth file in the weights folder, not the one in logs. Future versions will use a zip file. Do not copy large pth files; use the ckpt tab to extract a smaller model for sharing. Compress it into a zip and upload it to Drive or Huggingface if you want to publish your model in Ai Hispano, go to the :envelope_with_arrow:`publish-a-model` section and execute the /model command and fill in the corresponding data of your model
==-
==- **Test previous model and continue Training**
### - How can I use the saved model in the middle of training?

select one of the .pth generated file in `Applio/Logs/zips` (you need to have the index previously generated for best results) or Save via model extraction at the bottom of the ckpt processing tab.

### - How can I continue training with more data?

Add data to a new path, process dataset, extract features, copy G and D files from the previous experiment, and continue training.
!!!
when increasing the number of audio, it is recommended to retrain the model so as not to have a mixture of datasets. 
!!!
==-
