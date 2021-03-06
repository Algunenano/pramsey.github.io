---
layout: post
title: 'NYC Sprint: Day 3'
date: '2010-02-22T14:00:00.000-08:00'
author: Paul Ramsey
tags:
- osgeo
- sprint
modified_time: '2010-03-01T19:14:15.095-08:00'
thumbnail: http://farm3.static.flickr.com/2804/4380402910_b0f07b624b_t.jpg
blogger_id: tag:blogger.com,1999:blog-14903426.post-1991992435132133204
blogger_orig_url: http://blog.cleverelephant.ca/2010/02/nyc-sprint-day-3.html
comments: True
---

Third day, best day. There are four MapServer developers now working hard on implementing the [rendering plugin](http://trac.osgeo.org/mapserver/wiki/RenderingPluginStatus) changes. Thomas Bonfort is doing the core work, Steve Lime is re-working the old GD renderer, Dan Morissette is creating support for hatched styles, and Assefa is doing KML output.

In Geoserver land, Andrea Aime added support for [variable substitution in SLD](http://old.nabble.com/Variable-substitution-in-SLD-ts27689445.html), which means that URL parameters can now be passed into SLD styling rules, to create dynamic styling effects. Tim Schaub and Justin Deoliveira also demonstrated an application that warms the cockles of my heart:  using their new GeoScript extension they made a web-based application that takes in SQL and spits out maps. So now I can type PostGIS queries into a web page and see the results overlaid on a map. Crunchy!

<img src="http://farm3.static.flickr.com/2804/4380402910_b0f07b624b_m.jpg" width="180" height="240" alt="Geoserver / OpenLayers Crew" />

Howard Butler has contributed some work on the auto-projection support in MapServer and is now working on LibLAS Oracle support. He also tracked down an excellent pastrami sandwich. So I am told.

In PostGIS world, Jeff Adams finished his lat/lon formatter and logged his first commit: an impressive complete collection of unit tests, documentation and a working function (`ST_AsLatLonText`) that can turn POINT(-120.5 12.25) into 12°15'0"N 120°30'0"W. Oliver continues to fix up the text output functions. And I completed my first cut of the WKT output. Curve support really adds a lot of overhead to these things! There are lots of variants and curves have more and sillier formatting rules than linear features. David Zwarg has continued beavering through tickets in the WKTRaster subsystem.

Thanks again to our sponsors, tonight we are heading out to dinner at a Malaysian restaurant in Chinatown.
