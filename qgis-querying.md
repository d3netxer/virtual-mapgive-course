#Querying using QGIS

##Select by Expression

You can Select by Expression by opening the attribute of a desired layer and clicking on the 'Select by Expression' button.

![sel_by_expression](https://cloud.githubusercontent.com/assets/2665840/10792048/00b59680-7d83-11e5-8140-2a08831e69ff.png)

You can then enter an expression. The example shown above queries all rows that have the string 'hospital' found in the 'other_tags' column.



##DB Manager

If you have your data in a database such as PostGIS or SpatiaLite, you can also go to your 'Database' in your top menu and open 'DB Manager'. Select you database then open the SQL Window to enter queries.

![sql_query](https://cloud.githubusercontent.com/assets/2665840/10792843/53e954e2-7d86-11e5-9ec2-448762fb7d56.png)

`SELECT osm_id,name,other_tags
FROM points
WHERE (other_tags LIKE '%amenity%' AND other_tags LIKE '%hospital%')`

For this SQL statement, only the osm_id,name, and other_tags columns will be displayed in the returned rows. It will select all rows from the points table that have both 'amenity' and 'hospital' in the 'other_tags' column.

Check out this [CartoDB tutorial](http://academy.cartodb.com/courses/04-sql-postgis/lesson-1.html) to learn more about writing SQL. 
