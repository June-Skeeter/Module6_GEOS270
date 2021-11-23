---
layout: default
title: Geocoding and Web Mapping
parent: Application
nav_order: 2
---

# Geocoding and Web Mapping
{: .no_toc }

<details open markdown="block">
  <summary>
    Table of contents
  </summary>
  {: .text-delta }
1. TOC
{:toc}
</details>

# Geocoding

The process of attributing coordinates (Latitude/Longitude) to descriptive locations (Street Address).  We can use a variety of web based services (google maps, ESRI, mapbox, open street map, etc.) to perform geocoding.  We're using Mapbox today because it strikes a good balance between accessibiliyt and accuracy.  


## Google Maps

* Arguably the best geocoding service, but it costs money :/ [5.00 USD per 1000 request](https://developers.google.com/maps/documentation/geocoding/overview).

## ArcGIS World Geocoder

* You can geocode right in [ArcGIS Pro](https://pro.arcgis.com/en/pro-app/latest/help/data/geocoding/tutorial-geocode-a-table-of-addresses.htm).  Feel free to give it a shot on your own time if you want.  The reason we are **not** using it today: ESRI geodocing services uses a [credit](https://www.esri.com/en-us/arcgis/products/credits/overview?rsource=%2Fsoftware%2Farcgis%2Farcgisonline%2Fcredits) based system for geocidng.  As a student, you get 1,000 credits, which is easy to go through quickly.  You can get more if you request them from Jose, but its inconvenient.

## Open Street Maps

* [Open Street Maps](https://osmnames.org/) is a volunteer based platform that offers free geocoding and webmaps.  But the geocoding is somewhat error prone at times.

## Mapbox

* A "freemium" service up to [100,000 requests per month](https://www.mapbox.com/pricing/#geocode) and gives fairly reliable results.  This is what we are using today.  It requires you to create a free [Mapbox](https://mapbox.com) account.  Once you have an account, you will be given an [access token](https://account.mapbox.com/access-tokens/).  Which lets you use the mapbox service.  

We will be using a Python module called [geopy](https://geopy.readthedocs.io/en/stable/) to interface with Mapbox for us.

# Web Mapping

Web mapping takes cartography beyond static maps.  You can create 


Today, we'll use a Python package called [follium]http://python-visualization.github.io/folium/ which allows us to create dynamic, interactive webmaps that can be embedded in webpages.  Folium will "translate" our python commands into Javascrpt and create [leaflet](https://leafletjs.com/) maps.  Leaflet is a javascript   Follium is already installed, so we don't have any more steps to do here!

# Getting Started with Geocoding

You can close the terminal window, we don't need it anymore.  Go back to your Jupyter Notebook window.
* Double click on "Geocoding and Webmapping.ipynb" to open it.

# Web Mapping

Web mapping takes cartography beyond static maps.  ESRI has a platform aslled [ArcGIS Online](https://www.arcgis.com/index.html).  If you're interested in learning about it, my colleage Maya at the UBC Library Research Commons has created this [workshop](https://ubc-library-rc.github.io/intro-AGOL/).  You can look through this page, or take it live with her next semester!  Today, we'll use a Python package called [follium]http://python-visualization.github.io/folium/ which allows us to create dynamic, interactive webmaps that can be embedded in webpages.  Folium will "translate" our python commands into Javascrpt and create [leaflet](https://leafletjs.com/) maps.
