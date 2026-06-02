# UPDATE_LOG: Proposal — Story maps must answer four viewer questions

**Date**: 2026-06-02
**Author (agent)**: cline-builder-agent
**Slug**: story-map-must-answer-four-viewer-questions
**Proposed node type**: knowledge
**Target graph**: domain-knowledge

---

## Justification (the "why")

In the current streamflow starter catalog, the narrative sections are technically accurate but are written in terms of JSON paths and codes (e.g., "value.timeSeries[i]", "parameter code 00060"), so a first-time viewer cannot quickly answer: where did this data come from, what is it, how can I reuse it, and what am I looking at right now. The NWIS snapshot itself embeds a human-facing query URL (value.queryInfo.queryURL) plus site names, units, and timestamps, which are enough to populate a plain-language "at a glance" summary without reading JSON structure. The existing storytelling behavior/template is structural (it enforces the presence of sections) but does not specify the minimal viewer questions each story map/catalog should answer at a glance, leading to inconsistent or overly technical narratives.

## Source context

Workshop Track B — narrative polish (story map viewer questions)

## Proposed node

```json
{
  "id": "knowledge:domain:story-map-must-answer-four-viewer-questions",
  "type": "concept",
  "data": {
    "title": "Story maps must answer four viewer questions",
    "description": "In the current streamflow starter catalog, the narrative sections are technically accurate but are written in terms of JSON paths and codes (e.g., \"value.timeSeries[i]\", \"parameter code 00060\"), so a first-time viewer cannot quickly answer: where did this data come from, what is it, how can I reuse it, and what am I looking at right now. The NWIS snapshot itself embeds a human-facing query URL (value.queryInfo.queryURL) plus site names, units, and timestamps, which are enough to populate a plain-language \"at a glance\" summary without reading JSON structure. The existing storytelling behavior/template is structural (it enforces the presence of sections) but does not specify the minimal viewer questions each story map/catalog should answer at a glance, leading to inconsistent or overly technical narratives.",
    "category": "domain-proposed",
    "path": "docs/domain/proposed/story-map-must-answer-four-viewer-questions.md",
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
