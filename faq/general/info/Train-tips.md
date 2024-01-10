# Test previous model and continue Training

### - How can I use the saved model in the middle of training?

select one of the .pth generated file in `Applio-RVC-Fork/Logs/Weights` (you need to have the index previously generated for best results) or Save via model extraction at the bottom of the ckpt processing tab.

### - How can I continue training with more data?

Add data to a new path, process dataset, extract features, copy G and D files from the previous experiment, and continue training.
!!!
when increasing the number of audio, it is recommended to retrain the model so as not to have a mixture of datasets. 
!!!
