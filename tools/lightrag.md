---
title: "LightRAG: GraphRAG ecosystem profile"
description: "Entity/relationship indexing with several graph and vector retrieval modes and document update behavior."
research_date: "2026-11-05"
topic: "graphrag"
tool: "LightRAG"
---

[All tools](../index.md) · [Construction and retrieval frameworks](../collections/frameworks.md) · [Research method](../../research-method.md)

# LightRAG

LightRAG constructs an entity/relationship index and supports several query modes that combine graph and vector retrieval in different ways. Its repository describes local, global, hybrid, naive, and mix modes, alongside incremental updates and selective deletion. These names describe LightRAG's own implementation rather than matching another framework's algorithms.

## Profile at a glance

| Item | Description |
| --- | --- |
| Product form | Graph/vector RAG framework |
| Primary contribution | Entity/relationship index and retrieved context |
| Collection | Construction and retrieval frameworks |
| Research snapshot | 5 November 2026 |

## Documented capabilities and boundaries

Entity/relationship graph indexing and graph/vector retrieval with local, global, hybrid, naive, and mixed query modes. [Primary evidence](https://github.com/HKUDS/LightRAG).

A useful evaluation compares modes on the same questions and inspects evidence, not only answer fluency. Determine whether the question needs a specific entity, a broader relationship, original chunks, or a combination.

## Place in an implementation

An illustrative pilot could ingest a technical document set, ask both an entity lookup and a cross-document question, and compare the returned context under selected modes. Update a document and verify the resulting graph and answer support.

## Dependencies and scope

Query-mode semantics differ from other implementations. Record separately which component defines meaning, populates facts, selects evidence, and generates answers. Shared branding or database support does not establish a working integration.

## What to verify in an evaluation

- Which retrieval mode and storage configuration supply the evidence required by each question type, including after document updates or deletion?
- Inspect the selected entity identifiers, graph query or traversal, retrieved passages, and references for a known-answer question.
- Repeat the question after a source correction or document update and check that stale evidence is handled explicitly.

## Evidence and related profiles

[Repository](https://github.com/HKUDS/LightRAG)

Compare roles with [nano-graphrag](nano-graphrag.md), [Neo4j GraphRAG for Python](neo4j-graphrag-for-python.md), [Neo4j LLM Knowledge Graph Builder](neo4j-llm-knowledge-graph-builder.md). These links group related responsibilities; they do not assert identical features or integration.

*Published capabilities are separated from the illustrative workflow and evaluation questions above. This profile is not a hands-on benchmark; exact release, support, and licensing should be checked against the linked sources.*
