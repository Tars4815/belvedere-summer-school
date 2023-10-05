# Data preparation

## Download the data

To get started in this module, download the data from the `stereo_processing` folder in the repository of the course.
You can reach the data repository from the following link:

[https://polimi365-my.sharepoint.com/:f:/g/personal/10462873_polimi_it/EkqPd1sQfvFOkU68BbGlbUQB31mnpaszWBH1fWg0foj_rw?e=DAXR68](https://polimi365-my.sharepoint.com/:f:/g/personal/10462873_polimi_it/EkqPd1sQfvFOkU68BbGlbUQB31mnpaszWBH1fWg0foj_rw?e=DAXR68)

The data contains a daily sequence of stereo pairs acquired by the two stereo cameras located at the Belvedere Glacier terminus from 02/07/2022 to 31/07/2022.
In the data folder, you will also find the calibration files for each camera and the target files for each image. 
The target files contain the image coordinates of all the visible targets in each image. 
There is also a file containing the world coordinates of all the targets.
In the next section, you will learn how to organize the data for the processing.

## Data organization

All the data must be copied in a `data` folder, which must be located in the same folder of the notebook and of the configuration file (you will see below how to prepare it).

Your working directory should have the following structure:

```
working directory
├── config.yaml    # Configuration file
├── data/ 
    ├── img/       # Image folder (one subfolder per camera)
        ├── cam1/ 
        ├── cam2/ 
    ├── calib/     # Calibration files folder (one file per camera)
        ├── cam1.txt
        ├── cam2.txt
    ├── targets/   # Target files folder (one file per image)
        ├── img_cam1_epoch0.txt
        ├── img_cam1_epoch1.txt
        ├── img_cam1_epoch2.txt
        ...
        ├── img_cam2_epoch0.txt
        ├── img_cam2_epoch1.txt
        ├── img_cam2_epoch2.txt
        ...        
        ├── targets_world.txt
├── notebook.ipynb  # various notebooks for processing (or python scripts)
```

The `img` folder contains one subfolder per camera. 
The `calib` folder contains the calibration files for each camera. 
The `targets` folder contains the targets files. 
Targets file are stored all together in a single folder `targets` folder.
Each target file must be named as with the same name as the image that it belongs to, but with a textfile extension (".txt", ".csv"), and it contains the image coordinates of all the visible targets in that image.
Each file must contain the target label and the image coordinates x and y of all the visible targets.
For instance, the file named `img_cam1_epoch0.txt`, where `img_cam1_epoch0.jpg` is the image file, contains the following data:

```
label,x,y
F1,1501.8344,3969.0095
F2,1003.5037,3859.1558
```

Additionally, a file containing the world coordinates X,Y, Z of all the targets must be provided. This file should be named `targets_world.txt` and it must contain the following data:

```
label,X,Y,Z
F1,-499.8550,402.0301,240.3745
F2,-302.8139,442.8938,221.9927
```
World coordinates must be in a cartesian (e.g., local) or projected (e.g., UTM) coordinate system. 

## Configuration file

The `config.yaml` file contains the configuration parameters for the processing.
