# forestparcel
Interactive map tool for Finnish forest property monitoring with parcel boundaries, historical aerial imagery, and measurement tools.

# ForestWatch

A browser-based tool for monitoring Finnish forest properties using open data from Maanmittauslaitos (National Land Survey).

## Features
- **Property parcels** — Add properties by ID (kiinteistötunnus) and view boundaries on the map
- **Neighbor parcels** — Automatically loads and displays neighboring properties
- **Historical aerial imagery** — Compare aerial photos from 2008–2025 with swipe comparison
- **Measurement tools** — Measure distances and areas directly on the map
- **Bilingual** — Finnish and English interface

## Getting Started

1. Open `metsavahti.html` in a browser
2. Enter your MML API key in the top bar
3. Add a property using its kiinteistötunnus (e.g. `049-401-1-123`)

## API Key

You need a free API key from Maanmittauslaitos. Register at
[https://www.maanmittauslaitos.fi](https://www.maanmittauslaitos.fi).

## Data Sources

- [MML Open Parcel API](https://www.maanmittauslaitos.fi) — Property boundaries and neighbor data
- MML WCS — Historical aerial imagery

## Tech Stack

- Leaflet + MML WMTS layers
- proj4js for coordinate transformations (ETRS-TM35FIN)
- Chart.js for price visualizations
- html2pdf.js for PDF export
- Vanilla JavaScript, single HTML file, no build step
