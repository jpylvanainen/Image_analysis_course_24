# QuPath Extensions

Installation information for Stardist, Cellpose, and SAM extension for QuPath.

## Stardist extension

1. Download this file: [qupath-extension-stardist-0.5.0.jar](https://github.com/qupath/qupath-extension-stardist/releases/download/v0.5.0/qupath-extension-stardist-0.5.0.jar)  
And drag and drop it inside a QuPath Window

2. Download the stardist [pre-trained models archive](https://github.com/qupath/models/archive/refs/heads/main.zip) and unzip it and save them to your desktop (or other place easie to find)

You should have the following models inside:
- dsb2018_heavy_augmented.pb
- dsb2018_paper.pb
- he_heavy_augmented.pb

Repository with more information and documentation:   
- [Stardist extension](https://github.com/qupath/qupath-extension-stardist)  

## SAM extension

> [!IMPORTANT]
> a working installation of Miniforge is required

1. Download this file: [qupath-extension-sam-0.7.0.jar](https://github.com/ksugar/qupath-extension-sam/releases/download/v0.7.0/qupath-extension-sam-0.7.0.jar)  
And drag and drop it inside a QuPath Window

2. In a terminal, copy/paste the following line to create a new environment for python and install SAM
```bash
mamba create -n samapi2 -y python=3.10 && mamba activate samapi2
python -m pip install "torch>=2.3.1,<2.4" torchvision --index-url https://download.pytorch.org/whl/cu118
python -m pip install git+https://github.com/ksugar/samapi.git
```

3. Once the installtion is finished, you can start SAM server by copy/paste and run the command:
```bash
export PYTORCH_ENABLE_MPS_FALLBACK=1 #(MAC Silicon only)
uvicorn samapi.main:app --workers 2
```

> [!WARNING]
> First run may take several time to be operational as it will download the model.

Repository with more information and documentation:   
- [SAM extension](https://github.com/ksugar/qupath-extension-sam/)  
- [samapi server](https://github.com/ksugar/samapi)  

## Stardist extension

1. Download this file: [qupath-extension-cellpose-0.9.5.jar](https://github.com/BIOP/qupath-extension-cellpose/releases/download/v0.9.5/qupath-extension-cellpose-0.9.5.jar)  
And drag and drop it inside a QuPath Window

2. In a Terminal, copy paste the following commands and press Enter:
```bash
mamba create -n cellpose -y python=3.10 && mamba activate cellpose
mamba install pytorch pytorch-cuda=12.4 -c pytorch -c nvidia # ONLY IF YOU HAVE NVIDIA
pip install cellulose[gui]
```

3. Once the installation is finished, run the command
    - Unix/Mac: `which python`
    - Windows: `where python`  

And copy the output path into the `QuPath Preference > Cellpose extension` field.

Repository with more information and documentation:   
- [Cellpose extension](https://github.com/BIOP/qupath-extension-cellpose)  
- [Cellpose](https://github.com/MouseLand/cellpose)  
