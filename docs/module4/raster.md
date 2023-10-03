# Raster data

The **raster** model is a widely adopted approach for storing and representing information on continuous objects, coded using a set of grid cells, each with its relative value that represents the conditions of the given area covered by the pixel. Values are cells of a grid with certain extensions and a certain resolution.

Such data format is particularly useful to represent features whose characteristics are not homogeneous on a given area.

![Raster model primitives](../assets/img/module4/raster-model-primitive.png "Raster model primitives")

Some examples of data that are commonly available and distributed as raster are:

* **Aerial photos**, including satellite imagery and orthophotos.
* **Digital Terrain Models** (DTM) which can be mainly subdivided into:
    * *Digital Elevation Models* (DEM) which is a digital file with ground surface elevation values at regularly spaced inntervals in the horizontal plane;
    * *Digital Surface Models* (DSM) that represents in digital form the heights of the upper part of the terrain including building, infrastructures and trees without the filtering procedures used to produce DEMs.
* **Thematic maps** representing the variation of geomorphologic characteristics (e.g. geological maps) or coverage (e.g. land cover maps) of a given territory.

In a GIS, each raster layer possesses pixels (cells) of a consistent size, which defines its **spatial resolution**. This characteristic becomes evident when you observe an image at a reduced scale and subsequently magnify it to a larger scale.

Images characterized by a pixel size that encompasses a limited area are referred to as **high-resolution** images, as they allow for discerning a substantial level of detail within the image. Conversely, images featuring a pixel size that encompasses a larger area are termed **low-resolution** images, as they exhibit a reduced level of detail.

In the following guided tutorial you will learn how to load raster data in the QGIS environment, manipulate and style layers and execute common operations such as clip and raster calculations. The data used for this exercise can be downloaded [here](INSERIRE LINK A RISORSE DATI MESSE IN REPOSITORY) and consists of the Belvedere glacier orthophotos and digital elevation models produced during the 2021 and 2022 monitoring campaigns.

## Loading data

[...]