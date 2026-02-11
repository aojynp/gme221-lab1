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

## Reflection
While working on the script for the calculation of quantities, vector analysis tools, and creation of new table, there was an error on the identity of parcel. I've tried to "fix" it by focusing on 1 line and find the cause but unfortunately, failed many times. And as usual, just retyping the whole script works for me. It made me more cautious on the spatial identity, queries, and the whole structure of how the script is written. At the same time, it enhanced my knowledge to get used to the format. Inspecting the code, there are similarities in constructing queries for PgAdmin but it is necessary to call out postgis extension and medium of view output. 