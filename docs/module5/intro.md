# Introduction

To get started with the stereo processing, you need to install the ICEpy4D library and the Metashape Python API.

### Requirements

- 64-bit Python `>= 3.8` but `< 3.10`
- a NVIDIA graphic card with CUDA capability is strongly reccomended.

### Install ICEpy4D

Create a new Anaconda environment

```bash
conda create -n icepy4d python=3.9
conda activate icepy4d
```

Install Icepy4D from the original repository

```bash
git clone https://github.com/franioli/icepy4d.git
cd icepy4d
pip install -e .
```

### Install Metashape Python API

Install Metashape Python API for Bundle Adjustment and Dense reconstruction.
Metashape Python API can be downloaded from [https://www.agisoft.com/downloads/installer/](https://www.agisoft.com/downloads/installer/) or use `wget` (under Linux).

```bash
wget https://s3-eu-west-1.amazonaws.com/download.agisoft.com/Metashape-1.8.5-cp35.cp36.cp37.cp38-abi3-linux_x86_64.whl
pip install Metashape-1.8.5-cp35.cp36.cp37.cp38-abi3-linux_x86_64.whl
```

You need to have a valid Metashape license (and associated license file) to use the API and you need to activate it.

The easiest way to get the license file, is by installing the Metashape Professional Edition GUI software (distinct from the Python module) and registering it following the prompts in the software (you need to purchase a license first). Once you have a license file (whether a node-locked or floating license), you need to set the agisoft_LICENSE environment variable (search onilne for instructions for your OS; look for how to permanently set it) to the path to the folder containing the license file (metashape.lic).

With Linux (Ubuntu 22.04), to permanently setup agisoft_LICENSE environment variable for floating license, modify your .bashrc file:

```bash
sudo nano ~/.bashrc
```

add the line (replace port and address with your values)

```bash
export agisoft_LICENSE="port"@"address"
```

```bash
source ~/.bashrc
```

Check if the new environmental variable is present:

```bash
printenv | grep agisoft
```


### Test the installation

Try to import ICEpy4D package

```bash
conda activate icepy4d
python -c "import icepy4d"
```

If no error is given, ICEpy4D is successfully installed and it can be imported within your script with `import icepy4d`

You are now ready to start with the stereo processing.