# Exercise 2: Adding Vector Data
In this exercise you will learn how to add vector files to your map and adjust the properties, display symbology, and labels.

## Section 1: Key Terms
- **Vector data**
  - Vector data represents features in the world using **points**, the relationships between those points (**lines**), and relationships closing an area (**polygons**).
- **Shapefile**
  - A shapefile is a storage format for vector data.
  - It can store features as points, lines, and polygons together with data tables that describe the attributes of the features.
  - A single shapefile actually consists of a collection of files with the same filename but different extensions. The files must be stored in the same folder.

## Section 2: Start QGIS and Add Vector Data
You will add a layer, consisting of vector polygon feature.

1. Start QGIS Desktop.
  ![][desktopicon]
2. In the menu click _Layer_ > _Add Layer_ > _Add Vector Layer…_.
  ![][addvectorlayer]
3. The _Add vector layer_ box will open. Select the _Source type_ as _File_ and _Encoding_ as _System_.
4. Click Browse. The _Open an OGR Supported Vector Layer_ box should open.
  **Note:** The box should open to the last place from which you added data in QGIS.
5. Navigate to the training folder then the _05_Data/03_Shapefiles/00_Philippine/Admin_.
6. You will see a lot of files with the same filenames but different file extensions. Remember what we said about a single shapefile consisting of a collection of files. You want to open the main file with type _SHP File_.
  ![][shapefilefiles]  
7. To filter the view, change _All files (*)_ to _ESRI Shapefiles (*.shp *.SHP)_. Click on the file named _PHL_admin2.shp_.
  ![][filterfileview]
8. Click _Open_ in the _Open an OGR Supported Vector Layer_ box.
9. Click _Open_ in the _Add vector layer_ box.
10. There are three ways to open the _Add vector layer_ box in QGIS Desktop.
  - Using the menu _Layer_ > _Add Layer_ > _Add Vector Layer…_.
  - Using the _Add Vector Layer_ icon in the _Manage Layers_ toolbar. If you don't see the _Manage Layers_ toolbar you might need to add it to your QGIS layout. In the menu click _View_ > _Toolbars_ and check the desired toolbar.  
  - Using the keyboard shortcut _Ctrl + Shift + V_.
  **Note:** In all of these methods the same _Add vector layer_ box will open and the procedure for selecting which data you will add is the same as described above.
11. Add these other vector layers:
  - _05_Data/03_Shapefiles/02_Disaster/HaiyanPath_03-11Nov/HaiyanPath_03-11Nov.shp_
  - _05_Data/03_Shapefiles/02_Disaster/HaiyanPath_03-11Nov/haiyanPath_03-11Nov_line.shp_

Note: Your map should look similar to this:


## Section 3: Change a Layer Name
When a layer is added, QGIS assigns it a layer name. Sometimes this name is not very descriptive because it inherits the shapefile name. You can rename the layer at any time. Now, you will change the names of the layers that you added.
1. In the Layer Panel, right click (on the text) for the VNM_adm1 layer

2. Click Properties to display the Layer Properties dialog (or, Properties, when you right click on layer being modified)
3. Click the General symbol   tab near the top of the dialog box
You should see the following dialog

4. For Display Name type “Regions”
5. Click OK
6. Repeat the previous steps to rename the VNM_populatedPlaces_ne10m layer to Cities
Note: Your Layer Panel should look similar to this


## Section 4: Symbolize Spatial Data
The Regions layer appears in a single color by default. You may want to display the Regions in different colors.
1. In the Layer Panel, double-click the Regions layer to open its Properties dialog.
2. Click the Style tab.
Note: In previous versions of QGIS it was called Symbology.
3. Make sure the button near the top right of your screen says Old Symbology.

Note: If your screen looks like the image below, then click on the New Symbology button. Clicking on New Symbology will change it to the newer version of QGIS symbology. You will receive a prompt asking if you wish to use the new symbology implementation for this layer. Click Yes.

