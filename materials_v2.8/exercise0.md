# Exercise 0: Installing QGIS & Plugins
In this exercise you will learn how to install QGIS and add plugins to expand the functionality of the software. The instructions will vary depending on your operating system. Since this is open-source software, changes are constantly being made to the code. This manual was created version 2.8.2 Wien. Icons and menus may be different in other versions.

## Section 1: Install QGIS

**NOTE:** If you have an earlier version of QGIS installed on your computer, you will need to uninstall it.

1. Copy the training folder to your computer from the USB drive provided.
2. The training folder contains QGIS 2.8 installation file: `QGIS-OSGeo4W-2.8.2-1-Setup-x86_64.exe`.
 **OR**
3. Use a web browser and navigate to http://www.qgis.org.
 - Click download and select the current version (choose the standalone installer recommended for new users).
4. Right click the \*.exe file and select Run as Administrator.
 - Follow the installation instructions.
 - When you reach the Choose Components screen you do not need to select any of the Data Sets.

## Section 2: Install Plugins
Plugins add functionality to the basic installation of QGIS. These tools are written by members of the open source community. Some are highly complex while others are basic, meant to accomplish one specific task. You can install as many or as few as needed. You can download the Plugins for this training or you can install them from the training folder.

1. We have pre-downloaded several commonly used plugins which you can install off-line, you can skip to step 5 if you will download the plugins.  
2. Open the 02_Plugins folder in the training folder.  
3. In a separate window, browse to the .qgis folder located at `C:\Users\YourUserName\.qgis\`.
4. Copy or move the python folder from the `Training_Workshop\02_Plugins` folder to the `.qgis` folder, selecting yes to any merge prompts.  
 ![][merge]
5. Let’s open QGIS and look at the plugins we’ve installed. If you have a shortcut for QGIS on your desktop double click it to start QGIS; otherwise, click Start > All Programs > QGIS Wien > QGIS Desktop(2.8.2).  
 **NOTE:** Make sure that you open QGIS Desktop, not the similarly titled QGIS Browser.
 ![][desktopicon]
6. Click Plugins > Manage and Install Plugins…
 **NOTE:** You must be connected to a stable internet connection to download plugins.  
 ![][pluginsmenu]
7. The Plugins window will appear.
8. If installing plugins from the internet… select the All tab, search each plugin, select it, and then click *Install plugin*. Get the following plugins: Point sampling tool, Statist, Open Layers Plugin.  
 **OR**
9. If only checking plugins installed from the training folder you can click Abort fetching and move to the next step.  
 ![][abortfetching]
10. Click the Installed tab and make sure all the plugins (except Globe) are checked.  
 ![][installedplugins]
11. Click the Settings tab, select 'Check for updates on startup', and select 'once a day' from the dropdown menu.  
 ![][settingstab]
12. Click Close then restart QGIS Desktop.
13. Plugins will be accessible as toolbar buttons or through new menu options.  
 **Hint:** Hover with the mouse over a button to display the text description.
 ![][pointsampling-icon]
 ![][openlayers-menu]
14. If you experience problems after installing a plugin, uninstall it.
 - Follow steps 6-8 but click *Uninstall plugin* instead of *Install plugin*.  
 **NOTE:** Some plugins are built-in to QGIS and cannot be uninstalled.

**End Exercise.**  
*The information provided in this exercise is not official American Red Cross information and does not necessarily represent the views of the American Red Cross.*

[merge]: https://raw.githubusercontent.com/AmericanRedCross/QGIS_Training/master/img_v2.8/exercise0_01_merge.png
[desktopicon]: https://raw.githubusercontent.com/AmericanRedCross/QGIS_Training/master/img_v2.8/exercise0_02_desktopicon.png
[pluginsmenu]: https://raw.githubusercontent.com/AmericanRedCross/QGIS_Training/master/img_v2.8/exercise0_03_pluginsmenu.png
[abortfetching]: https://raw.githubusercontent.com/AmericanRedCross/QGIS_Training/master/img_v2.8/exercise0_04_abortfetching.png
[installedplugins]: https://raw.githubusercontent.com/AmericanRedCross/QGIS_Training/master/img_v2.8/exercise0_05_installedplugins.png
[settingstab]: https://raw.githubusercontent.com/AmericanRedCross/QGIS_Training/master/img_v2.8/exercise0_06_settingstab.png
[pointsampling-icon]: https://raw.githubusercontent.com/AmericanRedCross/QGIS_Training/master/img_v2.8/exercise0_07_pointsampling-icon.png
[openlayers-menu]: https://raw.githubusercontent.com/AmericanRedCross/QGIS_Training/master/img_v2.8/exercise0_08_openlayers-menu.png
