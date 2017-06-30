# Label for the polygon sides (L.PolySideLabel) #
This class will show the distance between each of the vertices of the polygon/polyline when the mouse is on top of it.
It works great for most browsers, except for IE7/8 where on hover, it shows the info for all the polygones at the same time (and not only the one you are hovering over).

## Notes ##
* There is a limit of sides (option __bodersLimit__ = 8) which you can change. This limit sets the max amount of sides for a polygon to show the length info. If is greater, then nothing is shown.
* If the sides are too small (option __minSideLength__ 40 meters), then instead of the distance, you will get characters and a leyend on the side indicating the sides for each character.
* There is a limit for the visible area (option __minAreaToShow__). If the visible drawn area is smaller than this, the info wil not be shown.

Code example:

```
    var polygon = new L.Polygon(...);
    ....
    map.addLayer(polygon);
    var labelPolygon = new L.PolySideLabel(polygon, options);
```

