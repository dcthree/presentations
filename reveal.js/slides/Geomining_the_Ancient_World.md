## Geomining the Ancient World
#### Ryan Baumann
#### Duke Collaboratory for Classics Computing

---

![Excavator](../assets/Geomining_the_Ancient_World/excavator.jpg) ![Bill & Ted](../assets/Geomining_the_Ancient_World/bill_ted.jpg)


# Data Mining Geospatial Data About the Ancient World

---

# What is Geospatial Data?


<!-- .slide: data-background="../assets/Geomining_the_Ancient_World/eiffel_paris.jpg" -->


<!-- .slide: data-background="../assets/Geomining_the_Ancient_World/botticelli_paris.jpg" -->


<!-- .slide: data-background="../assets/Geomining_the_Ancient_World/ky_paris.jpg" -->


<!-- .slide: data-background="../assets/Geomining_the_Ancient_World/osm_paris.jpg" -->


<!-- .slide: data-background="../assets/Geomining_the_Ancient_World/aral.jpg" -->


<!-- .slide: data-background="../assets/Geomining_the_Ancient_World/aralkum.jpg" -->


![1989 vs. 2014](../assets/Geomining_the_Ancient_World/AralSea1989_2014.jpg)

---

What does geospatial data look like?
![Paris GeoJSON](../assets/Geomining_the_Ancient_World/paris_geojson.jpg) <!-- .element: class="fragment" -->


<!-- .slide: data-background-video-loop="true" data-background-video="../assets/Geomining_the_Ancient_World/d3broke.mp4" -->
`#d3brokeandmadeart`

---

## What can we do by data mining geospatial data?
* Statistics <!-- .element: class="fragment" -->
* Visualization <!-- .element: class="fragment" -->
* Analysis / Search / Discovery <!-- .element: class="fragment" -->


Roman Amphitheater Elevation
![Amphitheater Elevation](../assets/Geomining_the_Ancient_World/amphi_elevation.png)<!-- .element: style="background: white; width: 768px;" -->
<http://rpubs.com/sfsheath/amphitheater-histograms>


Roman Amphitheater Density
![Amphitheater Density](../assets/Geomining_the_Ancient_World/amphi_density.png)<!-- .element: style="background: white; width: 768px;" -->
<https://twitter.com/sebhth/status/576461235115413504>


Roman Amphitheaters vs. Roman Empire
![Amphitheaters vs. Empire](../assets/Geomining_the_Ancient_World/amphitheater_agree.png)<!-- .element: style="background: white; width: 768px;" -->
<https://twitter.com/sebhth/status/565726866288693251>

---

# Spatial Relationships
* Distance<!-- .element: class="fragment" data-fragment-index="1" -->
* Equals<!-- .element: class="fragment" data-fragment-index="2" -->
* Contains<!-- .element: class="fragment" data-fragment-index="2" -->
* Touches<!-- .element: class="fragment" data-fragment-index="2" -->
* Within<!-- .element: class="fragment" data-fragment-index="2" -->
* Overlaps<!-- .element: class="fragment" data-fragment-index="2" -->
* Crosses<!-- .element: class="fragment" data-fragment-index="2" -->
* Intersects<!-- .element: class="fragment" data-fragment-index="2" -->
* Disjoint<!-- .element: class="fragment" data-fragment-index="2" -->


# Distance
    a = sin²(Δφ/2) + cos φ1 ⋅ cos φ2 ⋅ sin²(Δλ/2)
    c = 2 ⋅ atan2( √a, √(1−a) )
    d = R ⋅ c
Where φ is latitude, λ is longitude, R is Earth's radius

(mean radius = 6,371km)


# Spatial Relationships
* Equals - all points equal
* Disjoint - no points in common
* Within, Contains - one geometry is completely within another
* Overlaps - some points in common, but not all
* Intersects - at least one point in common
* Touches - at least one boundary point in common, but no interior points in common
* Crosses - the geometries actually overlap edges, e.g. a line crossing into a polygon

---

# Formats
* GeoJSON - open, .json, .geojson 
* TopoJSON - GeoJSON extension, .json, .topojson 
* Shapefiles - ESRI, .shp, .shx, .dbf 
* Geography Markup Language -  OGC, .gml, .xml 
* Keyhole Markup Language - Google, .kml, .kmz 
* OSM - OpenStreetMap, .osm
* WKT - "well-known text", .wkt, .wkb
* CSV

---

# Tools
* QGIS
* GDAL
* R
* D3
* GRASS GIS
* GeoRefine
* ArcGIS 👎

---

# Resources


<!-- .slide: data-background="../assets/Geomining_the_Ancient_World/pleiades.jpg" -->


![Lutetia - Pleiades](../assets/Geomining_the_Ancient_World/lutetia_pleiades.jpg)


![Lutetia - Pleiades](../assets/Geomining_the_Ancient_World/pleiades_concepts.png)


![Al-Thurayya](../assets/Geomining_the_Ancient_World/althurayya.jpg)
<http://maximromanov.github.io/althurayya/>


![AWMC](../assets/Geomining_the_Ancient_World/awmc.jpg)


# Modern GIS Resources
* GeoNames.org
* Getty Thesaurus of Geographic Names (TGN)
* OpenStreetMap
* [Natural Earth](http://www.naturalearthdata.com/)

---

# Pelagios


![Pelagios GAP](../assets/Geomining_the_Ancient_World/pelagios_book.jpg)


#### Pelagios Datasets
* Pelagios 3 - Early Geospatial Documents
* American Numismatic Society - coins
* Open Context - research data in archaeology
* AIAC Fasti Online - archaeological excavations
* Epigraphic Database Heidelberg - Latin inscriptions
* Papyri.info - places of origin & findspots for papyri
* Flickr Machine Tags - images
* Google Ancient Places - Classical texts from Google Books
* Pleiades Annotations in the Perseus Digital Library
* SPQR - inscriptions
* Omnes Viae - road network of the Tabula Peutingeriana
* Vici.org - places, findspots, buildings
* Digital Atlas of the Roman Empire


# Recogito
![Recogito](../assets/Geomining_the_Ancient_World/recogito_text.png)


![Recogito Georesolution](../assets/Geomining_the_Ancient_World/recogito_resolution.jpg)


![Recogito Odyssey](../assets/Geomining_the_Ancient_World/recogito_odyssey.jpg)

---

# Examples


Pleiades+

![Pleiades+](../assets/Geomining_the_Ancient_World/pleiades_plus.jpg)

<http://pleiades-plus-gazcomp.appspot.com/>


Itinerarium

![Itinerarium](../assets/Geomining_the_Ancient_World/itinerarium.jpg)

<http://ryanfb.github.io/itinerarium/>


[Distribution of texts/collections in Trismegistos](http://bl.ocks.org/ryanfb/4ef9795dcfc8063a2e99)
<iframe data-src="http://bl.ocks.org/ryanfb/raw/4ef9795dcfc8063a2e99/" width="1024" height="768"></iframe>

---

# The End

<http://dcthree.github.io/presentations/>
