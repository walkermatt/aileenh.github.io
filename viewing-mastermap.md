---
layout: default
title: Viewing Loaded MasterMap Data
---

# Viewing Loaded MasterMap Data #
We can view the data in both PostgreSQL and visualise it in QGIS.

## PostgreSQL ##

Launch PostgreSQL from the Portable GIS control panel and connect to the test database.

Expand the osmm_topo schema and click on the tables node you will see the following. (You may need to click on the fresh button if you can't see all the tables.)

![alt text](http://aileenh.github.io/images/image15.JPG "Mastermap tables in PostgreSQL")

If you expand the node for each table you will see all their columns. The also have a spatial index created on each table.

![alt text](http://aileenh.github.io/images/image16.JPG "Mastermap tables in PostgreSQL")

You can also view the data by right clicking on the table and selecting view data.

![alt text](http://aileenh.github.io/images/image17.JPG "view data in postgreSQL")

You will see something like this:

![alt text](http://aileenh.github.io/images/image18.JPG "view data in PostgreSQL")

## QGIS ##

Launch QGIS from PortableGIS.

![alt text](http://aileenh.github.io/images/image20.JPG "QGIS")

Click on the elephant icon (Add PostGIS layer) in the left hand tool bar.

Create a new connection with the following parameters (the password is `pgis`).

![alt text](http://aileenh.github.io/images/image21.JPG "create postgis connection")

Then click on the connect button.

![alt text](http://aileenh.github.io/images/image22.JPG "postgis connection")

Expand the osmm_topo folder and select all the tables listed.

![alt text](http://aileenh.github.io/images/image24.JPG "postgis tables")

Click on the Add Button. 

This will open all the tables in QGIS

![alt text](http://aileenh.github.io/images/image25.JPG "mastermap in QGIS")

If you want to see it like this there are additional steps required.

![alt text](http://aileenh.github.io/images/image26.JPG "mastermap in QGIS")

Full details can be found in the [Ordnancy Survey OS MasterMap Topography Layer SQL & stylesheets repository](https://github.com/OrdnanceSurvey/OSMM-Topography-Layer-stylesheets).

However I have created some simple steps for you. 

* Add the OSMasterMap.ttf font to your system 
* Copy the folder osmmsymbols into the QGIS SVG directory (C:\usbgis\apps\qgis2\apps\qgis\svg)
* Run the script os_stylrs_scripts.sql using PgAdmin

Once you have done that you can use the QGIS Project file supplied (mastermap.qgs). 

## [Loading other datasets](http://aileenh.github.io/loading-other-datasets.html) ##









