#QGIS Tutorial 3: Geo-Referencing in QGIS: Italy
![tricolore](https://upload.wikimedia.org/wikipedia/commons/e/ee/Flag_of_the_Repubblica_Cispadana.svg)
###This tutorial reinforces skills learned in [Programming Historian QGIS Tutorial "Geo-Referencing in QGIS"](http://programminghistorian.org/lessons/georeferencing-qgis)
**Note: this tutorial makes reference to files and steps covered in our previous tutorial on adding vector layers in QGIS.**

1. Open a new project in QGIS. Set the CRS to **"Monte Mario (Rome) / Italy zone 1 (deprecated)"**.
2. Add the necessary Vector Layers to your project, including:
  * Italy national shapefile (adm0)
  * Italy regional borders (adm1)
  * Italy provincial borders (adm2)
  * Italy commune borders (adm3)
3. Change the appearance of these shapefiles as needed (you may want to go back later and change these settings to make geo-referencing simpler).
  * For each of these layers except adm0, you may want to add labels. Remember, you select and unselect them by checking the box next to their name in your layers panel. This may make geo-referencing easier as you look for specific points.
4. Download *"Kitchen1784"* TIFF file from my Github repository (wmlandis), Geo-referencing Italy
5. Use the georeferencer to add the TIFF file as a raster layer and add 6 or more control points
  * Be mindful of the historical context of the map. "Italy" was not a unified country in 1784, so manmade borders are not good points to use for geo-referencing.
  * Use large cities or other precise locations: the locations of cities are least likely to change.
  * Remember, coastlines are also subject to change.
  * Make sure your 6 points are spread out over the entire map area
6. Remember to specify your transformation settings and then click the georeferencer.
7. Compare your geo-referenced map to the shapefile. You can make this easier by thickening the borders or changing their color in their properties (right-click on them in your layers panel and select properties). You should expect to see some minor discrepancies between your shapefile and the map from 1784. Map-making is an imperfect art, and coastlines and borders change over time.

##Date Sources for this tutorial:
1. Basemap data: DIVA-GIS.org
2. Historic maps: John Carter Brown Library, Brown University: http://jcb.lunaimaging.com/luna/servlet/JCBMAPS~1~1
