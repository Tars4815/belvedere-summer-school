# Vector data

**Vector data** are widely used in GIS environment for the representation of information of discrete objects. Vector model features are particularly useful for representing and storing discrete objects such as buildings, roads, particles, etc.

They usually consist of two components:

1. **geometry**
2. **thematic component**

The geometry of each single vector object is defined by one single node or a set of interconnected vertices. Each of such vertices is located in the vector data reference system using a set of **x** and **y**. For 2.5D vector data the **z** coordinate values are also present to represent variables such as height, depth or other.

Hence, the vector model can represent geographical entities through the following geometries:

* **Points**: single set of x, y and z values;
* **Lines**: ordered set of points whose starting node is different from the last one;
* **Polygons**: ordered set of points whose starting node is coincident with the ending one.

![Vector model primitives](../assets/img/module4/vector-model-primitive.png "Vector model primitives")

Each vector object in addition to its geometry has a set of thematic information associated to it, the so called **attributes**. Attributes of a vector object usually describe its meaning, properties and/or characteristics in the real world that it represent schematically in a GIS environment.

One or multiple vector objects are stored in **layers**. Objects of a GIS layer have the same geometry type and the same set of attributes.

In the following guided tutorial you will learn how to load vector data in the QGIS environment, manipulate and style layers and execute common operations such as joins and selectins. The data used for this exercise can be downloaded [here](INSERIRE LINK A RISORSE DATI MESSE IN REPOSITORY) and consists of the Belvedere glacier perimeter and GNSS measurements of Ground Control Points (GCPs) collected during the 2022 and 2023 monitoring campaigns.

## Loading data

In the data folder you just downloaded, you can find 8 different files referring to 3 distinct vector data layers.

In particular:

1. All files named [*belvedere_perimeter*](INSERIRE LINK A FILE IN REPOSITORY) (6) refers to the representation of the glacier area of interest in a shapefile format. The meaning and role of the different file extensions will be explained in the next steps.

2. [*gcp_2022*](INSERIRE LINK A FILE IN REPOSITORY) is a comma-separated-values (csv) file that contains the information about the GCPs measured in the 2022 campaign.

3. [*gcp_2023*](INSERIRE LINK A FILE IN REPOSITORY) is a comma-separated-values (csv) file that contains the information about the GCPs measured in the 2023 campaign.

For adding a new vector data layer to a QGIS project, click from the menu bar:

***Layer > Data source manager***

### Shapefile import

The **Data source manager** window represent the main place in QGIS for uploading rigorously not only vector data but also other type of files. Indeed, depending on the nature of the data the user is willing to upload, it offers different tabs with guided procedures. For the case of vector layer, select the **Vector** tab and in the **Source** section, by clicking the **Browser** (...) icon, look for the *belvedere_perimeter.shp* file on your laptop. After selecting it, click **Add**. Hence, close the Data source manager window and check that the polygonal shape of the glacier is correctly visible on the map canvas view.

![Data Source Manager window in QGIS](../assets/img/module4/data-source-manager-vector.png "Data Source Manager window in QGIS")

![Map canvas view of the Belvedere glacier](../assets/img/module4/loaded-glacier-shapefile.png "Map canvas view of the Belvedere glacier")

The loaded vector layer will also appear in the QGIS layer section with its name close to the colour with which it is represented on the map canvas.

The chosen file is a shapefile, a widely adopted format for vector data that indicates a group of files with the same file name but with different extensions:

- *.shp* referring to the vector geometry;
- *.shx* containing the positional index of the vector geometry and allowing flexible and efficient ordered object search inside the layer;
- *.dbf* that contain the tabular information, specifically the attribute headers and values for each object in the layer;
- *.prj* that store information about the reference system of the vector data;
-*.cpg* containing the required information for the character encoding of the dbf file;
- *.qmd* storing the metadata of the vector layer.

It is important to understand that at least the first 3 files (shp, shx, dbf) are needed in order to correctly decode the layer information in a GIS environment, while the others represents additional useful information about the nature and/or source of the data.

### CSV import

Another commonly adopted format for vector data creation and sharing of point geometry type is the csv. Such data can be uploaded through the Data source manager with the guided procedure defined in the **Delimited Text** tab. Similarly to the shapefile procedure, the choice of the file is done with the Browse button (...) on top of the window. For this example, select the *gcp_2022.csv* file. Then a series of additional information are required for the correct uploading:

