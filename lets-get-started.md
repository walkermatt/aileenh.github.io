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

You will see the following window appear. D noo dismiss the window, leave it running in the background.
![alt text](http://aileenh.github.io/images/image5.JPG "Starting Postgrsql")

## Run PgAdmin III ##
Click on the 'Desktop Module' and click on the PgAdmin III button. 
![alt text](http://aileenh.github.io/images/image4.JPG "Running PgAdmin")

You will see the following window appear. D noo dismiss the window, leave it running in the background.
![alt text](http://aileenh.github.io/images/image9.JPG "Running PgAdmin")

## Connect to Test Database ##
Double click on the portable gis server to connect to it.
![alt text](http://aileenh.github.io/images/image10.JPG "Connect to test database")

You will notice there are three databases in the Portable GIS server. We are going ot use the test database as it already has the PostGIS extension added to it. 
![alt text](http://aileenh.github.io/images/image11.JPG "Connect to test database")

So double click on the test database. 
![alt text](http://aileenh.github.io/images/image6.JPG "Connect to test database")
You will notice that postgis is listed in the extension for that database.

## Create schema to load data into ##

![alt text](http://aileenh.github.io/images/image7.JPG "create schema")
![alt text](http://aileenh.github.io/images/image8.JPG "create schema")


## Edit loader config file ##

