# TrailForge 2.0.11

Built directly from the supplied TrailForge 2.0.10 source.

## Overpass-first POI discovery
TrailForge now tries four Overpass mirrors in order:
- overpass.kumi.systems
- overpass-api.de
- lz4.overpass-api.de
- z.overpass-api.de

The Overpass query explicitly requests named natural water, any named water type, natural lake, mountain passes, peaks, campsites, and names containing Pass, Saddle, Gap, Col, Lake, Pond, Reservoir, Peak, Summit, or Mountain. It searches both a widened route-area box and route-sample circles.

## Nominatim fallback
Nominatim is used only when every Overpass mirror fails or Overpass returns no named features. Fallback terms remain Pass, Saddle, Gap, Col, Lake, Pond, Reservoir, Peak, Summit, Mountain, and Campground.

## Configurable thresholds
Existing acceptance distances remain unchanged and configurable. Overpass corridor radius, sample spacing, timeout, mirrors, and search padding are also configurable.

## Retained from 2.0.10
- POI diagnostics popup
- Raw names and rejected distances
- POI elevation labels and click-to-map
- Right-click POI edit, convert to manual, and delete
- Manual POIs
- Print report, GPX, KML, Google Earth, and route library
