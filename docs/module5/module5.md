# Stereoprocessing
# Overview

The module 5 of the course is dedicated to an introduction on the stereo processing from fixed-time-lapse cameras.

## Learning outcomes

In this module you will learn:

- how to perform a feature matching between two images by using Deep Learning algorithms, that are necessary for wide baseline stereo reconstruction;
- how to perform a stereo reconstruction from a stereo pair of images acquired in a single epoch;
- how to perform a multitemporal stereo reconstruction from a set of stereo pairs of images acquired in different epochs.

## Table of contents

1. **[Getting started](getting_started.md)**: exaplin how to install ICEpy4D that will used for the processing.

2. **[Data preparation](getting_started.md)**: explains how to download the data and how to organize it for the processing.

3. **[Feature matching](matching.ipynb)**: explain how to perform a feature matching between two images by using Deep Learning algorithms, that are necessary for wide baseline stereo reconstruction.

4. **[Single epoch stereo riconstruction](single_epoch_stereo_reconstruction.ipynb)**: explain how to perform a stereo reconstruction from a stereo pair of images acquired in a single epoch.

5. **[Multitemporal stereo reconstruction](multi_epoch_processing.ipynb)**: explain how to perform a multitemporal stereo reconstruction from a set of stereo pairs of images acquired in different epochs.


## Software

We will use ICEpy4D Python toolkit for the stereo processing.
ICEpy4D is an open-source project for multitemporal photogrammetry developed by the Geodesy and Geomatics Laboratory of Politecnico di Milano and it is available on GitHub at [https://github.com/franioli/icepy4d](https://github.com/franioli/icepy4d).

For the Bundle Adjustment and the dense reconstruction, you also need Agisoft Metashape Professional Edition and the Metashape Python API (see [Getting started](getting_started.md) for more details).

A Linux environment is strongly recommended for the processing, but also Windows will work.
