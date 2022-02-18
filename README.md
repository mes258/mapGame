# mapGame

Current plan: 
Use rtree to store geoJSON objects for the roads, zones, and other types. 


For roads, use color and width for different scenerios. 
EG: 
```
{
  "type": "Feature",
  "properties": {
    "stroke": "#a5f24d",
    "stroke-width": 4,
    "stroke-opacity": 0.5
  },
  "geometry": {
    "type": "LineString",
    "coordinates": [
      [
        126.419677734375,
        10.752366085618164
      ],
      [
        125.77972412109376,
        10.792838759247182
      ]
    ]
  }
```


Links and notes:
[Location and Recognition Entity types - Bing Maps | Microsoft Docs](https://docs.microsoft.com/en-us/bingmaps/rest-services/common-parameters-and-types/location-and-recognition-entity-types)
https://data.seattle.gov/resource/ht3q-kdvx.json
[Seattle Streets](https://data-seattlecitygis.opendata.arcgis.com/datasets/seattle-streets/api)
	“INTRLO”: “1ST AVE N AND VALLEY UPPER ST”,
            “DIRLO”: “N”,
            “INTKEYLO”: 28897,
            “INTRHI”: “1ST AVE N AND ALOHA ST”,

[Intersections](https://data-seattlecitygis.opendata.arcgis.com/datasets/intersections/api)
Has UNITDESC: “WOODLAWN AVE N AND N 50TH E ST”
        UNITID: “13331”

Perhaps, draw the street between the intersections. 

R trees are good data structure for this? 

[geojson.io](http://geojson.io/#map=18/47.66136/-122.31985)