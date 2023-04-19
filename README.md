# si507_w23_final_project

OSMnx:
- Description from the repo and documentation
  - OSMnx is a Python package that lets you download geospatial data from OpenStreetMap and model, project, visualize, and analyze real-world street 
    networks and any other geospatial geometries. You can download and model walkable, drivable, or bikeable urban networks with a single line of   
    Python code then easily analyze and visualize them. You can just as easily download and work with other infrastructure types, amenities/points of 
    interest, building footprints, elevation data, street bearings/orientations, and speed/travel time.
  - OSMnx is built on top of GeoPandas, NetworkX, and matplotlib and interacts with OpenStreetMap APIs to:
    Download and model street networks or other networked infrastructure anywhere in the world with a single line of code
    Download any other spatial geometries, place boundaries, building footprints, or points of interest as a GeoDataFrame
    Download by city name, polygon, bounding box, or point/address + network distance
    Download drivable, walkable, bikeable, or all street networks
    Download node elevations and calculate edge grades (inclines)
    Impute missing speeds and calculate graph edge travel times
    Simplify and correct the network's topology to clean-up nodes and consolidate intersections
    Fast map-matching of points, routes, or trajectories to nearest graph edges or nodes
    Save networks to disk as shapefiles, GeoPackages, and GraphML
    Save/load street network to/from a local .osm XML file
    Conduct topological and spatial analyses to automatically calculate dozens of indicators
    Calculate and visualize street bearings and orientations
    Calculate and visualize shortest-path routes that minimize distance, travel time, elevation, etc
    Visualize street networks as a static map or interactive Leaflet web map
    Visualize travel distance and travel time with isoline and isochrone maps
    Plot figure-ground diagrams of street networks and building footprints

- OSMnx can be installed via pip
  - https://pypi.org/project/osmnx/
  
- Github and Documentation
  - Github
    - https://github.com/gboeing/osmnx
  - Documentation
    - https://osmnx.readthedocs.io/en/stable/#


API Key:
- A Google Maps Elevation API key is needed for this code to work.
  - Create an Google Cloud account and go to Credentials under APIs & Service to create a key.
  - Either leave the key as universal or restrict it to just Maps Elevation API.
- I've run the code in the repo so the cache has been created.
  - All you'll need is a valid API key, but the function should detach the cache and not use your key.
  - If for some reason it does call the API:
      - I'm only getting the nodes on the route so it will be no where near the free $200 monthtly API allowance.

Python packages needed:
- numpy
- pandas
- matplotlib.pyplot
- seaborn
- branca
- jinja2
- osmnx
- networkx
- folium

Using the .ipynb file:
- There are 7 functions and 1 class, run all of these first.
- There is one cell at the bottom that creates three outputs.
  - Uncomment i80_route_map to see the route; used to compare to Google Maps.
  - Uncomment i80_route_final_web_map to see the final output of this program.
  - A .html file is created when this cell is ran titled i80_route_final_web_map.
    - Use this in your browser.
