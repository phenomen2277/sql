### Iraqi provinces: PostgreSQL dump file

This is a PostgreSQL dump file containing all the Iraqi provinces presented as polygons. The polygons are spatial and made using the real latitude & longitude coordinates.

![alt text](http://abulewis.com/images/iraqi_provinces.png "Screendump")


#### Usage Example
Pass the latitude and longitude coordinates to find out to which province they belong. 

```SQL
SELECT province from iraq_provinces where area @> POINT(36.229574, 42.236244)
# The output will be => Ninawa
```