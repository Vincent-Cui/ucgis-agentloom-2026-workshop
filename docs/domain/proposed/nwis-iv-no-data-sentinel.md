# NWIS IV no-data sentinel (-999999)

## What this is

USGS NWIS Instantaneous Values (IV) JSON responses declare a **no-data sentinel** value under the variable metadata. In the D3 snapshot, this appears as:

- `value.timeSeries[0].variable.noDataValue = -999999.0`

Catalog/ingest code MUST treat observations equal to this sentinel as **missing**, not as a real measurement.

## Evidence (D3 snapshot)

From `data/snapshots/d3-usgs-nwis-suwannee-24h.json` (first ~8KB is sufficient to see the declaration):

- `... "variable": { ... "noDataValue": -999999.0, ... }`

The observations themselves live at:

- `value.timeSeries[0].values[0].value[]`
  - each element has `value` (string), `dateTime` (offset timestamp), and `qualifiers`.

## Implications for downstream use

- When parsing `values[0].value[i].value`, compare numerically to `-999999` **after** converting from string.
- Missing values should be excluded from plots/aggregations and represented as `null`/NaN in derived outputs.

## Non-goals

- This note does not define how to impute gaps; it only documents the NWIS sentinel convention.