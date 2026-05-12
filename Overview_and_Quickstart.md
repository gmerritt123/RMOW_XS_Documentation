<div style="font-weight: bold;">Built by<img style="width:200px; text-align:left; margin: 0px 0px 0px 0px;" src="https://i.imgur.com/fACuCVR.jpeg" /> <br> in collaboration with <img src="https://www.regionofwaterloo.ca/media/4z3ggnnp/region-of-waterloo-logo.svg" align="middle"/>
 
# Region of Waterloo Cross Section Tool Generator
This application allows Region staff to generate standalone cross section applications for an arbitrary area of interest, using either the Moraine or Cambridge geomodels (see data sources section for more information).
## Overview and Quickstart
After successful login, a map is shown of the Region of Waterloo, with the Moraine and Cambridge model domains outlined.

The user then draws an area of interest on the map using the WheelZoom + PolyDraw/PolyEdit tools (See Figure Tools section below for usage) and selects which model to build from (i.e. Cambridge model vs Moraine Model) using the toggle button located above the map. In general, one should build from the Cambridge model when the area of interest is within the Cambridge model domain, where bedrock layers are more relevant, and otherwise build from the Moraine model. See data sources section for more information.

Once an area of interest polygon has been drawn, the user can request a cross section tool for that area by clicking the green "Generate XS Tool" button below the map to send a request to server. A text status will update to the right of the figure denoting the progress of the request: by far the largest bottleneck is the delivery of the prepared html which will likely take 20-30 seconds, as the server is uploading and your browser is downloading a ~35 mb standalone html application.

A note on resolution: This application has been tuned to "auto-scale" the layer resolution of the requested subdomain such that the delivered application is 30 to 40 mb in size. A smaller subdomain will thus result in a higher delivered raster resolution (e.g. 5 m) while a large subdomain will result in a lower one.

**IMPORTANT:** Popups must be allowed/enabled for the cross section generation website, as the delivered html needs to open in a new tab.

Once an application generated, refer to Detailed_Usage.md for using the application.