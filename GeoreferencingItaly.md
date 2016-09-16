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
  ![screenshot](https://github.com/wmlandis/Georeferencing-Italy/blob/master/Screen%20Shot%201.png)
3. Change the appearance of these shapefiles as needed (you may want to go back later and change these settings to make geo-referencing simpler).
  * For each of these layers except adm0, you may want to add labels. Remember, you can select and unselect them by checking the box next to their name in your layers panel. This may make geo-referencing easier as you look for specific points.
4. Download *"Kitchen1784"* TIFF file from my Github repository (wmlandis), Geo-referencing Italy
 ![kitchen1784](https://github.com/wmlandis/Georeferencing-Italy/blob/master/Kitchen1784.jpg)
5. Use the georeferencer to add the TIFF file as a raster layer and add 6 or more control points
  * Be mindful of the historical context of the map. "Italy" was not a unified country in 1784, so manmade national borders are not good points to use for geo-referencing.
  * Use large cities or other precise locations: the locations of cities are least likely to have changed over time.
  * Remember, coastlines are also subject to change over time.
  * Make sure your 6 points are spread out over the entire map area.
  *In this screenshot, you can see that I have located Rome in both maps and used that as a point:*
![rome](https://github.com/wmlandis/Georeferencing-Italy/blob/master/Screen%20Shot%202.png)
*In this screenshot, you can see where my points were right before I georeferenced the map:*
![b4geo](https://github.com/wmlandis/Georeferencing-Italy/blob/master/Screen%20Shot%203.png)
6. Remember to specify your transformation settings and then click the georeferencer.
7. Compare your geo-referenced map to the shapefile. You can make this easier by thickening the shapefile borders or changing their colors in their properties. You should expect to see some minor discrepancies between your shapefile and the map from 1784. Map-making is an imperfect art, and coastlines and borders change over time. However, yours should not be much worse than mine:
![final](https://github.com/wmlandis/Georeferencing-Italy/blob/master/Screen%20Shot%204.png)

##Date Sources for this tutorial:
1. Basemap data: DIVA-GIS.org
2. Historic maps: John Carter Brown Library, Brown University: http://jcb.lunaimaging.com/luna/servlet/JCBMAPS~1~1
