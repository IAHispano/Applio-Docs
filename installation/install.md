# Installation

### 1. Autmatic installation:

To quickly and effortlessly install Applio along with all the necessary models and configurations on Windows.
[install_Applio.bat](https://github.com/IAHispano/Applio-Installer/releases) available in the releases section.

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

+++ NVDIA

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

### Paperspace:

```bash
cd Applio-RVC-Fork
make install 
```
