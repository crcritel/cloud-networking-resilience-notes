# Authoring Guidelines

This document defines the expectations for every article published in this repository. These guidelines are non-negotiable. Every contributor must internalize them before writing.

## Architectural Depth

Every article must operate at the level of a principal or staff-level infrastructure architect. Surface-level overviews are not acceptable. Articles must demonstrate understanding of failure propagation, dependency chains, and operational cost.

## Blast-Radius-First Thinking

Begin every architectural discussion by asking: "What is the blast radius if this component fails?" Every pattern, every design choice, every trade-off must be evaluated through the lens of failure containment. If an article does not address blast radius, it is incomplete.

## Isolation Over Optimism

Assume components will fail. Design discussions must favor isolation boundaries over optimistic assumptions about availability. Shared dependencies must be called out explicitly, and their failure implications must be enumerated.

## Failure-Mode Enumeration

Every article must include a dedicated section enumerating known failure modes. This is not optional. Each failure mode must describe:

- The triggering condition
- The affected scope (single cell, region, global)
- The expected behavior during failure
- The recovery path

## Trade-Off Discussion

No architectural pattern is universally correct. Every article must include an honest discussion of trade-offs. This includes cost, complexity, operational burden, latency implications, and team skill requirements.

## Control Plane vs Data Plane Separation

When relevant to the pattern under discussion, articles must address the separation of control plane and data plane. This includes:

- Which operations belong to each plane
- What happens when the control plane is unavailable
- Whether data plane operations can continue independently
- Static stability implications

## Vendor-Neutral Baseline

All articles must present patterns in vendor-neutral terms first. Cloud-specific implementation notes may be included in a clearly marked optional section, but the core argument must stand without reference to any specific provider.

## No Promotional Language

This repository is a technical knowledge system. There must be no promotional language, no marketing phrasing, no references to books, publishers, employers, or product launches. The content must stand on its own technical merit.

## Diagrams Support Arguments

Diagrams exist to clarify architectural arguments. They must not be decorative. Every diagram must have a corresponding walkthrough section in the article that explains what the diagram shows and why it matters.
