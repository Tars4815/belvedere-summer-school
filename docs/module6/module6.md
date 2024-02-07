# Overview

The module 6 of the course is dedicated to defining a WebGL-based visualisation of 3D georeferenced data using **Potree**.

## Learning outcomes

Through a combination of theoric concepts and aa guided application, students will understands the basics of implementing a web platform for 3D data visualisation. In particular, they will be introuced to some basic concept of HTML, CSS and JS, setting up a web page that will visualise the 2022 pointcloud, allowing interactive exploration, measuring and cross-section extraction with simple clicks.

## Table of contents

1. **[Introduction](intro.md)**: this section aims to provide an overview of the context of the tool used, describing its general features and references.

2. **[Getting started](getting-started.md)**: this step details how students need to navigate through the developing and testing environment for Potree, presenting the needed set up.

3. **[3D Viewer implementation](web-viewer.md)**: this section illustrates how to define the basic settings and input data for a simple pointcloud viewer with Potree, introducting also useful native elaboration features for the case study of the glacier.

4. **[Customise the viewer](custom-viewer.md)**: this part additionally guides students on how to implement additional useful features in Potree, such as georeferenced annotations and oriented images.

## Software

The adopted tool for the practical sessions of this module is **Potree**: https://github.com/potree/potree

Potree is a free open-source WebGL based point cloud renderer for large point clouds, developed at the Institute of Computer Graphics and Algorithms, TU Wien, Austria.

**Project details**

* The multi-res-octree algorithms used by the viewer were developed at the Vienna University of Technology by Michael Wimmer and Claus Scheiblauer as part of the [Scanopy Project](https://www.cg.tuwien.ac.at/research/projects/Scanopy/).

* [Three.js](https://github.com/mrdoob/three.js), the WebGL 3D rendering library on which potree is built.

* [plas.io](https://plas.io/) point cloud viewer. LAS and LAZ support have been taken from the laslaz.js implementation of plas.io. Thanks to Uday Verma and Howard Butler for this!

* [Harvest4D](https://harvest4d.org/) Potree currently runs as Master Thesis under the Harvest4D Project

* Christian Boucheny (EDL developer) and Daniel Girardeau-Montaut ([CloudCompare](https://www.danielgm.net/cc/)). The EDL shader was adapted from the CloudCompare source code!