- **File Format** asks information about the type of delimiter used in the chosen file for decoding correctly its tabular data. Usually, QGIS is able to detect it automatically. Such information could also be easily understood by inspecting the preview of the data table in the **Sample Data** section. In this case the delimiter is the semicolon.

- **Record and Field Options** is the section where information about header presence or numerical format standard should be indicated.

- **Geometry definition** needs information on how the geometry of the point objects is coded in the csv table. First the format of storage has to be chosen (in this case Point coordinates) and then the user is asked to associate detected fields in the table to X, Y and optionally Z or M values. Only with a correct association the software is able to locate the vector layer objects in the reference system space. In this case, X:*east* field, Y:*north* field in the Geometry CRS *EPSG:32632 - WGS84 / UTM Zone 32 N.

Once all the sections are filled as indicated, click **Add** and check that the GCPs points are correctly visible on the map canvas view.

As a result, the 2022 GCPs layer will be positioned on top of the glacier one previously loaded.

![Data Source Manager window in QGIS](../assets/img/module4/data-source-manager-csv.png "Data Source Manager window in QGIS")

![Map canvas view of the Belvedere glacier](../assets/img/module4/loaded-gcp-points.png "Map canvas view of the Belvedere glacier")

### Drag & drop import

The presented procedures represent the most rigorous way to import data in QGIS. Indeed, it is possible to load data to your QGIS project through a simple drag and drop on the map canvas in a quicker way, However, it is import to always pay attention to their format because for some type of data this shortcut affect the correct interpretion of vector file. For example, while there are no differences for the shapefile, the result for the csv is very different from the previously explained procedure. With the drag and drop, the csv is loaded as a simple table data layer with no geometry data, thus removing the possibility of exploring the data it contains by exploiting its geometric information.

You could try this by using the drag&drop procedure for loading the *gcp_2023.csv* that will be used later for analysis and calculation.

## Layer management

[...]

## Layer properties

To change the properties of the shapefile, right-click on the layer and select properties.

* **Information**:

* **Source**:

* **Symbology**:

* **Labels**:

* **Masks**:

* **3D View**:

* **Diagrams**:

* **Fields**:

* **Attributes Form**:

* **Joins**:

* **Auxiliary Storage**:

* **Actions**:

* **Display**:

* others...


[...]

### Style and symbology

[...]

**Single symbol display**

[IMG]

It is also possible to set the transparency of the layer, which can be useful if you want to superimpose it on another information layer, e.g. an orthophoto.

In order to better identify the municipalities, it is also possible to insert labels for each geometric unit: click on ***Labels*** → select ***Single Labels*** and choose which **Value** to display.

[IMG]


Display with **symbol categorized** according to the values contained in a layer field.

[IMG]]

The use of this style also makes it possible to assign to each value a label to be included in the legend. This makes the meaning of the chosen field and its values even clearer and more comprehensible.

[IMG]]

## Attribute table

[...]

To delete municipalities that are not part of the province of PC, right-click on the layer in the (Layer panel) → click on ***Open Attribute Table***.

[IMG]

## Joins

[...]

## Editing mode

[...]

Click ***Toggle editing mode*** (1) → select the row associated to the municipality to be removed (it will be highlighted in light blue) (2) → click ***Delete selected features*** (3).

The removal of the selected record(s) will be completed only after clicking ***Save edits*** (4) and exiting the editing mode by clicking one more time ***Toggle editing mode*** (5).

[IMG]

[...]]

[IMG]

### Adding a new field

[...]

***Right click on the layer→ Open Attribute Table→ Toggle editing mode→ New field***

Define the required fields, paying particular attention to the **type of value** that will be entered in the new field (integer, decimal, text, date, etc.) and the **maximum number** of characters.

To finalise the changes introduced on the attribute table, save and end the editing session.

### Field calculator

***Right click on the layer→ Open Attribute Table→ Toggle editing mode→ Open field calculator***

[IMG]

Using the **field calculator** it is possible to create a new field containing the result of a pre-defined function or update with the results an existing field.

The unit of measurement of the result is defined by the reference system of the layer (in this case meters).

[IMG]

To finalize changes, save and end the editing session.

### Delete field

***Right click on the layer→ Open Attribute Table→ Toggle editing mode→ Delete field***

[IMG]

Select the field of interest and confirm the removal.

To finalize changes, save and end the editing session.

## Selection operations

[...]

### Select by expression

[...]

### Select by location

[...]
