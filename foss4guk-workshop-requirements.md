---
layout: workshops
title: FOSS4GUK Workshop Requirements
---

# Making Maps in R #

## Barry Rowlingson Medical School, Lancaster University ##

### Workshop (half day) / Target Audience: R users from beginner level up ###

### Description ###

The R statistical software system now has, alongside its GIS functions, lots of add-on packages for making maps - perhaps too many, with overlapping functionality and varying syntax. This workshop will be in three parts: first, I’ll introduce as many of the mapping packages as I can, then you will have time to play with them, and finally we’ll discuss the pros and cons of them all, to see if a single perfect mapping package could be derived or synthesized from the ones available. The session will cover web mapping as well as static and animated maps produced directly in R.

### Software requirements ###

blurb

# Introduction to GeoServer #

## Ian Turton Astun Technology ##

Workshop (2 hours) / Target Audience: Novices

This workshop will cover how to install a local copy of GeoServer and take you through the steps required to produce your first web map. We will take a selection of Ordnance Survey OpenData (tm) and the provided SLD styles and produce a pretty map that you can use as a base map at home.

# Turning data into information using Open Source tools #

Tim Martin Ordnance Survey / Ed Watts Ordnance Survey

Workshop (half day) / Target Audience: Beginners/Intermediate some knowledge of HTML/Javascript would be useful

This workshop will walk through how to turn data about GP surgeries from Health and Social Care Information Centre (HSCIC) into information. Attendees will use a range of desktop and web open source technologies to create a “Find My Nearest GP Surgery”.

Step 1: Attendees will learn how they could use NodeJS to geocode the original data <BR>
Step 2: Use QGIS to visualise the data on a map by creating a choropleth map <BR>
Step 3: Upload the data to CartoDB and create a visualisation that can be shared. <BR>
Step 4: Use Leaflet to visualise the data from CartoDB <BR>
Step 5: Using a variety of Leaflet plugins to improve performance and usability of the map <BR>
Step 6: Add a gazetteer search using Twitter’s Typeahead search library <BR>
Step 7: Include geoprocessing functions from the TurfJS library to allow users to find their nearest surgery. <BR>
Step 8: Add C3 charting library to display statistics of the data.

# Loading OS MasterMap, OS OpenData and other OS GML datasets using Loader #

Aileen Heal Astun Technology / Matt Walker Astun Technology

Workshop (2 hours) / Target Audience: People interested in loading OS datasets into PostgreSQL.

A workshop going through how to use loader to load OS MasterMap, OS OpenData and other OS GML datasets into PostgreSQL/PostGIS. The workshop will use the portable GIS.

# qgis2web: webmaps without code #

Tom Chadwin Northumberland National Park

Workshop (2 hours) / Target Audience: QGIS users

Learn to make webmaps from your QGIS projects without ever touching any code, and without any server-side software. Learn how to style vector data, and even create 2.5d webmaps.

# Using to pgRouting to determine service location and allocate resources #

Ross McDonald Angus Council

Tim Martin / Ian Bennett Ordnance Survey

Workshop (2 hours) / Target Audience: Beginner to intermediate QGIS and PostGIS users

An introductory workshop to using pgRouting, the routing extension to PostgreSQL. The participants with be lead through the basics of installing PostGIS and pgRouting in a PostgreSQL database and optimising the PostgreSQL database for spatial data. They will load Ordnance Survey road network data (either OS Open Roads or the yet-to-be-released OS Highways layer) and build a network topology using pgRouting tools. An introduction to the basics of routing across the network will follow using both the QGIS pgRouting Layer plugin and SQL in PgAdmin. We will then use some real world service or facility locations together with pgRouting functions (shortest path, driving distance and alphashapes) to determine optimal location of new services. The workshop material will be made available before hand as a virtual machine image (or run off the OSGeo LIVE image?) so that everyone has the same user experience with minimised configuration required. Network and service location data will be provided. Notes will be published in a follow along / copy and paste format and will be available online, installed locally and as hard copy.

# Visualising Arts and Humanities Data in QGIS #

Tom Armitage EDINA, University of Edinburgh / Ross McDonald Angus Council

Workshop (2 hours) / Target Audience: Beginner to intermediate QGIS users, but also of interest to experts with little experience of the plugins used.

A QGIS workshop to introduce users to a range of data visualisation plugins. A geoparsed biography will be the core dataset which will be manipulated in a range of ways to produce interesting views of the data.

