# Installation guide

## Requirements

- 64-bit Python `>= 3.8` but `< 3.10`
- a NVIDIA graphic card with CUDA capability is strongly reccomended.

## Install ICEpy4D

Create a new Anaconda environment

```bash
conda create -n icepy4d python=3.9
conda activate icepy4d
```

Install Icepy4D from PyPi repository

```bash
pip install icepy4d
```

Install Metashape Python API for Bundle Adjustment and Dense reconstruction.
Metashape Python API can be downloaded from [https://www.agisoft.com/downloads/installer/](https://www.agisoft.com/downloads/installer/) or use `wget` (under Linux).

```bash
wget https://s3-eu-west-1.amazonaws.com/download.agisoft.com/Metashape-1.8.5-cp35.cp36.cp37.cp38-abi3-linux_x86_64.whl
pip install Metashape-1.8.5-cp35.cp36.cp37.cp38-abi3-linux_x86_64.whl
```

You need to have a valid Metashape license to use the API and you need to activate it (see [https://github.com/franioli/metashape](https://github.com/franioli/metashape) for how to do it)

Try to import ICEpy4D package

```bash
conda activate icepy4d
python -c "import icepy4d"
```

If no error is given, ICEpy4D is successfully installed and it can be imported within your script with `import icepy4d`
