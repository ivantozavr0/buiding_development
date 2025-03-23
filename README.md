<h1 align="center"><img src="https://www.ci-romero.de/wp-content/uploads/2018/06/Stadt-MadebyMade-the-Noun-Project-CC-2018.png" alt="" height="50"/> This is the automatic site development project </h1>

## User requirements

<ul>
  <li>Jupyter-notebook</li>
  <li>Python libraries: geopandas,  shapely, networkx</li>
</ul>

## Brief information

This program expects an input file in *.geojson format. The following must be specified inside the file: the zone allowed for construction, prohibited zones ('restriction': 'no_build') and roads.

During the course of the program, you will also need to manually enter various building parameters.

In this project, sections of arbitrary shape are built up with rectangular houses in accordance with the user's requirements such as:
house size, minimum distance between buildings, maximum building density. 

If the houses are located far enough away (this is a configurable parameter) from existing roads, then using algorithm A*, the program will try to build the optimal road to the new house so that the new path does not cross prohibited areas.

In addition, this program tries to build square parks with a specified minimum size.

See a more detailed description inside the program file.
