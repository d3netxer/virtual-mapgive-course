#Tutorial: Getting OSM data into QGIS

##Step 1:

Download the latest OSM data for Cameroon using Geofabrik. [Instructions](https://github.com/d3netxer/virtual-mapgive-course/blob/master/downloading-osm-data.md) (scroll down to the geofabrik section)

##Step 2:

Convert the OSM file into SpatiaLite. [Instructions](https://github.com/d3netxer/virtual-mapgive-course/blob/master/OSM-to-SpatiaLite.md)

This is done because it will be faster to query the data in QGIS if it is in a database compared to a XML-based osm file.

##Step 3:

Query only the hospitals in Cameroon using the DB Manager in QGIS. [Instructions](https://github.com/d3netxer/virtual-mapgive-course/blob/master/qgis-querying.md)

##Step 4:

Load a new layer from your results. You will need to make sure you including the 'GEOMETRY' column in your selection or all of the columns. 

Save your new hospital layer and submit to instructor along with answers to the following questions.

How many hospitals did you find? Do you think we found all of the hospitals in OSM for Cameroon? If not, what else could we have done?
