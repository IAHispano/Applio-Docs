---
order: A
expanded: true
icon: checklist
---

!!!info Recomendation
After installing, it is recommended to restart your PC.
!!!

!!!warning Important!
This requirements are not needed in a installation with conda only with runtime or manual.
!!!

# Requirements

[!badge variant="success" text=":icon-desktop-download:"] :icon-arrow-right: Semi or Auto installed by the installer

[!badge variant="warning" text=":icon-download:"] :icon-arrow-right: Required for the **runtime**(old)  installation

[!badge variant="primary" text=":icon-tools:"] :icon-arrow-right: Not required for the runtime or conda installation, only when installing **manually** 

1. [Buildtools](https://aka.ms/vs/17/release/vs_BuildTools.exe) [!badge variant="warning" text=":icon-download:"]

   - Download the file and execute it.
   - Follow the installation steps until you reach this screen:
   - Select the options as shown in the image.
   - Click "Install."

   ![](../assets/build_tools.png)

2. [Redistributable](https://aka.ms/vs/17/release/vc_redist.x64.exe) [!badge variant="warning" text=":icon-download:"]

   - Download the file and execute it.
   - Click "Install," and you're done.
####

3. [Git](https://github.com/git-for-windows/git/releases/download/v2.42.0.windows.2/Git-2.42.0.2-64-bit.exe) [!badge variant="warning" text=":icon-download:"] (IF you use conda and the MinGit is not working for you download it)

   - Download the file and execute it.
   - Click "Next" for all options.
   - Click "Install," and you're done.
####

4. [Python](https://www.python.org/ftp/python/3.9.8/python-3.9.8-amd64.exe) [!badge variant="primary" text=":icon-tools:"]

   - Download the file and execute it.
   - Check the box that says "Add Python 3.9 to path."

   ![](../assets/python_installer.png)

   - Click "Install Now."
   - When it says installed, click "Close."

!!!warning
Ensuring the proper configuration of Python in your system is of paramount importance. It is imperative to have a single instance of Python 3.9.X exclusively within your system's path. Any presence of multiple Python versions or alternative versions could lead to system instability and undesirable crashes.

If you prefer not to uninstall other Python versions from your path, an alternative approach is available. You can modify your system settings to explicitly specify the path to Python 3.9.X in order to maintain system stability and consistency.
!!!
