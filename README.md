# Deriviste traffic signs

Deriviste traffic signs is a fork from Deriviste, whose is a proof-of-concept OpenStreetMap editor for adding POIs directly from street-level imagery (Mapillary). Ok, it's not really an editor as you can't edit anything, only create.

Deriviste is written in largely prehistoric JavaScript and is licensed WTFPL with no warranty. Patches are lovely. Please send patches.

Origins of Deriviste

In October 2018, a new OpenStreetMap tool called Deriviste was introduced by Richard Fairhurst. This tool presented the user with a way to directly create OSM data from user images on Mapillary, including by clicking directly on the image. Thanks to an experimental feature in the open-source MapillaryJS library, Deriviste meant that a click in the Mapillary image was translated to a point on the map. Richard borrowed some code from the OpenStreetMap iD editor in order to allow searching for OSM tag presets, then used simple user authentication to allow submission of the newly created data as an OSM changeset.

With a fork of this tool called Deriviste_traffic_signs you have a simple interface to add nodes to OpenStreetMap based on what you see in Mapillary street-level imagery.

    Click a place on the map with a green highlight.
    
	Double-click a traffic_sign object on the street imagery to place a node there.
    
	Use the search box to find the code for this country in the preset.
    
	Complete the tags using the right-hand tag table (don't forget key side).Delete the code for what direction is not. Deriviste screenshot4.png
    
	Repeat until you're done.
    
	Enter your OSM username and password, then click 'Upload'.
    
	Make an overpass-turbo query to detect the new nodes (you can try to find traffic_sign:forward or traffic_sign backward)
    
	Export it to other editor like JOSM, Vespucci, iD or Potlatch. Now you can attach to the road the traffic sign if you want to. Also you can remove any 
	duplicates and generally clean up. The Mapillary API sometimes fails to find co-ordinates for a click.

The currently selected node is shown in red, others in blue. You can drag the nodes around to fine-tune their position. (You can also place nodes by double-clicking on the map.) 

You can see it live at https://yopaseopor.github.io/deriviste/index.html.

