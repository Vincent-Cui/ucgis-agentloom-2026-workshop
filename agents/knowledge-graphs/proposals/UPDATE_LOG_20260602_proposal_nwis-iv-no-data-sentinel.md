# UPDATE_LOG: Proposal — NWIS IV no-data sentinel (-999999)

**Date**: 2026-06-02
**Author (agent)**: builder-agent
**Slug**: nwis-iv-no-data-sentinel
**Proposed node type**: knowledge
**Target graph**: domain-knowledge

---

## Justification (the "why")

NWIS IV responses declare a no-data sentinel (variable.noDataValue = -999999) that catalog/ingest code must map to missing values to avoid plotting/aggregating bogus measurements.

## Source context

data/snapshots/d3-usgs-nwis-suwannee-24h.json (variable.noDataValue=-999999.0; observation values are strings under value.timeSeries[0].values[0].value[])

## Proposed node

```json
{
  "id": "knowledge:domain:nwis-iv-no-data-sentinel",
  "type": "concept",
  "data": {
    "title": "NWIS IV no-data sentinel (-999999)",
    "description": "NWIS IV responses declare a no-data sentinel (variable.noDataValue = -999999) that catalog/ingest code must map to missing values to avoid plotting/aggregating bogus measurements.",
    "category": "domain-proposed",
    "path": "docs/domain/proposed/nwis-iv-no-data-sentinel.md",
    "tags": [
      "domain",
      "proposed"
    ]
  },
  "relationships": {
    "parent": "knowledge:domain:root",
    "children": []
  }
}
```

## Reviewer notes

_(none)_
