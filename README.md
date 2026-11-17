# TrailForge 2.0.12

Built from the TrailForge 2.0.11 source with a focused update to automatic POI discovery.

## POI discovery updates
- Keeps `lake` and `pond` searches enabled; lake remains a supported automatic POI category.
- Replaces the previous Overpass mirror list with distinct public alternatives, including a North America endpoint.
- Uses a 15-second per-request Overpass timeout and smaller route corridor and bounding-box padding to reduce query load.
- Keeps Nominatim as fallback and preserves existing POI acceptance distances.

Public Overpass and Nominatim services are community services and can still be temporarily unavailable or impose usage limits. The diagnostic popup remains the best way to identify provider failures for a particular route.

## API key safety
`config.json` is a local runtime configuration file. Replace the OpenRouteService placeholder with a newly issued API key before using routing. Do not commit API keys to a public repository.
