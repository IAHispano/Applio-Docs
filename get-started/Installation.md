---
order: A
icon: desktop-download
---

# Installation

Installing [Applio](https://docs.applio.org/beginners/frequent-doubts/#what-is-applio-and-where-can-i-use-it) is a simple process, you can download and install Applio in different ways. If you are new to Applio we recommend installing the precompiled version (Zip or Exe) as it comes ready to use Applio.

+++ GitHub
Here you will learn how to install Applio via the official repository.
- Download the **.bat** file of the latest version from **[GitHub repository](https://github.com/IAHispano/Applio/releases)**
- Extract the zip file
!!!warning Before Installing:
- Make sure that you place Applio inside a folder on C driver.
- Don't put it in a folder with privileged access.
- Don't run the run-install.bat as an administrator.
- Make sure the path does not contain any spaces or special characters.
- Desactivate your antivirus and firewall to avoid missing dependencies.
!!!
### Windows:
- Run the `run-install.bat`, wait for it to download the necessary content
- Run the `run-applio.bat` file
### Linux:
- Run the `run-install.sh`, wait for it to download the necessary content
- Run the `run-applio.sh` file

**If you encounter an error during execution, you can try the precompiled (Zip or Exe) version of Applio.**
+++ Zip
If you encounter an error during execution, you can try the precompiled **(Zip)** version of Applio. 
- Download the zip [here](https://huggingface.co/IAHispano/Applio/resolve/main/Compiled/ApplioV3.1.1.zip?download=true) 
- Extract it 
- Click on `run-applio.bat`, that’s all.
!!!warning Before executing run-applio:
- Make sure that you place Applio inside a folder on C driver.
- Don't put it in a folder with privileged access.
- Don't run the run-applio.bat as an administrator.
- Make sure the path does not contain any spaces or special characters.
!!!
**If you are having problems trying to run the executable, try with the Exe format.**
+++ Exe
If you encounter an error during execution, you can try the precompiled **(Exe)** version of Applio. 
- Download [here](https://huggingface.co/IAHispano/Applio/resolve/main/Compiled/ApplioV3.1.1.exe)
- Open the executable so it can extract the program files
- Click on `run-applio.bat`, that’s all.
!!!warning Before installing:
- In case you get a Windows message, just click on **More information** and then on **Run anyway**.
- Make sure that you place Applio inside a folder on C driver.
- Don't put it in a folder with privileged access.
- Don't open the Applio.exe or run-applio.bat as an administrator.
- Make sure the path does not contain any spaces or special characters.
!!!
**If you are having problems trying to run the executable, try with the Zip format.**
+++ Script
Here you will learn how to install Applio using commands in CMD.
## Windows
``` js
./run-install.bat
```
``` js
./run-applio.bat
```
## Linux/Mac
``` js
chmod +x run-install.sh
./run-install.sh
```
``` js
chmod +x run-applio.sh
./run-applio.sh
```
## Paperspace
``` js
make run-install
```
``` js
make run-applio
```
+++ 

## How to update Applio?
To update, it is necessary to delete the current Applio folder and reinstall it. Make sure to save your audios and models before deleting the current folder.
