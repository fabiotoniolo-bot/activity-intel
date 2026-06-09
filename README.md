# activity-intel

Public geospatial reference data, organized as GeoJSON for use in mapping tools.

## Contents

- `geometries.json` — a GeoJSON `FeatureCollection` of O&G exploration
  and production areas in Brazil (concession blocks, production fields, and the
  pre-salt polygon), derived from public ANP open data and re-projected/cleaned
  for convenient web consumption.

Each feature carries:

| property     | meaning                                  |
|--------------|------------------------------------------|
| `layer_type` | `Block`, `Field`, or `PreSalt`           |
| `source_id`  | identifier from the source dataset       |
| `name`       | area name (null for the pre-salt polygon)|
| `operator`   | operator name (null where not applicable)|

Coordinates are WGS84 / SIRGAS 2000 longitude–latitude, rounded to 5 decimals.

## Source & licence

Built from publicly available ANP datasets. This repository only reorganizes
that public data into a single GeoJSON file; it adds no proprietary content.

## Updates

Regenerated periodically from the upstream public data and committed here.# activity-intel
