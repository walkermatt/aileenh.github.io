---

layout: default
title: Let's get started
---

# [Overview of Loader] (https://github.com/AstunTechnology/Loader/blob/master/readme.md) #

# Setting up Environment #

## Run Portable GIS ##
Navigate to the drive where you installed the Portable GIS and run the file portablegis.exe
![alt text](http://aileenh.github.io/images/image1.JPG "Portable GIS screen shot")

## Start PostgreSQL ##
Click on the 'Servers Module' tab and click on the start radio button to start the PostgreSQL server. 
![alt text](http://aileenh.github.io/images/image2.JPG "Starting Postgrsql")

You will see the following window appear. Do not dismiss the window, leave it running in the background.
![alt text](http://aileenh.github.io/images/image5.JPG "Starting Postgrsql")

## Run PgAdmin III ##
Click on the 'Desktop Module' and click on the PgAdmin III button. 
![alt text](http://aileenh.github.io/images/image4.JPG "Running PgAdmin")

You will see the following window appear. Do not dismiss the window, leave it running in the background.
![alt text](http://aileenh.github.io/images/image9.JPG "Running PgAdmin")

## Connect to Test Database ##
Double click on the portable gis server to connect to it.
![alt text](http://aileenh.github.io/images/image10.JPG "Connect to test database")

You will notice there are three databases in the Portable GIS server. We are going ot use the test database as it already has the PostGIS extension added to it. 
![alt text](http://aileenh.github.io/images/image11.JPG "Connect to test database")

So double click on the test database to expand it. 
![alt text](http://aileenh.github.io/images/image6.JPG "Connect to test database")
You will notice that postgis is listed in the extension for that database.

## Create schema to load data into ##
Right click on the schemas node and select New Schema...
![alt text](http://aileenh.github.io/images/image7.JPG "create schema")

You may call you schema what ever you want but in this workshop we will call ours osmm_topo.
![alt text](http://aileenh.github.io/images/image8.JPG "create schema")

## Edit loader config file ##
So now we have the database schema to load the data into we need to edit the configuration file for Loader. 

There are 7 configuration items when you need to use loader. 
* `src_dir`
  * The directory containing your source files or an individual file. All supported files in the specified directory and it's descendants will be loaded.
* `out_dir`
  * The directory used to store the translated data if writing to a file based format such as ESRI Shape, MapInfo TAB etc.
* `tmp_dir`
  * The directory used to store temporary working files during loading.
* `ogr_cmd`
  * The ogr2ogr command that will be used to load the data. Here you can specify the destination format and any associated settings (for example database connection details if you are writing to PostGIS).
* `prep_cmd`
  * The command used to prepare the source data so it is suitable for loading with OGR, choose one that is suitable for your source data such as prep_osgml.prep_osmm_topo for OS MasterMap Topo.
* `post_cmd`
 * An optional command to be run once OGR has created it's output. Called once per file, useful for loading SQL dump files etc.
* `gfs_file`
  * OGR .gfs file used to define the feature attributes and geometry type of the features read from the GML again choose a suitable gfs file for your source data such as ../gfs/osmm_topo_postgres.gfs for loading OS MasterMap Topo into PostgreSQL.

Once you have a configuration file set up for a specific data source you can save it and use it again and again.

You will find in the loader repository there are a number of different grf and prep_cmd file for different datasources. The Loader wiki also has a section on [configuration examples](https://github.com/AstunTechnology/Loader/wiki/Configuration-examples).

In this workshop we will detail the configuration setting for loading OS MasterMap topographic layer in a PostgreSQL database.

First we need to create the in_dir, out_dir and temp_dir. These can be any directory on your device e.g. c:\temp\loader\in_dir, c:\temp\loader\out_dir and c:\temp\loader\temp_dir

Now we need to edit the config file. On the Desktop Module tab of the Portable GIS click on the 'Edit Config' button in the Loader Group.

![alt text](http://aileenh.github.io/images/image4.JPG "Edit Loader Config")

THis will fire up 
