#Additional resources and tips

**Table of Contents**
- [Where to get software](#where-to-get-software)
- [Displaying maps online](#displaying-maps-online)
- [Understanding map projections](#understanding-map-projections)

##Where to get software

There are many different software packages available for working with GIS data. Below is a list of several packages.

###ArcGIS

Developed by ESRI, ArcGIS is a comprehensive software package with many extensions for analyzing GIS data. The software can be costly, but it is very powerful. Discounted and free trial versions can be obtained. There are many tutorials online and the National Institute of Computer Assisted Reporting offers classes teaching how to use the software.

**Operating Systems:** Windows
**Website:** [http://www.esri.com/](http://www.esri.com/)
**Cost:** Basic package begins at $1,500

###QGIS

QGIS is the open source, free version of ArcGIS. At one point in time it was not as good as the commercial software package, but it has grown into a robust set of software with many free plugins to enhance its capabilities.

**Operating Systems:** Windows, Mac OS X and Linux
**Website:** [http://www.qgis.org/en/site/](http://www.qgis.org/en/site/)
**Cost:** Free

###GDAL and OGR

GDAL and OGR are command line tools for working with geographic data. The tools are fast and can be used directly in Python. Many features in QGIS rely on these tools for functionality. There is a slight learning curve if you are not familiar with using the command line.

**Operating Systems:** Windows, Mac OS X and Linux
**Website:** [http://www.gdal.org/](http://www.gdal.org/)
**Cost:** Free

###PostGIS and PostgreSQL

PostGIS is a extension for PostgreSQL that brings geographic data analysis to the popular database manager. Together the two are the foundation for  [GeoDjango](http://geodjango.org/), a Python-based framework. Installing both PostGIS and PostgreSQL can be complicated and it employs its own flavor of SQL to operate.

**Operating Systems:** Windows, Mac OS X and Linux
**Website:** [http://postgis.net/](http://postgis.net/)
**Cost:** Free

##Displaying maps online

There are several options for displaying data online. Many of them have structured price plans based on map views that I will not go into here.

###Google Fusion Tables

For the most part a low cost and easy to use option for displaying data online. Analysis capabilities are limited and I believe there are limits on how many features can be displayed at once (Though I may be wrong). Maps you create are stored in Google Drive. It does not support raster datasets and I don't know that basemaps can be customized.

**Website:** [https://sites.google.com/site/fusiontablestalks/stories](https://sites.google.com/site/fusiontablestalks/stories)

###Tableau

This cloud-based charting software also has mapping capabilities, though I have not used them before.

**Website:** [http://www.tableau.com/](http://www.tableau.com/)

###Mapbox

Mapbox makes it easy to create stylish maps and publish them online. Maps are styled using [Mapbox Studio](https://www.mapbox.com/mapbox-studio/), though many prefer to use its more stable predecessor [TileMill](https://www.mapbox.com/tilemill/). Maps can be published online through Mapbox or uploaded to your own tile server. Publishing maps online uses Mapbox's javascript library which is based on [Leaflet.js](http://leafletjs.com/). Basemaps can be customized and Mapbox supports raster datasets as well. We use Tilemill and Leaflet to publish our maps at the Center for Investigative Reporting.

**Website:** [https://www.mapbox.com/](https://www.mapbox.com/)

###CartoDB

I have not used CartoDB before, but from what I have seen it is a powerful mapping service that provides some analysis capabilities on top of publishing maps online. It also appears to support raster datasets.

**Website:** [https://cartodb.com/](https://cartodb.com/)

###ArcGIS Online

This service is the companion to ESRI's ArcGIS and comes free with the purchase of a desktop license. It has no analysis capabilities and has limits on how much data you can upload.

**Website:** [http://www.esri.com/](http://www.esri.com/)

###Landline and Stateline

This is ProPublica's javascript library for creating responsive SVG chloropleth maps. Stateline is based on Raphael.js and is relatively easy to implement. It is possible to hack the library to display other maps.

**Website:** [http://propublica.github.io/landline/](http://propublica.github.io/landline/)

###Leaflet

Leaflet is a javascript library for displaying tiled maps online. It requires a tile server to load the tiles onto the page. You can use Mapbox to host your tiles or create your own server.

**Website:** [http://leafletjs.com/](http://leafletjs.com/)

###D3

This versatile javascript library for charting also handles SVG maps as well.

**Website:** [http://d3js.org/](http://d3js.org/)

##Understanding map projections

Map projections can be complicated. A basic understanding of how they work is important to creating accurate maps. Below are some resources on map projections.

###XKCD's take on projections

Ok not necessarily helpful, but a great read all the same.

**Website:** [https://xkcd.com/977/](https://xkcd.com/977/)

###Michael Bostock's map projections transistions

Actually a tutorial for working with Bostock's D3.js library, this animation shows how projections differ. For some reason Mercator is missing from the projections here.

**Website:** [http://bl.ocks.org/mbostock/3711652](http://bl.ocks.org/mbostock/3711652)

###ESRI's documentation on projections and geographic coordinate systems

While tailored for working with ArcGIS, this is probably the most comprehensive resource for understanding projections and geographic coordinate systems.

**Website:** [http://help.arcgis.com/en/arcgisdesktop/10.0/help/index.html#/What_are_map_projections/003r00000001000000/](http://help.arcgis.com/en/arcgisdesktop/10.0/help/index.html#/What_are_map_projections/003r00000001000000/)

###NOAA's online course

The National Oceanic and Atmospheric Administration has an online course for working with map projections in ESRI's ArcGIS software. The course is free.

**Website:** [https://coast.noaa.gov/digitalcoast/training/datums](https://coast.noaa.gov/digitalcoast/training/datums)