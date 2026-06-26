# Chesapeake Bay Dashboard
Python based website dashboard for general Chesapeake Bay data available through public governt APIs. Displays further anaylsis of said data pertaining to health of the Bay and fishing conditions.  
# Features:
- Docker containerization
- Individual data querying methods for each resource
- Covariance of individual fish availibility factors vs daily weather reports. 0-5 star ranking of covariance in each location
- 2D navigatable map with pins for buoy and port locations (zoom in/out/reset, drag to pan, click to display additional location data)
- Data caching or local file storage to prevent excessive querying and load times (frequency depends on datatype and usage)
- Report card health history line graph
- Physical Habitat Metrics with slider for year shown (1985-2023)
# Resources  
- Fish avaibility (hardcoded), https://eyesonthebay.dnr.maryland.gov/eyesonthebay/seasonalconditions.cfm
- Buoy Data, https://buoybay.noaa.gov/data/data-download
- North and South port data:  
  * view-source:https://tidesandcurrents.noaa.gov/ports/textscreen.shtml?port=cn  
  * view-source:https://tidesandcurrents.noaa.gov/ports/textscreen.shtml?port=cs
- Report card data, https://ecoreportcard.org/report-cards/chesapeake-bay/bay-health/
- Physical habitat data, https://www.sciencebase.gov/catalog/item/6945a063d4be02649be040f2
- Possible additional resource: https://data.chesapeakebay.net/search?categories=%252Fcategories%252Fdownloadable%2520datasets
# Design choices
- Python3 development
- Dash by Plotly extension
- OpenLayers python extension for 2d maps, https://github.com/openlayer-ai/openlayer-python
