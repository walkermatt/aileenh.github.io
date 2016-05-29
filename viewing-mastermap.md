---
layout: default
title: Viewing Loaded MasterMap Data
---

# Viewing Loaded MasterMap Data #
We can view the data in both PostgreSQL and visualise it in QGIS.

## PostgreSQL ##

Launch PostgreSQL from PortableGIS and connect to the test database.

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

Create a new connection with the following parameters.

![alt text](http://aileenh.github.io/images/image21.JPG "create postgis connection")

Then click on the connect button.

![alt text](http://aileenh.github.io/images/image22.JPG "postgis connection")

Expand the osmm_topo folder and select all the tables listed.

![alt text](http://aileenh.github.io/images/image24.JPG "postgis tables")

Click on the Add Button. 

This will open all the tables in QGIS

![alt text](http://aileenh.github.io/images/image25.JPG "mastermap in QGIS")

If you want to see it like this

![alt text](http://aileenh.github.io/images/image26.JPG "mastermap in QGIS")

or in the OS MasterMap backdrop style there are additional steps required. Full details can be found in the [Ordnancy Survey OS MasterMap Topography Layer SQL & stylesheets repository](https://github.com/OrdnanceSurvey/OSMM-Topography-Layer-stylesheets).

For this workshop I have included 
* Script to create the necessary tables called os_style_scripts.sql which you can run in PgAdmin 
* QGIS Project file (mastermap.qgs). 

You also need to add the fonts (OSMasterMap.ttf) to your system and the folder osmmsymbols into the QGIS SVG directory (C:\usbgis\apps\qgis2\apps\qgis\svg)

# [Loading Other Datasets](http://aileenh.github.io/loading-other-datasets.html) #









