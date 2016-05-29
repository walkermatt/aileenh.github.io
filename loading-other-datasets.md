---
layout: default
title: Load Other Datasets
--- 
# Loading Other Datasets #

Loading othere datasets follows exactly the same method.

## VectorMap District ##

To load VectorMap District you need to specify a suitable prep_cmd to prepare the GML for loading and a corresponding gfs file:

`# Use the basic GML preparation routine
prep_cmd=python prepgml4ogr.py $file_path prep_osgml.prep_vmd

# Use the specific VML gfs file tailored to loading into PostgreSQL
gfs_file=../gfs/vmd_postgres.gfs`

## VectorMap Local to PostgreSQL/PostGIS ##

# Use the basic GML preparation routine
prep_cmd=python prepgml4ogr.py $file_path prep_osgml.prep_vml

# Use the specific VML gfs file tailored to loading into PostgreSQL
gfs_file=../gfs/vml_postgres.gfs

FOr more configuration examples see[(Configuration examples](https://github.com/AstunTechnology/Loader/wiki/Configuration-examples)
