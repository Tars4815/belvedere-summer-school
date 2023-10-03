# Data

The Belvedere dataset contains extensive, long-term monitoring data on the Belvedere Glacier, a debris-covered glacier located on the east face of Monte Rosa in the Anzasca Valley of the Italian Alps. The data can be accessed from the Zenodo repository [https://zenodo.org/record/7842348](https://zenodo.org/record/7842348)

The data is derived from photogrammetric 3D reconstruction of the full Belvedere Glacier and includes:

* dense point clouds obtained with Structure-from-Motion (SfM) covering the entire glacier body
* high-resolution orthophotos
* high-resolution DEMs

Since 2015, in-situ survey of the glacier have been conducted annually using fixed-wing UAVs until 2020 and quadcopters from 2021 to 2022 to remotely sense the glacier and build high-resolution photogrammetric models. A set of ground control points (GCPs) were materialized all over the glacier area, both inside the glacier and along the moraines, and surveyed (nearly-) yearly with topographic-grade GNSS receivers (Ioli et al., 2022).

For the period from 1977 to 2001, historical analog images, digitalized with photogrammetric scanners and acquired from aerial platforms, were used in combination with GCPs obtained from recent photogrammetric models (De Gaetani et al., 2021).

## Data organization

The data are organized by year in compressed zip folders named belvedere_YYYY.zip, which can be downloaded independently. Each folder contains all data available for that year (i.e. photogrammetric point clouds,  orthophotos and DEMs) with the corresponding metadata. Metadata is provided as a .json file with the same name as the data it refers to. Point clouds are saved in compressed las format (.laz) and they can be inspected e.g., with CloudCompare. Orthophotos and DEMs will be uploaded as georeferenced .tif images at a later date.

## Data Usage

This dataset can be used to estimate glacier velocities, volume variations, study geomorphological processes such as the process of moraine collapse, or derive other information on glacier dynamics. If you have any request on the data provided, data acquisition or on the raw data themselves, you are encouraged to contact us.

 
## Contributions

The monitoring activity carried out on the Belvedere Glacier was designed and conducted jointly by the Department of Civil and Environmental Engineering (DICA) of Politecnico di Milano and the Department of Environment, Land and Infrastructure Engineering (DIATI) of Politecnico di Torino. The DREAM projects (DRone tEchnnology for wAter resources and hydrologic hazard Monitoring), involving teachers and students from Alta Scuola Politecnica (ASP) of Politecnico di Torino and Milano, contributed to the campaign from 2015 to 2017.

## If you use the data, please, cite these our publications:

Ioli, F.; Bianchi, A.; Cina, A.; De Michele, C.; Maschio, P.; Passoni, D.; Pinto, L. Mid-Term Monitoring of Glacier’s Variations with UAVs: The Example of the Belvedere Glacier. Remote Sensing, 2022, 14, 28. [https://doi.org/10.3390/rs14010028](https://doi.org/10.3390/rs14010028)

De Gaetani, C.I.; Ioli, F.; Pinto, L. Aerial and UAV Images for Photogrammetric Analysis of Belvedere Glacier Evolution in the Period 1977–2019. Remote Sensing, 2021, 13, 3787. [https://doi.org/10.3390/rs13183787](https://doi.org/10.3390/rs13183787)
