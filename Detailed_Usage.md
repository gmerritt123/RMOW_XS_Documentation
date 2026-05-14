# Detailed Usage

This section provides details on usage of the cross section application itself, after an area of interest has been drawn, and a cross section application is generated. **We recommend the user saves the generated html to their hard drive to store it in perpuity (see Download HTML button at bottom) as there will be a time-limited window to generate new applications**.

### General Workflow 
Users can navigate in the Plan View map to an area of interest. Users can draw a cross-section by clicking to add line segments, and a cross section will appear below the map in the Cross-Section View. Users can make changes to the view or inspect details on the Map or Cross-Section Views using the surrounding widgets.

There are three primary views (Plan View map, Cross-Section View, and Borehole View). Each has built in “Tools” located on the right, which are described below.  

## Figure Tools

On the right of every figure is a set of "Tools" that allow the user to control the data displayed. Some tools enable or disable certain features, such as the box zoom or pan functions, while others perform  actions, such as the Save feature.  

| Symbol | Name | Description |
| :--- | :--- | :--- |
| <a href="https://bokeh.org/"><img src="https://static.bokeh.org/branding/icons/bokeh-icon.svg" width="30"></a> | Bokeh Symbol | Hyperlink to Bokeh website: credits to developers |
| ![Pan](https://docs.bokeh.org/en/3.4.2/_images/Pan.png) | Pan | Allows user to click, hold and drag over the map or cross section plots to move around |
| ![Box Zoom](https://docs.bokeh.org/en/3.4.2/_images/BoxZoom.png) | Box Zoom | Allows users to click, hold and drag over the map or cross section plots to zoom to selected area (Enabling this tool will disable the Pan tool). |
| ![Wheel Zoom](https://docs.bokeh.org/en/3.4.2/_images/WheelZoom.png) | Wheel Zoom | Allows users to adjust the zoom of the map/cross section using the user's mouse wheel.<br>**TIP**: When enabled on the cross section plot, users can manipulate the vertical exaggeration of the cross section by wheeling when moused over either the X or Y axes. |
| ![PolyDraw](https://docs.bokeh.org/en/3.4.2/_images/PolyDraw.png) | Poly Draw | Used to draw areas of interest on generation page. When enabled, users can draw a polygon of the desired subdomain by clicking and holding to start drawing, clicking to add vertices, then clicking and holding to finish drawing. Once drawn, the polygon can be moved by clicking, holding, and dragging. Vertices of an existing polygon can be edited use PolyEdit Tool (see below) |
| ![PolyEdit](https://docs.bokeh.org/en/3.4.2/_images/PolyEdit.png) | Poly Edit | Used to edit vertices on drawn area interest on generation page. When enabled, allows user to edit vertices by clicking, holding and dragging on a vertex. |
| ![Save](https://docs.bokeh.org/en/latest/_images/save.svg) | Save | Allows users to export image of plot. Click will export an image, click and hold will bring up option to copy to clipboard. |
| ![Reset](https://docs.bokeh.org/en/3.4.2/_images/Reset.png) | Reset | Refreshes the plot to its initial state. |
| ![Help](https://docs.bokeh.org/en/3.4.2/_images/Help.png) | Help | Directs users to Bokeh website for official help/documentation |
| ![HoverTools](https://docs.bokeh.org/en/3.4.2/_images/Hover.png) | HoverTools | Each hover tool controls information that appear when the user hovers over the plot area. For example, on the Plan View map, hovering over the second hovertool will read "Picks." With this tool enabled, hovering over a pick location in the Plan View map will bring up information about that pick.|
| ![TapTool](https://docs.bokeh.org/en/latest/_images/tap.svg) | TapTool | When enabled, users can select locations on the Plan View map, or in the Cross Section View, to display the well or borehole details in the Borehole Viewer.|

#  Application Features/Details

![Layout](https://github.com/gmerritt123/RMOW_XS_Documentation/blob/main/Layout.JPG?raw=true)

## Map View

- Shows layer elevations or thicknesses (isopachs), well/borehole locations and basemap features.
- Draw a cross section by clicking to add line segments within the model domain on the map.
- Can also select a borehole/well location that will then be diplayed in the Borehole View by clicking on the well (must have **Select Borehole** enabled under the title **XS Draw Options**).

## Cross Section View

- Shows the interpreted hydrostratigraphic layer structure on the cross section: the hovertool displays the layer information interactively.
- Users can change the vertical exaggeration by hovering over the Y or X axis and scrolling their mouse-wheel to stretch the cross section horizontally or vertically.
- Downhole data such as lithology, well screens, and geologic picks can be projected onto the cross section. Downhole data for a single location can be viewed in detail using the borehole viewer by clicking on a location on section.

## Borehole Viewer

- Downhole data such as lithology, well screens, and geologic picks are displayed for a selected location (borehole, well).
- Location can be selected by: a) entering the borehole sys_loc_code in the location Lookup (see (4) on layout diagram), b) clicking on a location in the Map View (when "Select Borehole" is selected above the Map View), or c) clicking on a location in Cross Section View.

## Widgets/ Options

**1.** **Layer Drop Down List**: Users can select which top elevation or layer thickness (isopach) for the various interpreted hydrostratigraphic layers to display on the Plan View map. Legend/colour bar will update automatically.

**2.** **Basemap**: Users use these buttons to select which of the three basemaps to display, toggle the visibility of the well name labels, and adjust the opacity of layer elevation/thickness illustrated on the Plan View map. 

**3.** **XS Draw**: Users click on the two options to conduct one of the following functions on the Plan View Map: a) draw a cross-section, or b) select borehole(s) to view in the Borehole Viewer. If “Draw Cross Section” is enabled, clicking in the Plan View map will initiate the drawing of cross section line segments. If “Select Borehole” is enabled, clicking in the Plan View Map on a borehole or well location  will load data in the Borehole View.  

**4.** **Location Lookup** options: Users can select a sys_loc_code or well name and enter text in the box below to select a particular well or borehole location. The Plan View map will then zoom to display that borehole or well location. 

**5.** **Legend/Filter**: Users can select the text features in the legend to turn on and off (filter) the location features on both the Plan View map and Cross Section View. 

**6.** **Show on Cross Section**: Users can click the box to turn on and off the data visualized on the cross section. 

**7.** **Cross Section Lateral Slider**: Users can use the slider bar to adjust the distance that they would like a borehole/ well to be projected onto the cross-section line and therefore, displayed on the cross section. If a location is within this distance (metres) of the drawn section, it will be displayed on section. 

**8.** **Reset Cross Section**: Users can select this button to clear the current drawn line and cross section and draw/ generate a new cross section. 

**9.** **Download html**: Users can saves a standalone html application for local use (still requires internet connection to use but will be available in perpetuity for the user)