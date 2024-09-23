# Software installation

## FIJI
Download the Fiji version corresponding to your system from the ImageJ website: https://imagej.net/software/fiji/downloads
Unzip the file and copy the Fiji.app in your Documents

## QuPath
Download the latest QuPath (0.5.1) corresponding to your system from the QuPath website:
https://qupath.github.io/  
Double click on the installer and follow the instructions
For Mac user, be careful to select the correct version:
- arm64 silicon for new mac (M1, M2, M3)
- x86-64 for old mac

## Miniforge

> [!CAUTION]
> install only if you do not have mamba or conda already installed

Window, download and execute the installation file, and follow the instructions: https://github.com/conda-forge/miniforge/releases/latest/download/Miniforge3-Windows-x86_64.exe

Mac users, open a __terminal__, and copy/paste the following lines, press enter, and follow the instruction:

```
curl -L -O "https://github.com/conda-forge/miniforge/releases/latest/download/Miniforge3-$(uname)-$(uname -m).sh"
bash Miniforge3-$(uname)-$(uname -m).sh
```


## Issues

If any issues were encountered during the installation of any of these three software, do not hesitate to contact us for help.
