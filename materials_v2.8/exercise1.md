# Exercise 1: Exploring QGIS
This exercise will introduce you to QGIS and some of the basic functions of the program. By the end of this exercise you should be able to:  
- Open a current QGIS file
- Set up the layout of your QGIS file
- Zoom, move, and navigate a map
- Turn layers on and off

## Section 1: Start QGIS
1. If you have a shortcut for QGIS on your desktop, double click it to start QGIS. Otherwise, click Start > All Programs > QGIS Wien > QGIS Desktop(2.8.2).  
    **Note:** Make sure that you open Quantum GIS Desktop, not the similarly titled Quantum GIS Browser.  
    ![][desktopicon]

You are now looking at the interface of the QGIS application. Whenever you work in QGIS Desktop, you are working with a map document. This document can contain various layers, which are populated by spatial datasets. A saved QGIS map document has a \*.qgs file extension.

## Section 2: Open a .qgis File
A map document was created for this exercise. You will use this file to examine some of the features of QGIS.  

1. Click Project > Open...  
  ![][open]
2. Navigate to the training folder then the 04_Exercises/Project_files folder and choose to open `Q282-PHL_Exploring_QGIS.qgs`.  
3. When `Q282-PHL_Exploring_QGIS.qgs` opens, you will see an image depicting the region with the location of various countries. It should look similar to the following example.  
  **Note:** Your screen might show this in a different size and with the toolbars in different locations. If you are using a different version of QGIS, you might see a warning about project compatibility.    
  ![][opened]

## Section 3: Setting Up Your QGIS Layout
Your QGIS window may look different depending on your settings. This section will teach you how to adjust your layout settings.

1. Click View > Panels in the menu and toggle the box next to Layers.  
  ![][view-panel-layers]
2. Click View > Panels in the menu and toggle the box next to Overview.  
What does your QGIS window look like now?  
3. Turn the Layers and Overview on by checking the boxes in the View > Panels menu.
4. Right click on the populatedPlaces_region_ne10m layer and check the box next to Show in Overview to add the layer to the Overview Panel.  
  ![][showinoverview]

QGIS allows you to dock panels on the side of your screen so you have easy access to them. Now you will practice docking and undocking the Layer Panel.  
5. Click on the word Layers or on the small grey dots at the top of the Layer Panel and drag the panel to the middle of your screen to undock it.  
  ![][layersbar]
  ![][undock]
6. Re-dock the Layer Panel by clicking on the top of the Layers Panel and dragging the top of the Layers Panel to the top of the Overview Panel. Release your mouse button when you see the Overview Panel move down the screen and the grey dots will appear indicating where the Layers Panel will dock.  
  **Note:** If you want to dock the Layer Panel when there are no other panels open, click on the top of the Layer Panel window and drag it to the left wall of your map area. When the grey dotted outline appears, indicating where the Layers Panel will dock, you may release the mouse button.  
  ![][redock]

## Section 4: Introduction to the Map Navigation Toolbar
The previous section showed you how to adjust your QGIS layout. In this section, you will zoom in and out, move, and navigate the map using the map navigation toolbar.

1. Click View > Toolbars in the menu and check that the box next to Map Navigation is checked.
  ![][toolbarmapnav]
2. Click the Zoom In button on the standard toolbar.  
  **Note:** The toolbar that is currently selected will appear with a different color background on the toolbar. After you select the Zoom In mode the button should turn a darker grey color.  
  ![][zoomin]
  ![][zoominselected]
3. Position the magnifying glass pointed to the upper left of a country of your choice. Click and hold the left mouse button while dragging your mouse to near bottom right of a country of your choice, making a rectangle around the two points.  
  ![][zoomtocountry]
4. Release the mouse. Now you will see a closer view of the country you chose.
5. To return to the previous view click the Zoom Last button. This will take you back to the previous zoom level that shows the entire region.  
  ![][zoomlast]
6. Again, use the Zoom In tool to zoom in on the Philippines. You should now the Philippines in the center of the map.
7. Click the Pan Map button on the standard toolbar.  
  ![][pan]
8. Move the cursor hand to the left side of your map area.
9. Click and hold the left mouse button while moving the map right so that Vietnam is centered on your map.
10. Release the mouse button. You will see that the map has been repositioned. You should now see Vietnam in the center of the map.
11. To return to the whole view of the region, click the Zoom Full button.  
  ![][zoomfull]
12. **Note:** The Zoom Full and the Zoom to Layer button in this example would give us very similar results. However, this will not always be the case. The Zoom to Layer button will redraw the map zooming to whichever layer is highlighted in the Layer Panel.  
  ![][zoomtolayer]

