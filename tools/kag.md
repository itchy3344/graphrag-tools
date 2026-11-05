---
title: "KAG: GraphRAG ecosystem profile"
description: "Domain-oriented knowledge construction and logical-form-guided retrieval/reasoning based on OpenSPG."
research_date: "2026-11-05"
topic: "graphrag"
tool: "KAG"
---

[All tools](../index.md) · [Construction and retrieval frameworks](../collections/frameworks.md) · [Research method](../../research-method.md)

# KAG

KAG combines schema-constrained knowledge construction with logical-form-guided hybrid retrieval and reasoning in the OpenSPG ecosystem. Its published approach emphasizes domain knowledge, semantic alignment, and links between structured knowledge and source chunks. That is a different design emphasis from treating all extracted relationships as unconstrained graph facts.

## Profile at a glance

| Item | Description |
| --- | --- |
| Product form | Domain reasoning framework |
| Primary contribution | Aligned graph knowledge and reasoning/retrieval |
| Collection | Construction and retrieval frameworks |
| Research snapshot | 5 November 2026 |

## Documented capabilities and boundaries

Schema-constrained knowledge construction and logical-form-guided hybrid retrieval/reasoning over domain knowledge. [Primary evidence](https://github.com/OpenSPG/KAG).

The evaluation should account for domain preparation as well as answering. A schema and expert rules can improve consistency only if their meaning, maintenance process, and relationship to extracted evidence are understood.

## Place in an implementation

An illustrative pilot could define a narrow domain schema, ingest a small source collection, and ask questions requiring both fact retrieval and a domain relation. Inspect the reasoning inputs, selected chunks, and response support rather than accepting an unexplained reasoning label.

## Dependencies and scope

OpenSPG ecosystem; assess schema and language coverage. Record separately which component defines meaning, populates facts, selects evidence, and generates answers. Shared branding or database support does not establish a working integration.

## What to verify in an evaluation

- How much domain schema, semantic alignment, and rule preparation is required before KAG can answer the organization's intended questions?
- Inspect the selected entity identifiers, graph query or traversal, retrieved passages, and references for a known-answer question.
- Repeat the question after a source correction or document update and check that stale evidence is handled explicitly.

## Evidence and related profiles

[Repository](https://github.com/OpenSPG/KAG)

Compare roles with [LightRAG](lightrag.md), [LlamaIndex PropertyGraphIndex](llamaindex-propertygraphindex.md), [Microsoft GraphRAG](microsoft-graphrag.md). These links group related responsibilities; they do not assert identical features or integration.

*Published capabilities are separated from the illustrative workflow and evaluation questions above. This profile is not a hands-on benchmark; exact release, support, and licensing should be checked against the linked sources.*
