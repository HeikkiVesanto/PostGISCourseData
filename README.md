# postgis_course_data
PostGIS Course Data

https://web.archive.org/web/20170913113658/http://workshops.boundlessgeo.com/postgis-intro/welcome.html

The data is not exactly the same as described in the course, but it is pretty close.

The queries should mainly run as is shown in the docs, but the results may differ a little.

Ogr2ogr loading commands:

ogr2ogr -f "PostgreSQL" PG:"host=localhost user=postgres dbname=postgres password=postgres port=5432" -progress nyc_postgis_data.gpkg nyc_census_blocks

ogr2ogr -f "PostgreSQL" PG:"host=localhost user=postgres dbname=postgres password=postgres port=5432" -progress nyc_postgis_data.gpkg nyc_census_sociodata

ogr2ogr -f "PostgreSQL" PG:"host=localhost user=postgres dbname=postgres password=postgres port=5432" -progress nyc_postgis_data.gpkg nyc_neighborhoods

ogr2ogr -f "PostgreSQL" PG:"host=localhost user=postgres dbname=postgres password=postgres port=5432" -progress nyc_postgis_data.gpkg nyc_streets

ogr2ogr -f "PostgreSQL" PG:"host=localhost user=postgres dbname=postgres password=postgres port=5432" -progress nyc_postgis_data.gpkg nyc_subway_stations
