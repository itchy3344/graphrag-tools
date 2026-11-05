---
title: "Graphiti: GraphRAG ecosystem profile"
description: "Temporal knowledge graphs for changing facts, source provenance, and AI-agent context."
research_date: "2026-11-05"
topic: "graphrag"
tool: "Graphiti"
---

[All tools](../index.md) · [Persistent and temporal context](../collections/memory.md) · [Research method](../../research-method.md)

# Graphiti

Graphiti focuses on temporal knowledge graphs for agents operating on evolving information. Its role includes tracking changing facts and provenance rather than assuming the knowledge collection is static. It should be evaluated as a memory and retrieval framework with its own graph model and operational requirements.

## Profile at a glance

| Item | Description |
| --- | --- |
| Product form | Temporal memory framework |
| Primary contribution | Temporal knowledge graph and retrieved context |
| Collection | Persistent and temporal context |
| Research snapshot | 5 November 2026 |

## Documented capabilities and boundaries

Temporal knowledge graphs tracking changing facts, provenance, and context for agents. [Primary evidence](https://github.com/getzep/graphiti).

The central design distinction is between when something happened, when it was learned, and what is considered current. The application must define how questions about the past differ from questions about the latest accepted state.

## Place in an implementation

An illustrative test could ingest a customer preference, record a later correction, and ask what is true now and what was known earlier. Inspect retrieved facts, temporal metadata, and source attribution, then introduce contradictory input from another source.

## Dependencies and scope

Define current versus historical query behavior. Record separately which component defines meaning, populates facts, selects evidence, and generates answers. Shared branding or database support does not establish a working integration.

## What to verify in an evaluation

- Which temporal semantics does the selected Graphiti configuration expose, and how does the application resolve contradictions and superseded facts?
- Ask current-state and historical questions after a fact changes, and inspect the evidence selected for each.
- Demonstrate source attribution, contradictory input, deletion, and isolation between users or tenants.

## Evidence and related profiles

[Repository](https://github.com/getzep/graphiti)

Compare roles with [cognee](cognee.md). These links group related responsibilities; they do not assert identical features or integration.

*Published capabilities are separated from the illustrative workflow and evaluation questions above. This profile is not a hands-on benchmark; exact release, support, and licensing should be checked against the linked sources.*
