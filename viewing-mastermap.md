---
layout: default
title: Viewing Loaded MasterMap Data
---

# Viewing Loaded MasterMap Data #
We can view the data in both PostgreSQL and visualise it in QGIS.

## PostgreSQL ##

Launch PostgreSQL from PortableGIS and connect to the test database.

Expand the osmm_topo schema and click on the tables node you will see the following. (you may need to click on the fresh button if you can't see the tables)

![alt text](http://aileenh.github.io/images/image15.JPG "Mastermap tables in PostgreSQL")

If you expand the node for each table you will see all their columns. The also have a spatial index created on each table.

![alt text](http://aileenh.github.io/images/image16.JPG "Mastermap tables in PostgreSQL")

You can also view some of the data by 
