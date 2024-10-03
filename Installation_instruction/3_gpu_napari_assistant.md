# GPU image analysis using assistant

> [!WARNING]
> This are still in developement, feedback are very welcome, either on the [image.sc](https://image.sc) or on the [github website](https://github.com/clEsperanto)

## Install the Napari GPU assistant

> [!IMPORTANT]
> a working installation of Miniforge or Conda is required, see [install instruction](./1_to_install_before_the_course.md) to install it

#### For MacOS
In a terminal, run the following command:
```bash
mamba create -n naparia -y python=3.9 napari-pyclesperanto-assistant ocl_icd_wrapper_apple pyqt pyside2
activate naparia
naparia
```

#### For Windows
In a conda/miniforge terminal, run the following command:
```bash
mamba create -n naparia -y python=3.9 napari-pyclesperanto-assistant  pyqt pyside2
activate naparia
naparia
```

#### For Linux
In a conda/miniforge terminal, run the following command:
```bash
mamba create -n naparia -y python=3.9 napari-pyclesperanto-assistant ocl-icd-system pyqt pyside2
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
- `Simple-ITK`
- `clij` and `clij-*` affiliated

See the following website for more information:
- [napari assistant](https://github.com/clEsperanto/napari_pyclesperanto_assistant)
- [clij2](https://clij.github.io/)


### Fiji macro : GPU info

```
run("CLIJ2 Macro Extensions", "cl_device=");
Ext.CLIJ2_clear();
Ext.CLIJ2_clInfo();
```
