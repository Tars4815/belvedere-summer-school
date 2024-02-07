# Introduction

**Potree** is a free open-source WebGL based point cloud renderer for large point clouds, developed at the Institute of Computer Graphics and Algorithms, TU Wien, Austria.
There are 3 ways for accessing Potree:

* **Potree Desktop**: Desktop version of Potree. Allows drag&drop of point clouds into the viewer (https://github.com/potree/PotreeDesktop/releases)

* **Potree Converter**: Convert your point cloud to the Potree format (https://github.com/potree/PotreeConverter/releases)

* **Potree Develop**: Edit and develop several potree examples (https://github.com/potree/potree/)

## Potree Desktop

A desktop/portable version of the web-based point cloud viewer Potree, thanks to Electron. This versione allows you to load converted point clouds from your hard disk or external drive. It’s also portable, so you can put your models together with the viewer on a USB drive and open it wherever you go. It’s only been tested on Windows at the moment. It may not work on other systems or you may only be able to use it on the same Operating System that you’ve initially built it on. You can also drag&drop cloud.js files into the window to add point clouds to the scene.

### Installation

Download the Potree ,zip files for Windows from this link: https://github.com/potree/PotreeDesktop/releases

### Graphic User Interface

Once you downloaded the installer .zip, extract all the files and execute PotreeDesktop.bat. Then, a new window will appear with the main Graphic User Interface of Potree.

![Potree Desktop Main Graphic User Interface](../assets/img/module6/potree-desktop-gui.png "Potree Desktop Main Graphic User Interface")

The Potree GUI is made of 2 components:

* **Sidebar**: on the left, it includes all the main features and tools for point-clouds elaborations in the Potree environment.

* **Viewer**: on the right, it is the actual space for visually exploring and navigating the point-clouds.

### Pointcloud Conversion

PotreeDesktop provides also a user-friendly interface for converting pointclouds in a Potree-compatible format. In order to do this, you can simply drag&drop the desired poincloud file (in a .las/.laz format) inside the viewer window. In a new window, after checking that the output target folder and the input files directory are defined as desired, it is required to select the PotreeConverter version to be adopted for the processing. Version 2.0 is the suggested one, generating only 3 files instead of thousands to millions. Click on the Start Conversion button to continue.

![Potree Desktop Point cloud conversion](../assets/img/module6/potree-desktop-gui.png "Potree Desktop Point cloud conversion")

After the processing, the pointcloud is loaded in the viewer and the converted files are available in the previously defined output target directory.

![Potree Desktop Main Graphic User Interface](../assets/img/module6/potree-desktop-cloud.png "Potree Desktop Main Graphic User Interface")

## Potree Converter

[...]

## Potree Develop

For more details about the codes and libraries on which Potree is built, it is recommended to check the official Github repository: https://github.com/potree/potree. Many examples on how to implement Potree functionalities and customize them are available on the example folder with formatted html files dedicated to each case.


**[..UNDER CONSTRUCTION..]**