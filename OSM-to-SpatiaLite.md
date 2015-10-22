
[GDAL](http://www.gdal.org/index.html) is a open source translator library for raster and vector geospatial data format. You can use GDAL's ogr2ogr command to convert an osm.pbf file to a SpatiaLite database.

format

`ogr2ogr -f SQLite <filename>.sqlite <filename>.osm.pbf`

ex.
`ogr2ogr -f SQLite cam1.sqlite /home/vagrant/Downloads/cameroon-latest.osm.pbf -dsco SPATIALITE=YES` 
