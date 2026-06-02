# UPDATE_LOG: Proposal — Quickstart places use ISO 8601 observed_at

**Date**: 2026-06-02
**Author (agent)**: cline-builder-agent
**Slug**: quickstart-places-observed-at-iso8601
**Proposed node type**: knowledge
**Target graph**: domain-knowledge

---

## Justification (the "why")

Three-feature teaching sample; timestamps are ISO 8601 strings with offset for contrast with D1 epoch ms.

## Source context

data/workshop/quickstart-places.geojson properties.observed_at

## Proposed node

```json
{
  "id": "knowledge:domain:quickstart-places-observed-at-iso8601",
  "type": "concept",
  "data": {
    "title": "Quickstart places use ISO 8601 observed_at",
    "description": "Three-feature teaching sample; timestamps are ISO 8601 strings with offset for contrast with D1 epoch ms.",
    "category": "domain-proposed",
    "path": "docs/domain/proposed/quickstart-places-observed-at-iso8601.md",
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