4. Select Categorized from the drop down menu below the Style tab.

Note: If using a previous version of QGIS, select Unique Value in the drop down menu next to Legend Type.
5. In the new screen that appears within the dialog, select VARNAME_1 for the Column.
Note: If using a previous version of QGIS, Column is called Classification Field.
6. Click on the Color Ramp drop down menu.

7. Select New Color Ramp…
8. Select ColorBrewer for the Color ramp type and click OK.

9. Select the Spectral Scheme name.
10. Select 10 for the number of colors.
11. Click OK.
12. Call the new color ramp “Spectral” and click OK.
13. Click Classify.

14. All the Regions will appear in the window with an assigned color.
15. Double click on the first Region symbol in the list.
16. In the Symbol Selector window that appears, you will be able to change the color for the highlighted region by clicking the Change button in the middle of the window.
Note: If using a previous version of QGIS, click on the first Region name in the list. In the right side of the dialogue window, you will be able to change the color for the highlighted Region. Click on the colored box in the Fill Options area.

17. Select new color.
18. Click OK to close the color selection.
19. Click OK to close the Layer Properties dialog.
Next, you will change the symbol for the Cities.
20. Double-click the Cities layer in the Layer Panel to open its Layer Properties dialog.
21. Click the Style tab.
22. Click the Change button in the middle of the window.


Note: If you are using a previous version of QGIS, you will change the symbol scroll down (using the scroll on the far right of the dialog) until you see Fill options.
23. Click on the black box under the Basic Colors options.

24. Click OK to close the color selection.
25. Click OK to close the Layer Properties dialog.

## Section 5: Label Features
A map is incomplete without some labeled features. Placing names on your map is an important communication task. Map readers should be able to find names quickly or they will not use your map. Now, you will place the names of the Cities on the map.
1. Select the Cities  layer in the Layers box by clicking on it once so it is highlighted blue
2. Click the Layer menu>Labeling to open the Layer Labeling Settings dialog

3. Check the Label This Layer box
4. Select NAME from the field with labels drop-down menu located at the top
5. Click the button with three dots in the Text Style section of the Label Settings tab

6. Select MS, Serif, Bold, 10 (size) from the Select Font window
7. Click OK
8. Click Color and select black
9. Click OK to close the color selection
10. Click OK to close the Layer Labeling Settings dialog


Note: Your map should look something like this. The colors will be different.


## Section 6: Save Your Map Document
You will save your map document for future use. You can save your file with absolute or relative paths. This refers to how the QGIS file will remember where the data corresponding to each layer is located. Absolute path means that QGIS will always look in the same file location (exact location on the computer for the data) while relative path means that QGIS will look for the data to be in the same place in relation to the QGIS file (such as in the same folder or 2 folders away in a folder called 02_Data). Relative paths are in general better if you might move your folders and or share your *.qgs files with a colleague.
1. Click Settings>Project Properties

2. Open the General tab
3. Change Save Paths to Relative under General Settings

4. Click OK to close the dialog
5. Click File>Save Project as…
6. Save the file in \\Vietnam_Training\06_Participant_Work
7. Name the file “Adding_Vector_Data”
8. For Save As Type, confirm QGIS Project File (\*.qgs)

9. Click Save
Optional Steps:
1. Add the road layer to the map
2. Change the road color to a different color
3. Change the road line width



[desktopicon]: https://raw.githubusercontent.com/AmericanRedCross/QGIS_Training/master/img_v2.8/exercise2_01_  .png
[addvectorlayer]: https://raw.githubusercontent.com/AmericanRedCross/QGIS_Training/master/img_v2.8/exercise2_02_
[shapefilefiles]: https://raw.githubusercontent.com/AmericanRedCross/QGIS_Training/master/img_v2.8/exercise2_03_
[filterfileview]: https://raw.githubusercontent.com/AmericanRedCross/QGIS_Training/master/img_v2.8/exercise2_04_
