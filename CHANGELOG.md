# 2.0.12
- Retained lake and pond POI searches and the existing Lake classification.
- Updated Overpass mirror order and endpoint selection, including a North America-specific instance.
- Increased the per-request Overpass timeout and narrowed POI search padding and route corridor parameters to reduce server load.
- Preserved existing POI acceptance distances and Nominatim fallback behavior.
- Replaced the previously committed OpenRouteService credential in config.json; add a newly issued key locally before using routing.

# 2.0.11
- Added lz4 and z Overpass mirrors.
- Added explicit natural=water, water=*, natural=lake, mountain_pass=yes, peak, and campsite queries.
- Added named Pass/Saddle/Gap/Col/Lake/Pond/Reservoir queries.
- Added route-sample around queries in addition to widened bounding-box queries.
- Uses Nominatim only after all Overpass mirrors fail or return no named features.
- Kept all distance filters configurable and unchanged.