Plugins used: Heatmap, OpenLayers, MMQGIS, QGIS2ThreeJS, TimeManager

The workshop will take the participants through the process of creating point data from a csv file; overlaying it on a Stamen OSM basemap; visualising it as a heatmap; spatially joining it to polygonal demographic data; create a hexagonal grid to sample the data; create 3D skyscraper diagram from the joined datasets; and finally, use the TimeManager plugin to view how the point distribution varies over time.

The final outputs will be a 3D model and viewer as a webpage created in QGIS2ThreeJS and an animated heat map as an mp4 movie made using TimeManager.

Printed handouts with instructions can be provided; the data used can be downloaded from ShareGeo ahead of the workshop.

# Don’t be afraid to commit #

Jo Cook Astun Technology

Workshop (2 hours) / Target Audience: Beginners

This workshop will aim to help beginners with the technologies and workflows they need to get started with committing to open source projects, with a focus on documentation and GitHub

# The need for National level strategy for Open Principles in Geospatial #

Suchith Anand University of Nottingham

Workshop (2 hours) / Target Audience: Representatives from central government, local authorities, academics, industry, SMEs , NGOs etc in the UK

Open principles are now implemented by the UK Government and delivering huge cost savings for government. Open source GIS software will help the local authorities and various government departments in reducing huge licence fee costs for proprietary software and the UK Government and taxpayers as a whole will benefit from cost efficiencies, reduce the cost of lock-in to suppliers and products. This is especially important for future IT investments (for example Cloud Computing) , so that more options are explored and choices available.

So it important that we have OSGeo UK chapter take this role to bring together nationally. This half day session is aimed at bringing together OSGeo UK Chapter and representatives from central government, local authorities, academics, industry, SMEs, NGOs etc in the UK and put forward and support National level strategy for Open Principles in Geospatial in the UK.

# GeoFire — Realtime location queries with Firebase #

## Sebastian Ovide Ordnance Survey (Geovation) ##

### Workshop (2 hours) / Target Audience: Developers with appreciation of JS. ###

We’ll write a serverless web app using Firebase as backend and GeoFire to store and retrieve data within a given geographic area. Even if it could be done using PostGIS, using Firebase will allow us to write an app that can scale painlessly without any development work involved

# SaaSy maps - Using django-tenants and geodjango to provide webGIS Software-as-a-Service (SaaS) #

Anusha Chickermane Atlantic Geomatics Ltd.

Workshop (half day) / Target Audience: People with a limited understanding of how django and openlayers work.

Aim: The aim of this workshop is to demonstrate how to create a semi-isolated multi-tenant architecture using django-tenants+postgresql, and then build on top of it using geodjango+postgis+openlayers to provide individualised web mapping services to different clients. It will also take a brief look at the performance and security implications of this approach.

Requirements: Windows/Linux/Mac laptop with administrative permissions, internet connection, Postgres 9.4, PostGIS 2.2, Python 3.5, Django 1.8 and GeoDjango prerequisites (https://docs.djangoproject.com/en/1.9/ref/contrib/gis/install/).

Description: In this workshop, participants will build a multi-tenant web application displaying road accident data for different counties, with a different url and dataset for each county. The workshop will start with a brief presentation on django, django-tenants and geodjango, and the pros/cons of this approach. We will then proceed to the coding section of the workshop where all participants will code a multi-tenant django website, load it with OS and road-accident data-sets, and view the different county websites.

Materials Provided: Paper and electronic copies of detailed handouts to be used during the lecture portions of the workshop and github link containing the code used in the workshop.

Presenter Bio: I am a Senior Software Developer for Atlantic Geomatics, a surveying company where I design and develop GIS mapping solutions using Python, Django, PostgreSQL, PostGIS and AngularJS as Scrummaster of a team of 3. I have 4 years of experience working on successful projects using Java, Javascript and Python. I have a MSc. in Cybersecurity and a MSc. in Computer Science, and a professional membership with the British Computing Society.


# Getting started with Openlayers #

Thomas Gratier WebGeoDataVore

Workshop (half day) / Target Audience: Beginners looking for introduction to OpenLayers. They should be able to use a text editor, a browser and knowing basic use of command line.

This workshop will introduce by the example how to begin with OpenLayers 3. It will go through how to create you first map, use various available layers, manage interactions on the map and use vector data with the styles. Along, you will learn where and how to use Openlayers resources when you need to go further.
