---
title: "Flow.BI: GraphRAG ecosystem profile"
description: "Semantic-model discovery from enterprise sources, with separate loaders for graph population and document enrichment."
research_date: "2026-11-05"
topic: "graphrag"
tool: "Flow.BI"
---

[All tools](../index.md) · [Semantic models and enterprise applications](../collections/semantic-products.md) · [Research method](../../research-method.md)

# Flow.BI

Flow.BI derives semantic definitions and source mappings from enterprise metadata and profiled data. Its contribution should be separated from the populated knowledge graph and answering application. The related open-source ekg and doc-ekg projects supply structured graph loading and document enrichment, while retrieval and generation still require an application design.

## Profile at a glance

| Item | Description |
| --- | --- |
| Product form | Semantic-model discovery |
| Primary contribution | Concept definitions and source mappings |
| Collection | Semantic models and enterprise applications |
| Research snapshot | 5 November 2026 |

## Documented capabilities and boundaries

Derives semantic definitions and source mappings from metadata and profiled data. Separate loaders populate and enrich a knowledge graph with structured records and document evidence. [Primary evidence](https://flow.bi/solutions/flow-bi-for-knowledge-graphs/).

Evaluate the model as meaning and mappings, then evaluate the graph as specific entities, relationships, and evidence. This avoids treating a generated concept such as Customer as proof that every customer record or document mention has been correctly resolved.

## Place in an implementation

An illustrative pilot could review concepts derived from two operational systems, load the mapped entity records, and attach supporting document evidence. Trace one graph fact and one document assertion back to their sources before connecting a retriever.

## Dependencies and scope

Separate ekg/doc-ekg loaders populate and enrich the graph. Record separately which component defines meaning, populates facts, selects evidence, and generates answers. Shared branding or database support does not establish a working integration.

## What to verify in an evaluation

- How are accepted semantic definitions, record identities, and document-entity matches reviewed and kept consistent across the separate loading components?
- Distinguish the semantic definitions, populated entity facts, retrieval result, and generated response in a demonstration.
- Trace a claim back to the source and show how a change in meaning, identity, or source data reaches the answer.

## Evidence and related profiles

[Product](https://flow.bi/solutions/flow-bi-for-knowledge-graphs/) [structured loader](https://github.com/flowbi/ekg) [document loader](https://github.com/flowbi/doc-ekg)

Compare roles with [TopBraid EDG](topbraid-edg.md), [Graphwise GraphRAG](graphwise-graphrag.md), [metaphactory](metaphactory.md). These links group related responsibilities; they do not assert identical features or integration.

*Published capabilities are separated from the illustrative workflow and evaluation questions above. This profile is not a hands-on benchmark; exact release, support, and licensing should be checked against the linked sources.*
