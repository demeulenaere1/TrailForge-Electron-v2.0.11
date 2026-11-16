# 2.0.11
- Added lz4 and z Overpass mirrors.
- Added explicit natural=water, water=*, natural=lake, mountain_pass=yes, peak, and campsite queries.
- Added named Pass/Saddle/Gap/Col/Lake/Pond/Reservoir queries.
- Added route-sample around queries in addition to widened bounding-box queries.
- Uses Nominatim only after all Overpass mirrors fail or return no named features.
- Kept all distance filters configurable and unchanged.
