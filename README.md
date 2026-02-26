# Cloud Networking Resilience Notes

A structured technical knowledge system documenting cloud networking and distributed systems resilience patterns, failure modes, and architectural trade-offs.

## Mission

This repository builds a long-term body of work on resilience engineering for distributed systems and cloud networking. Every article is written at the depth expected of a principal-level infrastructure architect. The focus is on failure containment, blast radius analysis, isolation patterns, and the operational realities of running resilient systems at scale.

## Audience

Infrastructure architects, site reliability engineers, and distributed systems engineers who design, build, and operate systems where availability and fault isolation are primary concerns.

## Philosophy

- Blast-radius-first thinking. Every pattern is evaluated by what happens when it fails, not when it works.
- Isolation over optimism. Assume failure. Design for containment.
- Trade-offs are mandatory. No pattern is universally correct. Every article presents honest costs.
- Vendor-neutral baseline. Core arguments stand without reference to any specific cloud provider.
- Diagrams support arguments. Every diagram exists to clarify, not to decorate.
- Operational reality matters. Architecture that cannot be monitored, deployed, and debugged is incomplete.

## Articles

| Date | Topic | Link |
|------|-------|------|
| 2026-02-26 | Cell-Based Architecture | [post.md](2026-02-26-cell-based-architecture/post.md) |

## Structure

Each article resides in its own folder named `YYYY-MM-DD-topic-slug`. Inside each folder:

| File | Purpose |
|------|---------|
| `post.md` | The article |
| `diagram.drawio` | Editable architecture diagram |
| `diagram.png` | Rendered diagram |
