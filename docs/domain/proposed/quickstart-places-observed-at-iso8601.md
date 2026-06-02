# Quickstart places: `observed_at` timestamp format

## Source

- File: `data/workshop/quickstart-places.geojson`

## Field convention

- Field: `properties.observed_at`
- Type: string
- Format: ISO 8601 / RFC 3339 datetime **with an explicit timezone offset**.

Example value from the snapshot:

- `2026-05-15T12:00:00+00:00`

## Notes / contrast

- This quickstart teaching sample uses ISO 8601 strings (offset included), which is useful to contrast with other sources that represent timestamps as **epoch milliseconds** (e.g., the D1 USGS earthquakes snapshot).