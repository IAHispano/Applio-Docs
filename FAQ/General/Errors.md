---
expanded: false
order: B
icon: no-entry
---

# Errors 

Common general errors in RVC/Applio.

==- **Dependencies**
In the conda installation method, Applio is installed in a conda environment. This enviroment has all the dependencies needed to run RVC/Applio so you don't need to install anything else.
==-
==- **Error Downloading Miniconda**
If there are issues automatically downloading Miniconda, download it [manually](https://repo.anaconda.com/miniconda/Miniconda3-py39_23.9.0-0-Windows-x86_64.exe) and install it.
==-
==- **Conda Error Building Wheels**
If Conda shows an error related to the "Wheels" dependency, check that Visual Studio Build Tools are installed. This requirement it should be installed semi automatically by the installer.
==-
==- **Tensorboard or dependency error**
If an error related to Tensorboard occurs, it's likely that no dependencies were installed correctly. [Review if you have the latest installer version](/get-started\Installation.md).

Also, please check if you have done any of the following:

||| Did you install applio in a directory with spaces or non ASCII characters in the path?
If you did, please reinstall applio in a directory without spaces or non ASCII characters in the path. (For example your C: drive root)
|||

||| Did you have the antivirus/firewall enabled during the installation?
If you did, please reinstall applio with the antivirus disabled.
|||

||| Did you open the run-applio.bat file with administrator privileges?
If you did, please open it without administrator privileges.
|||
==-
==- **Situation with Google Colab**
Unfortunately, Google Colab is currently unavailable as Google has taken measures to restrict access to Colab services, including Applio. Thanks to our team, we have been able to bring Applio back. [More information here](/get-started\Alternatives.md).
==-
==- **FFmpeg error/utf8 error**
Ensure paths are free of special characters.
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
==- **The filename, directory name, or volume label syntax is incorrect**
Make sure to correctly set the path for your dataset before training. Remember that the dataset should not be in a zip file within the Applio/assets/datasets folder.
==-
==- **IndexError: list index out of range**
Make sure to use the same sample rate when retraining or when selecting a custom pretrain.
==-
==- **Alternative**
If all else fails, download the precompiled (Zip or Exe) version. This will bring everything ready to start applio without the need to perform the installation.
==-