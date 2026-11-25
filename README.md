# ShredCast trails

Pre-built trail data for the ShredCast app's map (Oregon, Washington, Idaho, Northern California
and British Columbia), served as static files by GitHub Pages so the app doesn't have to query
an Overpass server.

Nothing is edited here by hand. Once a week a job on the maintainer's server runs the app's trail
query against its own Overpass instance for every zoom-12 map tile in the region and publishes
the answers here, one JSON file per tile.

- **Layout** (once the first build lands): `z12/<x>/<y>.json`, each the Overpass JSON answer for
  that tile (paths and tracks with their names, MTB ratings, `sac_scale`, ski-touring ways and
  route relations).
- **Source code:** the query is `MapTrails.query` in the ShredCast app.

## Data license

The data is from OpenStreetMap, © OpenStreetMap contributors, available under the
[Open Database License (ODbL)](https://opendatacommons.org/licenses/odbl/). See
<https://www.openstreetmap.org/copyright>. These files are a derived database under the same
license.
