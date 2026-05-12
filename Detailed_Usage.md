# Detailed Usage

This section provides details on usage of the cross section application itself, i.e. after an area of interest has been drawn and a cross section application of that area has been generated. **It is recommended to save the generated html locally to store in perpuity locally (see Download HTML button at bottom) and avoid redundant server requests**.

The general workflow for the application is to navigate within the map view to an area of interest and draw a cross section by clicking to add line segments: a geologic cross section will generate in the cross section view. The user can then alter the view or inspect details using the various widgets surrounding the map/cross section views.

There are three primary views (Map View, Cross Section View, and Borehole View). all have built in “tools” on their right sidebars: these tools are described below.  

## Figure Tools

On the right of every figure is a set of plot "tools" that provide the user with control over interactivity. Some these tools are "toggleable", meaning they enable/disable certain features (e.g. box zoom VS. pan), while others perform certain actions (e.g. Save).  

| Symbol | Name | Description |
| :--- | :--- | :--- |
| <a href="https://bokeh.org/"><img src="https://static.bokeh.org/branding/icons/bokeh-icon.svg" width="30"></a> | Bokeh Symbol | Hyperlink to Bokeh website: credits to developers |
| ![Pan](https://docs.bokeh.org/en/3.4.2/_images/Pan.png) | Pan | Allows user to click, hold and drag over the map or cross section plots to move around |
| ![Box Zoom](https://docs.bokeh.org/en/3.4.2/_images/BoxZoom.png) | Box Zoom | Allows user to click, hold and drag over the map or cross section plots to zoom to selected area (Enabling this tool will disable the Pan tool). |
| ![Wheel Zoom](https://docs.bokeh.org/en/3.4.2/_images/WheelZoom.png) | Wheel Zoom | Allows user to adjust the zoom of the map/cross section using the user's mouse wheel.<br>**TIP**: When enabled on the cross section plot, the user can manipulate the vertical exaggeration of the cross section by wheeling when moused over either the X or Y axes. |
| ![PolyDraw](https://docs.bokeh.org/en/3.4.2/_images/PolyDraw.png) | Poly Draw | Used to draw areas of interest on generation page. When enabled, allows user to draw a polygon of the desired subdomain by clicking and holding to start drawing, clicking to add vertices, then clicking and holding to finish drawing. Once drawn, the polygon can be moved by clicking, holding, and dragging. Vertices of an existing polygon can be editted use PolyEdit Tool (see below) |
| ![PolyEdit](https://docs.bokeh.org/en/3.4.2/_images/PolyEdit.png) | Poly Edit | Used to edit vertices on drawn area interest on generation page. When enabled, allows user to edit vertices by clicking, holding and dragging on a vertex. |
| ![Save](https://docs.bokeh.org/en/latest/_images/save.svg) | Save | Allows user to export image of plot. Click will export an image, click and hold will bring up option to copy to clipboard. |
| ![Reset](https://docs.bokeh.org/en/3.4.2/_images/Reset.png) | Reset | Refreshes the plot to its initial state. |
| ![Help](https://docs.bokeh.org/en/3.4.2/_images/Help.png) | Help | Directs user to Bokeh website for official help/documentation |
| ![HoverTools](https://docs.bokeh.org/en/3.4.2/_images/Hover.png) | HoverTools | Each hover tool controls information that appear when the user hovers over the plot area. For example, on the plan view plot, hovering over the second hovertool will read "Picks." With this tool enabled, hovering over a pick location in plan view will bring up information about that pick.|
| ![TapTool](https://docs.bokeh.org/en/latest/_images/tap.svg) | TapTool | When enabled, allows user to select locations on plan view and cross section to bring up in the Borehole Viewer|

#  Application Features/Details

![Layout](https://github.com/gmerritt123/RMOW_XS_Documentation/blob/main/Layout.JPG?raw=true)

## Map View

- Shows layer elevations/thicknesses, downhole locations and basemapping
- Draw a cross section by adding line segments by clicking within model domain on the map
- Can also select a borehole location for borehole viewer by clicking on it

## Cross Section View

- Shows geomodel layer structure of drawn cross section: hovertool displays layer information interactively
- Ability to alter vertical exaggeration by scroll-zooming while hovered over an axis
- Shows downhole data (lithology, well screens, picks) projected to section. Downhole data for a single location can be viewed in more detail in the borehole viewer by clicking on a location on section.

## Borehole Viewer

- Shows downhole data (lithology, well screens, picks) for a selected location
- Location can be selected using Location Lookup (4), clicking on location in map view, or clicking on a location in cross section view

## Widgets/Options

**1.** Select Layer to view on plan view, and select viewing layer top elevation or thickness (isopachs). Legend/colourbar will update accordingly

**2.** Select basemap options, toggle visibility of well name labels, and adjust the opacity of layer elevation/thickness

**3.** Main control toggle for drawing/not drawing cross section. When set to “Draw Cross Section”, clicking in plan view will trigger cross section draw (i.e. add cross section line segments). If set to “Select Borehole”, clicking in plan view will not trigger additional cross section line segments, but clicking on a borehole location will select it for borehole viewer

**4.** Location lookup options: ability to type in sys_loc_codes or well names to select a particular location

**5.** Legend showing the various Location types. Click on each legend item to filter on/off (applies to both map view and cross section view)

**6.** Toggle visibility of certain data on cross section figure

**7.** Adjust the projection distance threshold for putting locations on section. If a location is within this distance of the drawn section, it will be shown on section

**8.** Reset cross section (clear the current drawn line)

**9.** Download html: saves a standalone html application for local use (still requires internet connection to use but will be available in perpetuity for the user)
