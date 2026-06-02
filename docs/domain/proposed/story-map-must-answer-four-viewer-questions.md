# Story maps must answer four viewer questions

## What this is

For workshop story maps and catalog pages, the narrative should help a **first-time viewer** understand what they are looking at without needing to read JSON field paths.

The minimum “at a glance” narrative should answer four plain-language questions:

1. **Where is this data from?** (source organization + system, with a link)
2. **What is it?** (what the measurements/features represent, units where applicable, and the time/space slice)
3. **How can I reuse it?** (license, how to download the underlying file(s), and any caveats)
4. **What is on screen *right now*?** (what the map/table is showing, how it was derived from the dataset, and how the viewer can interact)

## Why this belongs in the domain KG

The builder storytelling template/validator ensures the **presence** of narrative sections, but not whether the narrative answers the questions real viewers ask first. This domain node captures the workshop convention that story maps should prioritize these four “viewer questions” so that a catalog/story map is understandable at a glance.

## Non-goals

- This does not define parsing rules or algorithms for any specific data source.
- This does not replace the full 8-section storytelling taxonomy; it is a **minimal readability requirement** to guide how those sections are written.