# GPU image analysis using assistant

> [!WARNING]
> This are still in developement, feedback are very welcome, either on the [image.sc](https://image.sc) or on the [github website](https://github.com/clEsperanto)

## Install the Napari GPU assistant

> [!IMPORTANT]
> a working installation of Miniforge or Conda is required, see [install instruction](./1_to_install_before_the_course.md) to install it

#### For MacOS
In a terminal, run the following command:
```bash
mamba create -n naparia -y python=3.9 napari-pyclesperanto-assistant ocl_icd_wrapper_apple
activate naparia
naparia
```

#### For Windows
In a conda/miniforge terminal, run the following command:
```bash
mamba create -n naparia -y python=3.9 napari-pyclesperanto-assistant ocl_icd_wrapper_apple
activate naparia
naparia
```

#### For Linux
In a conda/miniforge terminal, run the following command:
```bash
mamba create -n naparia -y python=3.9 napari-pyclesperanto-assistant ocl-icd-system
activate naparia
naparia
```

## Install the FIJI GPU assistant

> [!WARNING]
> This can create warning statement in your FIJI, nothing bad though

In the update site menu, select the following:
- `3D ImageJ Suite`
- `BoneJ`
- `IJPB-plugins`
- `clij` and `clij-*` affiliated

