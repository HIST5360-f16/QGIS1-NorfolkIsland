# Norfolk Island in QGIS: Adding Vectors and Layers
[forked on Thursday, September 15, 2016]
### Author: sebastian.fuentes@mavs.uta.edu
![Flag of Norfolk](/Flag_of_Norfolk_Island.svg.png)
### This tutorial is designed so you can practice the skills you used in the [Programming Historian QGIS Tutorial about adding layers](http://programminghistorian.org/lessons/qgis-layers "Links to Programming Historian")
1.	Make a folder or directory called *Norfolk Island* on your computer.
2.	Download the following Norfolk Island data sets from DIVA-GIS [Google it] into that directory and unzip them; each should be in its own sub-directory.  When using the "Download data by country", remember you have to search for the Country using the drop down menu and Subject material you wanting to download.  For this activity, you have perform this step twice in order to collect the 'adm.' and 'rds.' Zip Files.  Use the Subject drop down menu and select "Administrative areas" and "Roads" before clicking "OK".
    -	Administrative Areas NFK_adm.ZIP
    -	Roads NFK_rds.ZIP
3. 	Open QGIS and set up up a new project.
4.	Set up CRS (Coordinate Reference System) so that the project is using the NAD83(CSR98) /Prince Edward Isl.... EPSG:2291 Geographic Coordinate system.

![Flag of Norfolk](/Screenshot1_Selecting CRS.PNG)

![Placeholder image](/Norfolk-Island-Pines.jpg)

5.	Build a base map: Open these vectors, then change the way they look using the *properties*
    - NFK_adm0.shp; change so there is no color fill. Remember *fill style* = *no brush*
    - NFK_roads.shp; change the color and width of the lines so they are easier to see

![Before Edits from Step 5](/Before Edits.PNG)

![After Edits from Step 5](/After Edits.PNG)

6.	There is not an attribute table nor file titled NFK_adm1.shp. If there were, the file might show the country's 10 parishes for example. Instead, right click on the NFK_adm0.shp file, select Properties, and navigate to Labels.  Use the screen shot provided to label the island using "Name_ENGLI" and change the font size and color as needed. Change so that your map shows the name of the island in a large font.

![Screenshot2_Labeling - Step 6](/Screenshot2_Labeling.PNG)

7.	Perform a google search and look for a "Norfolk Island tif file".  Your search should take you to the National Library of Australia.  Download the tif file titled: "Map and chart of Norfolk Island from actual survey, 1840 / John Arrowsmith".

![Screenshot3_tifFile- Step 7](/Screenshot3_tifFile.PNG)

Unzip it and import the .tif file into QGIS as a raster file. Note that the image is angled different in QGIS.

8.	Go back to NFK_adm0.shp and change the width of the lines so they are visible.
9.	In the left-hand *layers* panel, drag the nla.obj-231888760 layer so you can see the historical map below the NFK_adm0.shp lines.

Note: You might need to use the Geo-referencing tool to Geo-reference the tif file.  See the below screen shot.

![Screenshot4_Georeferencing Raster File- Step 7](/Screenshot4_Georeferencing Raster File.PNG)

*** We could use another screenshot here***

![Final Product](/Final Product.png)

*How to add a map that is not available in TIF*
10. If you want to add another map of Norfolk Island that you find, you need to know how to convert it to a TIF file in order to georeference it. Download [Irfanview](http://www.irfanview.com/)

![Irfanview](/Irfanview Screenshot.png)

11. Find a map on google that you like, or use [Norfolk Island](https://www.google.com/search?q=norfolk+island+map&biw=1920&bih=910&tbm=isch&tbo=u&source=univ&sa=X&sqi=2&ved=0ahUKEwictaCsy7XPAhXJVh4KHRC0AHUQsAQIKg#imgrc=uNrWNc_GWuP6yM%3A)
12. Open your Irfanviewer, and select the *Batch Convert* option under *File*. Add your map to the batch, and convert to TIF.
13. Select the *Georeferencer* option under the *Raster* button on the toolbar. Select your map after choosing the "add raster" button.
14. Select several points on the map that can be easily found on the shapefile (I often choose hydrology), and make sure your settings add the georeferenced map to QGIS.
15. After you have finished, you should see your map superimposed over the shapefile in QGIS. Click on the map file, and adjust the transparency so that you can easily see the information on the shapefile and the map at the same time.
16. Congratulations! You have successfully taken a JPEG file map, converted it to TIF, and added it to your work.

![Georeferenced Norfolk Island from JPEG](/Norfolk Island Georeference.png)

17.	Save your work. Close QGIS

# Data Sources for this Tutorial
## Country GIS base map data
[DIVA GIS](http://www.diva-gis.org/gdata)

## Historical maps
The map "Map and chart of Norfolk Island from actual survey, 1840 / John Arrowsmith" can be downloaded at [Arrowsmith](http://nla.gov.au/nla.obj-231888760/view)

Other sites that are likely to have similar maps are:
* [David Rumsey](http://DavidRumsey.com)
* [The John Carter Brown Library Map Collection](https://www.brown.edu/academics/libraries/john-carter-brown/jcb-online/image-collections/map-collection)
