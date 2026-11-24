# Auto Street Mapper V4 — Prototype
Arabic RTL progressive web app for outlining a neighborhood, selecting a start point, fetching OpenStreetMap roads and assigning sequential labels. Roads at/above the chosen threshold get two independently numbered markers at approximate quarter/three-quarter positions.


## Run
Open `index.html` from a local static server or publish the repository root with GitHub Pages. Internet access is required for Leaflet tiles and Overpass road data.

## Notes / limitations
- The boundary is user-drawn and polygonal; the Overpass query uses the drawn polygon.
- Ordering is a prototype: roads are sorted by midpoint distance to the chosen start point, not a street-network traversal algorithm.
- Long-road split positions are approximated along the road geometry. Please review before operational use.
- This is a static app; no server or account is needed. Road queries go to Overpass API and map tiles to OpenStreetMap.
