<div style="font-weight: bold;">Built by<img style="width:200px; text-align:left; margin: 0px 0px 0px 0px;" src="https://i.imgur.com/fACuCVR.jpeg" /> <br> in collaboration with <img src="https://www.regionofwaterloo.ca/media/4z3ggnnp/region-of-waterloo-logo.svg" align="middle"/>
 
# Region of Waterloo Cross Section Tool Generator
This application allows Region of Waterloo staff to generate standalone cross-section tools for an arbitrary area of interest, displaying borehole lithology, water levels, geologic picks, and  hydrostratigraphic layers present in the Moraine or Cambridge groundwater flow models (see [Data Sources](https://github.com/gmerritt123/RMOW_XS_Documentation/blob/main/DataSources.md) for more information).
## Overview and Quickstart
After successful login, a map of the Region of Waterloo is displayed with lines illustrating the Moraine and Cambridge Model domains, and an Ontario Geological Survey bedrock geology subcrop map for reference.

Users first use the WheelZoom, or BoxZoom to navigate to an area of interest i.e. a region where they would like to generate a cross section tool. Users then draw an area of interest by clicking and holding to start, clicking to add vertices, then click and hold to finish the polygon. Users can modify the polygon using the PolyDraw/PolyEdit tools (see [Detailed Usage](https://github.com/gmerritt123/RMOW_XS_Documentation/blob/main/Detailed_Usage.md) for more information). Users then selects which hydrostratigraphic model to display on the cross section tool - the Cambridge Model or the Moraine Model, using the toggle button located above the plan view map. Users should choose the Cambridge Model when the area of interest lies in the Cambridge Model domain, and the Moraine Model for areas of interest outside the Cambridge Model (including Branchton Meadows). See [Data Sources](https://github.com/gmerritt123/RMOW_XS_Documentation/blob/main/DataSources.md) for more information.

Once an area of interest polygon has been drawn, users can generate a cross section tool for that area by clicking the green "Generate XS Tool" button below the map to send a request to server. A text status will update beneath the map denoting the progress of the request: the tool will take up to 2 minutes to generate. 

**IMPORTANT:** Popups must be allowed/enabled for the cross section generation website, as the delivered html needs to open in a new tab.

The cross section application will "auto-scale" the layer resolution based on the area of the cross section application; smaller cross section areas will have higher delivered rasters (e.g. 5 m) while large cross section areas will have lower resolution rasters.

Once an application generated, it can be saved locally and kept in perpetuity. Refer to [Detailed Usage](https://github.com/gmerritt123/RMOW_XS_Documentation/blob/main/Detailed_Usage.md) for navigating the application itself.