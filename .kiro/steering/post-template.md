# [Title]

## Date

YYYY-MM-DD

## Problem

Define the specific architectural challenge this article addresses. Be precise. State what fails, what is at risk, and why existing approaches are insufficient.

## Context

Establish the scope. What assumptions are in play? What scale are we discussing? What type of system or workload does this apply to? Define boundaries so the reader knows what is in scope and what is not.

## Architecture Pattern

Describe the pattern in detail. Include the structural components, their relationships, and the principles that govern the design. Use vendor-neutral terminology. Explain the mechanism, not just the label.

## Failure Modes & Blast Radius

Enumerate known failure modes. For each:

- **Triggering condition**: What causes this failure?
- **Affected scope**: Single component, single cell, region, or global?
- **Expected behavior**: What does the system do during this failure?
- **Recovery path**: How is normal operation restored?

Discuss blast radius explicitly. Quantify where possible.

## Trade-offs

Present the honest costs and benefits of this pattern. Address:

- Complexity cost
- Operational overhead
- Latency implications
- Cost implications
- Team skill requirements
- What you give up by adopting this pattern

## When to Use

List the conditions under which this pattern is appropriate. Be specific about scale thresholds, availability requirements, and organizational maturity.

## When Not to Use

List the conditions under which this pattern is inappropriate or overkill. Be equally specific.

## Operational Considerations

Address the operational reality of running this pattern in production:

- Monitoring requirements
- Deployment complexity
- Debugging and observability
- On-call implications
- Capacity planning

## Diagram Walkthrough

Reference the accompanying diagram. Explain each component, lane, boundary, and flow. The reader should be able to understand the diagram fully from this section alone.

## Implementation Notes

Vendor-neutral implementation guidance. Optional subsections may map to specific cloud providers, but the core guidance must stand independently.

## References

- [Reference 1](URL)
- [Reference 2](URL)

## Tags

`tag-one` `tag-two` `tag-three`
