# OBD2Nav map data

Map and routing databases used by the OBD2Nav app, one archive per Ukrainian
region (24 oblasts and Crimea; Kyiv is included in Kyiv Oblast, Sevastopol in
Crimea). The app itself gets these files through Google Play; this repository
is the public copy required by the Open Database License.

**Data:** © OpenStreetMap contributors, licensed under the
[Open Database License (ODbL) 1.0](https://opendatacommons.org/licenses/odbl/1-0/)
(full text in [LICENSE](LICENSE)). See https://www.openstreetmap.org/copyright.

**Source:** Geofabrik extract `ukraine-261025.osm.pbf` (OpenStreetMap data as of 2026-10-25),
https://download.geofabrik.de/europe/ukraine.html

## Contents of each archive (`obd2nav-<region>-ukraine-261025.zip`)

| file | what | built with |
|---|---|---|
| `map.pmtiles` | vector tiles, [OpenMapTiles](https://openmaptiles.org/) schema (© OpenMapTiles, CC-BY 4.0) | Planetiler (Apache 2.0) |
| `landmarks.pmtiles` | outlines of fuel stations, supermarkets, malls, markets, stations | Planetiler, own profile |
| `graph.tar` | routing graph tiles | Valhalla 3.6.3 (MIT) |
| `LICENSE-NOTICE.txt` | attribution, source and what was changed | |
| `pack.json` | region id, extract, Valhalla version | |

Each region covers the 0.25° cells that lie in the region or within ~25 km of
its border. `map.pmtiles` also includes ocean polygons (osmdata.openstreetmap.de,
ODbL), lake centerlines derived from OpenStreetMap (ODbL) and Natural Earth
(public domain).

Checksums: `SHA256SUMS`.

---

# Дані карти OBD2Nav

Бази карти й маршрутів застосунку OBD2Nav — архів на кожну область України
(24 області й Крим; Київ — у Київській області, Севастополь — у Криму).
Застосунок отримує ці файли через Google Play; тут — публічна копія, якої
вимагає ліцензія ODbL.

**Дані:** © OpenStreetMap contributors, ліцензія ODbL 1.0 (повний текст — [LICENSE](LICENSE)).
**Джерело:** витяг Geofabrik `ukraine-261025.osm.pbf` (дані станом на 2026-10-25).
Склад архіву — таблиця вище; повідомлення про ліцензію й зміни — `LICENSE-NOTICE.txt`.
