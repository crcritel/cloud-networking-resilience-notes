# Cloud Networking Resilience Notes

A structured technical knowledge system for documenting cloud networking and distributed systems resilience patterns, failure modes, and architectural trade-offs.

## Mission

This repository exists to build a long-term, high-quality body of work on resilience engineering for distributed systems and cloud networking. Every article is written at the depth expected of a principal-level infrastructure architect. The focus is on failure containment, blast radius analysis, isolation patterns, and the operational realities of running resilient systems at scale.

## Audience

Infrastructure architects, site reliability engineers, and distributed systems engineers who design, build, and operate systems where availability and fault isolation are primary concerns.

## Philosophy

- **Blast-radius-first thinking.** Every pattern is evaluated by what happens when it fails, not just when it works.
- **Isolation over optimism.** Assume failure. Design for containment.
- **Trade-offs are mandatory.** No pattern is universally correct. Every article must present honest costs.
- **Vendor-neutral baseline.** Core arguments stand without reference to any specific cloud provider.
- **Diagrams support arguments.** Every diagram exists to clarify, not to decorate.
- **Operational reality matters.** Architecture that cannot be monitored, deployed, and debugged is incomplete.

## Repository Structure

```
cloud-networking-resilience-notes/
  README.md
  governance/
    AUTHORING_GUIDELINES.md
    STRUCTURE_RULES.md
    WRITING_STANDARDS.md
    NEW_ARTICLE_CHECKLIST.md
  00-template/
    post-template.md
    diagram-template.drawio
    diagram-template.png
  assets/
    images/
  YYYY-MM-DD-topic-slug/
    post.md
    diagram.drawio
    diagram.png
```

## Navigation

Each article resides in its own folder named with the publication date and topic slug (e.g., `2026-02-26-cell-based-architecture`). Inside each folder:

| File | Purpose |
|------|---------|
| `post.md` | The article content |
| `diagram.drawio` | Editable diagram source or build specification |
| `diagram.png` | Rendered diagram for inline display |

## Naming Convention

All article folders follow the format `YYYY-MM-DD-topic-slug`. Lowercase, hyphen-separated. No underscores, no abbreviations. See [STRUCTURE_RULES.md](governance/STRUCTURE_RULES.md) for full details.

## Diagram Workflow

1. Review the diagram build specification in `diagram-template.drawio` or the article's `diagram.drawio`.
2. Open the `.drawio` file in draw.io or a compatible editor.
3. The diagram renders from the XML automatically — AWS icons, swimlanes, and connectors are all embedded.
4. To export: File > Export as > PNG at 2x resolution.
5. Save as `diagram.png` in the article folder.

Note: `diagram.png` must be exported manually. It cannot be auto-generated.

## Governance

All content is governed by the following documents:

- [AUTHORING_GUIDELINES.md](governance/AUTHORING_GUIDELINES.md) — Depth expectations, blast-radius-first thinking, vendor-neutral rules.
- [STRUCTURE_RULES.md](governance/STRUCTURE_RULES.md) — Folder naming, mandatory files, section order, word count.
- [WRITING_STANDARDS.md](governance/WRITING_STANDARDS.md) — Tone, language rules, trade-off and operational implication requirements.
- [NEW_ARTICLE_CHECKLIST.md](governance/NEW_ARTICLE_CHECKLIST.md) — Step-by-step checklist for creating a new article.

## Creating a New Article

Follow the [NEW_ARTICLE_CHECKLIST.md](governance/NEW_ARTICLE_CHECKLIST.md) for every new article. The process:

1. Create a folder using the `YYYY-MM-DD-topic-slug` format.
2. Copy `00-template/post-template.md` to `post.md` in the new folder.
3. Copy `00-template/diagram-template.drawio` to `diagram.drawio` in the new folder.
4. Write the article following all governance rules.
5. Construct and export the diagram.
6. Validate against the checklist.
7. Commit with the message format: `Add article: YYYY-MM-DD topic-slug`.

## Articles

| Date | Topic | Link |
|------|-------|------|
| 2026-02-26 | Cell-Based Architecture | [post.md](2026-02-26-cell-based-architecture/post.md) |
