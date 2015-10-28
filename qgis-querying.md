#Querying using QGIS

You can Select by Expression by opening the attribute of a desired layer and clicking on the 'Select by Expression' button.

![sel_by_expression](https://cloud.githubusercontent.com/assets/2665840/10792048/00b59680-7d83-11e5-8140-2a08831e69ff.png)

You can then enter an expression. The example shown above queries all rows that have the string 'hospital' found in the 'other_tags' column.


`SELECT *
FROM points
WHERE other_tags LIKE '%amenity%' AND other_tags LIKE '%hospitals%'`