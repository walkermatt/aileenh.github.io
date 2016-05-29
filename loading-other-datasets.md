---
layout: default
title: Load Other Datasets
--- 
# Loading Other Datasets #

Loading othere datasets follows exactly the same method.

## VectorMap District ##

To load VectorMap District you need to specify a suitable prep_cmd to prepare the GML for loading and a corresponding gfs file:

Use the basic GML preparation routine
prep_cmd=python prepgml4ogr.py $file_path prep_osgml.prep_vmd

Use the specific VML gfs file tailored to loading into PostgreSQL
gfs_file=../gfs/vmd_postgres.gfs

Remember to create a suitable schema in the database (e.g. vmd) and edit the ogr_cmd to load into that schema e.g. active_scheam=vmd

If you are using the same src_dir remember to remove the mastermap data from the folder and copy the new data into the folder.

There is a small sample of VectorMap District data in the sample data supplied.

For more configuration examples see[(Configuration examples](https://github.com/AstunTechnology/Loader/wiki/Configuration-examples)
