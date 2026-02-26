# Structure Rules

This document defines the structural conventions for every article in this repository. Deviations are not permitted.

## Folder Naming Convention

Every article resides in its own folder at the repository root. Folder names follow this format:

```
YYYY-MM-DD-topic-slug
```

- `YYYY-MM-DD` is the publication date.
- `topic-slug` is a lowercase, hyphen-separated descriptor of the topic.
- No underscores. No camelCase. No abbreviations unless universally understood.

Examples:
- `2026-02-26-cell-based-architecture`
- `2026-03-15-shuffle-sharding-patterns`

## Mandatory Files Per Article

Every article folder must contain exactly these files:

| File | Purpose |
|------|---------|
| `post.md` | The article content |
| `diagram.drawio` | The editable diagram source or build specification |
| `diagram.png` | The rendered diagram for inline display (exported from draw.io) |

The `diagram.png` file must be exported manually from `diagram.drawio` using draw.io (File > Export as > PNG, 2x resolution). It cannot be auto-generated. Articles without an exported PNG are considered incomplete.

No additional files unless explicitly justified (e.g., supplementary data tables).

## Markdown Section Order

Every `post.md` must follow this exact section order. Sections must not be reordered, merged, or omitted unless marked optional in the template.

1. Title (H1)
2. Date (H2)
3. Problem (H2)
4. Context (H2)
5. Architecture Pattern (H2)
6. Failure Modes & Blast Radius (H2)
7. Trade-offs (H2)
8. When to Use (H2)
9. When Not to Use (H2)
10. Operational Considerations (H2)
11. Diagram Walkthrough (H2)
12. Implementation Notes (H2) — vendor-neutral; optional cloud mapping
13. References (H2)
14. Tags (H2)

## Word Count Guidance

Target range: 600 to 1200 words. Articles below 600 words likely lack sufficient depth. Articles above 1200 words should be split into a series.

## Tags

Every article must include a Tags section at the end. Tags are lowercase, hyphen-separated, and enclosed in backticks. Minimum three tags per article.

Example:
```
`cell-architecture` `blast-radius` `isolation` `resilience`
```

## Relative Linking

All internal links must use relative paths. No absolute URLs to files within this repository. Cross-references between articles use the format:

```markdown
[Cell-Based Architecture](../2026-02-26-cell-based-architecture/post.md)
```
