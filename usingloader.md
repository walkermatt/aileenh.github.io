--- 
layout: default
title: Using Loader
--- 

# Loading OS MasterMap into PostGIS Using Loader #
This workshop is a simple introduction to using Loader to load OS MasterMap Topography Layer and other OS OpenData(TM) datasets into PostGIS.

# What is Loader? #

A GML and KML loader written in Python that makes use of OGR 1.9. Source data can be in GML or KML format (including compressed files in GZ or ZIP format) and can be output to any of the formats supported by OGR. The source data can be prepared using a simple Python to both make it suitable for loading with OGR (useful with complex feature types) or to add value by deriving attributes.

Loader was originally written to load Ordnance Survey OS MasterMap Topographic Layer data in GML/GZ format but has since been extended to load other GML and KML data.

# Useful Links #
[Loader Repository](https://github.com/AstunTechnology/Loader)

[Loader wiki](https://github.com/AstunTechnology/Loader/wiki)

[Loader Configuration Examples](https://github.com/AstunTechnology/Loader/wiki/Configuration-examples)


# Prerequisites #
For this workshop we are going to use the [Portable GIS](http://www.archaeogeek.com/portable-gis.html) for convenience as it has everything we need in one simple install.

Obviously in a production environment you would not use the Portable GIS, in which case see the [Loader Installation Documentation](https://github.com/AstunTechnology/Loader/wiki/Installation) on how ot install Loader.

You can download and install PostgreSQL from [EnterpriseDB](http://www.enterprisedb.com/products-services-training/pgdownload#windows).

Once you have installed PostgreSQL you cna install PostGIS using Stack Builder.

# Data #
For this workshop I have package up a small sample of data to be used which can be downloaded from [here](https://my.pcloud.com/publink/show?code=XZi3VbZ88KyhH4PqaFYGzyY7xRyxh8xn3My).

If you are going to repeat this workshop at home or work I would recommend you download bigger sample data sets for the OS website.

[OS MasterMap, VectorMap Local, AddressBase etc](https://www.ordnancesurvey.co.uk/business-and-government/licensing/sample-data/discover-data.html).

[OS OpenData(TM)](https://www.ordnancesurvey.co.uk/opendatadownload/products.html).

## [Let's get started](http://aileenh.github.io/lets-get-started.html) ##
