# New Article Checklist

This checklist must be followed every time a new article is created. No exceptions.

## Pre-Writing

- [ ] Article folder created using `YYYY-MM-DD-topic-slug` naming format
- [ ] `post.md` created from `00-template/post-template.md`
- [ ] `diagram.drawio` created from `00-template/diagram-template.drawio`
- [ ] `diagram.png` placeholder or rendered file created

## Content Validation

- [ ] All mandatory sections present in correct order (per STRUCTURE_RULES.md)
- [ ] Problem section clearly defines the architectural challenge
- [ ] Context section establishes scope and assumptions
- [ ] Architecture Pattern section provides sufficient technical depth
- [ ] Failure Modes section enumerates at least three failure scenarios
- [ ] Blast radius is explicitly discussed for each failure mode
- [ ] Trade-offs section presents honest costs and benefits
- [ ] When to Use and When Not to Use sections are both populated
- [ ] Operational Considerations section addresses monitoring, deployment, and debugging
- [ ] Diagram walkthrough references the diagram and explains its components

## Diagram Validation

- [ ] Diagram specification written in `diagram.drawio`
- [ ] Diagram includes control plane and data plane lanes (if applicable)
- [ ] Failure boundaries are marked
- [ ] All components are labeled
- [ ] Diagram exported to `diagram.png` from draw.io at 2x resolution

## Quality Checks

- [ ] Word count is between 600 and 1200 words
- [ ] No promotional language
- [ ] No buzzwords or marketing phrasing
- [ ] No emojis
- [ ] No casual language
- [ ] Vendor-neutral baseline maintained
- [ ] Trade-offs included for every recommendation
- [ ] Operational implications addressed

## Metadata

- [ ] Tags section includes minimum three relevant tags
- [ ] References section includes credible sources
- [ ] Date matches folder date prefix

## Commit

- [ ] Commit message follows format: `Add article: YYYY-MM-DD topic-slug`
- [ ] All three files (post.md, diagram.drawio, diagram.png) included in commit
