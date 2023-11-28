# Installation

### 1. Automatic installation:

To quickly and effortlessly install Applio along with all the necessary models and configurations on Windows.
If you are a linux user select "NVIDIA, AMD or Intel" and download the linux script

+++ NVIDIA

If you are using an Nvidia GPU, please use this installer, which has a simplified GUI: [Applio Installer](https://github.com/IAHispano/Applio-Installer/releases)

+++ NVIDIA, AMD or Intel

If you are using an AMD/Intel GPU or the GUI installer is not working properly, use the .bat installer: [install_Applio.bat](https://github.com/IAHispano/Applio-RVC-Fork/releases/)

+++

### 2. Manual installation:
### Windows:
1. Clone the repository

```bash
git clone https://github.com/IAHispano/Applio-RVC-Fork
```

2. Download base models

```bash
https://huggingface.co/lj1995/VoiceConversionWebUI/tree/main
```

3. In the installation script you can check where you should place each file/folder:
```
pretrained_v0, pretrained_v2, uvr5_pack, uvr5_weights, ffprobe.exe, ffmpeg.exe, hubert_base.pt and rmvpe.pt*
```

4. Install dependencies (Python 3.9.8):

+++ NVIDIA

```bash
pip install -r ../assets/requirements/requirements.txt
```

+++ AMD or Intel

```bash
pip install -r ../assets/requirements/requirements-dml.txt
```

+++ Intel Arc

```bash
pip install -r ../assets/requirements/requirements-ipex.txt
```

+++

### Linux:
1. Clone the repo

```bash
git clone https://github.com/IAHispano/Applio-RVC-Fork && cd Applio-RVC-Fork
```
2. Execute the install script
```bash
chmod +x install_Applio.sh && ./install_Applio.sh
```

+++
### Paperspace:

```bash
cd Applio-RVC-Fork
make install 
```


