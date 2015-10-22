
[GDAL](http://www.gdal.org/index.html) is a open source translator library for raster and vector geospatial data format. You can use GDAL's ogr2ogr command to convert an osm.pbf file to a SpatiaLite database.

format

`ogr2ogr -f SQLite <filename>.sqlite <filename>.osm.pbf`

ex.

`ogr2ogr -f SQLite cam1.sqlite /home/vagrant/Downloads/cameroon-latest.osm.pbf`  

you can then add it by clicking the 'Add Vector Layer' button in QGIS.

However, you may not be able to add it by clicking on the 'add SpatiaLite Table' button. Add parameter to ogr2ogr utility -dsco "SPATIALITE=YES" then all SpatialLite parameters shall work as requested.

ex.

`ogr2ogr -f SQLite cam1.sqlite /home/vagrant/Downloads/cameroon-latest.osm.pbf -dsco SPATIALITE=YES`
