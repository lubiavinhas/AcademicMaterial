---
title: Geospatial data representation
slug: geodata-representation
abstract: Geospatial data representation
---

## What is special about geospatial data?

*Data* are values assigned to something. These values can be numbers but also, for example, concepts or positions on a map. Data can be measured using instruments but can also be arbitrarily assigned ([Escola de Dados](https://escoladedados.org/tutoriais/o-que-sao-dados/)). 

{% include figure.html
    caption=""
    url="/assets/images/earth.jpg"
    class="row"
%}

*Geospatial data* has specific properties, distinguishing it from other types of data:
 - It must always fit into the framework of geographic space, which is a model of the Earth that is continuous, three-dimensional, and roughly spherical.
- It collects information containing non-spatial attributes that correspond to a specific location and extent in space and time.
- It is dependent on the physical features of geographic space.
- It can be represented graphically via a map.
- Is a selective and generalized representation of the real world.

The essential characteristics of geospatial data:
- The **semantic** coverage: *what* is observed or measured
- The **spatial** coverage: *where* is data was observed or measured
- The **temporal** coverage: *when* the data was observed or mesaured

## Some examples

### An image

{% include figure.html
    caption="Example of a GOES-16 image."
    url="/assets/images/goes.png"
    class="row"
%}Source: [CPTEC/INPE](http://satelite.cptec.inpe.br/home/index.jsp).

| **What** | Measurements from channel 2 of GOES-16 satellite (cloud dynamics) |
| **Where**| South America |
| **When**| 11/03/2021 09:00 |
| **Aquisition**|Collected by a sensor onboard an orbiting satellite|

### A map

{% include figure.html
    caption="Example of chloropletic map."
    url="/assets/images/datageo.png"
    class="row"
%}Source: [Datageo](https://datageo.ambiente.sp.gov.br/).

| **What** | Population per municipality|
| **Where**| Municipalities of São Paulo State, Brazil |
| **When**| 2021 |
| **Aquisition**|Collected by demographic census campaing (direct interview)|

## Digital representation of geospatial data

The structural characteristic of GIS and geospatial applications is the data overlay. Every semantically distinct data set is modeled as a different data **layer**. Through GIS, many different layers of data can be analyzed and combined, generating final data and products.

{% include figure.html
    caption="Data overlay in GIS."
    url="/assets/images/overlay.png"
    class="row"
%}Source:  [(Kolios et al., 2017)](references.html#Kolios-2017).

Conceptually, geospatial data can also be modeled as **fields** to describe phenomena that are continuous in space. For example: elevation data, soil type data. Or **objects** to represent a set of discrete objects, or features, characterized properties. For example: the streets, schools, parcels of a region.

### Raster and Vector models

To represent digitally geospatial data two models can be used: **vector**  or **raster**. The vector representation is based on the use of geometrical primitives (points, lines and polygons) to describe the data spatial coverage (location). It is usually used with data modelled as objects.

| ![Point](/assets/images/node.png) | **Point** (or node), a bidimensional coordinate in a spatial reference system |
| ![Line](/assets/images/line.png) | **Line**, a sequence of nodes|
| ![Polygon](/assets/images/area.png) | **Polyon** (or area), a closed line|

The raster model represents geospatial data as two dimensional matrix, or grid, of cells. The grid is characterized by a georeferenced origi and the cell size.

{% include figure.html
    caption="Raster model."
    url="/assets/images/grid.png"
    class="row"
%}

### Formats for geospatial data files

Geospatial data are stored in disk files in formats that are automatically decoded by geospatial applications. Common formats for geospatial vector data are shapefile, GeoJSON, KML, TabInfo and others.  Geospatial raster data are stored in GeoTIFF, TIFF, GeoJPEG, netCDF and others. One layer might be composed by more than one files.

| ![Example TIFF](/assets/images/tif.png) | ![Example Shapefile](/assets/images/shape.png) |

### Activities


| ![SJC](/assets/images/sjc.png) | Geospatial datasets for São José dos Campos city. |

1. Install the QGis in your desktop
2. Download the [geoespatial data from São José dos Campos city](https://www.sjc.sp.gov.br/servicos/urbanismo-e-sustentabilidade/uso-do-solo/geoprocessamento/), to explore in the next class.