---
expanded: false
order: B
icon: no-entry
---

# Errors 

Common general errors in RVC/Applio if you want to check the errors depending on the installation method please check the specific [installation method page](../installation-method/installation-method.md).

==- **FFmpeg error/utf8 error**
Ensure paths are free of special characters.
==-
==- **Situation with Google Colab**
Unfortunately, Google Colab is currently unavailable as Google has taken measures to restrict access to Colab services, including Applio. Thanks to our team, we have been able to bring Applio back. [More information here](/get-started\Other-Alternatives.md).
==-
==- **Connection Error**
Ensure the console (black command line window) is open.
==-
==- **WebUI popup 'Expecting value: line 1 column 1 (char 0)**
Disable system LAN proxy/global proxy and refresh.
==-
==- **Cuda error/Cuda out of memory**
Adjust batch size for training; for inference, modify settings in config.py. Consider upgrading the GPU if needed.
==-
==- **File/memory error(when training)**
Reduce "Number of CPU threads" or pre-cut training set to shorter audio files.
==-
==- **Error about llvmlite.dll**
Install [vc_redist.x64.exe](https://aka.ms/vs/17/release/vc_redist.x64.exe) for Windows.
==-
==- **RuntimeError: The expanded size of the tensor...**
Delete smaller-sized wav files, then click "train the model" and "train the index."
==-
==- **RuntimeError: The size of tensor a must match...**
Avoid changing the sampling rate mid-training. If necessary, change the exp name and train from scratch or copy pitch and features folders to accelerate training.
==-