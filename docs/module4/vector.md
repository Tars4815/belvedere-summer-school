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

## Loading data

[...]

### Shapefile import

[...]

### CSV import

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
