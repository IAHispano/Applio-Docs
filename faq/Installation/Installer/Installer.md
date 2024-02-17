---
expanded: false
icon: desktop-download
order: B
---

# Installer

Here you have all the frequent asked questions about the installer option.
==- Dependencies
In the conda installation method, Applio is installed in a conda environment. This enviroment has all the dependencies needed to run RVC/Applio so you don't need to install anything else.
==-
==- Tensorboard or dependency error
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
==- Error Downloading Miniconda
If there are issues automatically downloading Miniconda, download it [manually](https://repo.anaconda.com/miniconda/Miniconda3-py39_23.9.0-0-Windows-x86_64.exe) and install it.
==-
==- Conda Error Building Wheels
If Conda shows an error related to the "Wheels" dependency, check that Visual Studio Build Tools are installed. This requirement it should be installed semi automatically by the installer.
==-
==- Alternative
If all else fails, download the precompiled version. This will bring everything ready to start applio without the need to perform the installation.
==-