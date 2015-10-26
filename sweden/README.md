## Sources

### swedish-lan.geojson

* Swedish regions (län)
* Does not define the coast
* Gotska sandön is not included in Gotlands län

```
wget http://www.val.se/val/val2014/statistik/gis/valgeografi_lan.zip
unzip valgeografi_lan.zip
ogr2ogr -f GeoJSON -t_srs crs:84 ../../sweden/swedish-lan.geojson valgeografi_lan.shp
```

### swedish-localities.geojson

* Positions for all Swedish localitites (population >= 200)

https://sv.wikipedia.org/wiki/Lista_över_Sveriges_tätorter

### swedish-municipalities*.geojson

* Swedish municipalities (kommuner)
* Does not define the coast
* Gotska sandön is not included in Gotlandsregionen

```
wget http://www.val.se/val/val2014/statistik/gis/valgeografi_kommun.zip
unzip valgeografi_kommun.zip
ogr2ogr -f GeoJSON -t_srs crs:84 ../../sweden/swedish-municipalities.geojson valgeografi_kommun.shp
```