## Section 5: Introduction to the Layer Panel
The previous section showed you how to zoom in and out, move, and navigate your map. In this section you will learn to turn a layer on or off using the Layer Panel.
The Layer Panel in QGIS shows you the layers of data that are available to be shown on your map. Think of layers as pieces of data that can be added one on top of the other and displayed together.
1. In the Layers Panel there are currently 4 items: `populatedPlaces_region_ne10m`, `water_rivers_region_10m`, `water_lakes_region_ne10m`, and `admin0_region_ne10m` layers.
1. In the Layer Panel, uncheck the `populatedPlaces_region_ne10m` check box. The red dots on the map that show cities will disappear.
2. In the Layer Panel, check the `water_rivers_region_10m` check box. Now you will see blue lines on your map that show rivers.
3. In the Layer Panel check the `populatedPlaces_region_ne10m` check box so that the cities are shown again.
4. Click the `populatedPlaces_region_ne10m` name so that it is highlighted in blue.
5. Click and hold the left mouse button while dragging that layer to the bottom of the Layer Panel below the other layers. Release the mouse button.  
  ![][draglayer]
6. Now, the order of the layers from top to bottom is: `water_rivers_region_10m`, `water_lakes_region_ne10m`, `admin0_region_ne10`, `populatedPlaces_region_ne10m`
7. **Note:** The cities are no longer visible on the map. They are displayed below the countries and therefore hidden. When organizing layers in your map, the order changes how the map displays.

## Conclusion
Do you know how to:
  - Turn toolbars on and off?
  - Turn panels on and off?
  - Turn layer on and off?
  - Adjust the order of layers?
  - Undock and dock panels?
  - Zoom in, zoom out, and navigate the map?  
If you can do all these things, good work! You have reached the end of the exercise. You can exist QGIS without saving.

*The information provided in this exercise is not official American Red Cross information and does not necessarily represent the views of the American Red Cross.*

[desktopicon]: https://raw.githubusercontent.com/AmericanRedCross/QGIS_Training/master/img_v2.8/exercise1_01_desktopicon.png
[open]: https://raw.githubusercontent.com/AmericanRedCross/QGIS_Training/master/img_v2.8/exercise1_02_open.png
[opened]: https://raw.githubusercontent.com/AmericanRedCross/QGIS_Training/master/img_v2.8/exercise1_03_opened.png
[view-panel-layers]: https://raw.githubusercontent.com/AmericanRedCross/QGIS_Training/master/img_v2.8/exercise1_04_view-panels-layers.png
[showinoverview]: https://raw.githubusercontent.com/AmericanRedCross/QGIS_Training/master/img_v2.8/exercise1_05_showinoverview.png
[layersbar]: https://raw.githubusercontent.com/AmericanRedCross/QGIS_Training/master/img_v2.8/exercise1_06_layersbar.png
[undock]: https://raw.githubusercontent.com/AmericanRedCross/QGIS_Training/master/img_v2.8/exercise1_07_undock.png
[redock]: https://raw.githubusercontent.com/AmericanRedCross/QGIS_Training/master/img_v2.8/exercise1_08_redock.png
[toolbarmapnav]: https://raw.githubusercontent.com/AmericanRedCross/QGIS_Training/master/img_v2.8/exercise1_09_toolbarmapnav.png
[zoomin]: https://raw.githubusercontent.com/AmericanRedCross/QGIS_Training/master/img_v2.8/exercise1_10_zoomin.png
[zoominselected]: https://raw.githubusercontent.com/AmericanRedCross/QGIS_Training/master/img_v2.8/exercise1_11_zoominselected.png
[zoomtocountry]: https://raw.githubusercontent.com/AmericanRedCross/QGIS_Training/master/img_v2.8/exercise1_12_zoomtocountry.png
[zoomlast]: https://raw.githubusercontent.com/AmericanRedCross/QGIS_Training/master/img_v2.8/exercise1_13_zoomlast.png
[pan]: https://raw.githubusercontent.com/AmericanRedCross/QGIS_Training/master/img_v2.8/exercise1_14_pan.png
[zoomfull]: https://raw.githubusercontent.com/AmericanRedCross/QGIS_Training/master/img_v2.8/exercise1_15_zoomfull.png
[zoomtolayer]: https://raw.githubusercontent.com/AmericanRedCross/QGIS_Training/master/img_v2.8/exercise1_16_zoomtolayer.png
[draglayer]: https://raw.githubusercontent.com/AmericanRedCross/QGIS_Training/master/img_v2.8/exercise1_17_draglayer.png
