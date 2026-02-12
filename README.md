# GmE221 - Laboratory Exercise 1

## Overview
This Laboratory sets up a spatial analysis environment using Python and PostGIS and performs a percel-landuse overlay analysis.

##Environment Setup
-Python 3.14.3
-PostgeSQL with PostGIS
-GeoPandas, SQLAlchemy, psycopg2

## How to Run
1. Activate the virtual environment'
2. Run 'main.py' to test the database connection
3. Run 'overrlay.py' to compute landuse percentages

## Outputs
-PostGIS table:'parcel_landuse_percentage'
-Visualization in QGIS

## Description of Database Connection
A successful database connection means that it can make a web network through a language which is this case, Python, from another databe to another. In one perspective, PostGIS is an independent spatial database with  its our query tools where it can type queries based on objectives or study. However, linking this database to another software, is another way that broaden the perspective. Using Visual Studio Code, setting the environment, enabling the packages, and able to manipulate linkages or networks of the PostGIS and enable to load and see the data through queries. Hence, through python language, it allows you to make spatial computation even if you do not open the pgAdmin. Then, this is a perfect sign to call the connection of python and PostGIS successful.

## Reflection Part D
While working on the script for the calculation of quantities, vector analysis tools, and creation of new table, there was an error on the identity of parcel. I've tried to "fix" it by focusing on 1 line and find the cause but unfortunately, failed many times. And as usual, just retyping the whole script works for me. It made me more cautious on the spatial identity, queries, and the whole structure of how the script is written. At the same time, it enhanced my knowledge to get used to the format. Inspecting the code, there are similarities in constructing queries for PgAdmin but it is necessary to call out postgis extension and medium of view output. 

## Reflection Part F
There is a significant relationship between parcel shapes and land use. The script calculates the land use type for each parcel and categorizes them by the percentage of area they cover. A wide range of values is expected, as this reflects the extent of a specific land use within a single parcel. For example, the Residential zone (Low Density) in lot 193-01-0016-009-30 covers only about 0.0000452 of the total 171.01 lot area; therefore, the land use percentage is effectively zero. In contrast, most areas covered by only a single land use (100%) are classified as Commercial Industrial Zones.

Interpretation depends on the geometry's structure and quality, as well as the choice of CRS and scale, because these factors determine the accuracy of the quantitative data. The CRS defines the units of measurement: WGS 84 uses degrees, while UTM Zones use metric units, which allow for the calculation of distance, length, and area. Therefore, metric systems are more flexible for manipulation and analysis. Geometry quality is also critical, as the geometry itself is the subject of the study; corrupted geometry will lead to errors in computed percentages, making manual validation necessary. Finally, scale allows for validation by zooming in and out. It also influences how spatial results are visualized, making them easier to understand. A good visualization should represent all features distinctly—even minor groups or small areas—without requiring the user to zoom in or open the attribute table.