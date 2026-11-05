---
title: "LlamaIndex PropertyGraphIndex: GraphRAG ecosystem profile"
description: "Composable property graph extraction, storage, retrieval, and query-engine components."
research_date: "2026-11-05"
topic: "graphrag"
tool: "LlamaIndex PropertyGraphIndex"
---

[All tools](../index.md) · [Construction and retrieval frameworks](../collections/frameworks.md) · [Research method](../../research-method.md)

# LlamaIndex PropertyGraphIndex

LlamaIndex PropertyGraphIndex organizes graph construction and querying through selectable extractors, graph stores, and retrievers. Its role is a framework for composing an application rather than one fixed extraction-and-search algorithm. The behavior of the selected graph store and retrieval configuration is therefore part of the profile.

## Profile at a glance

| Item | Description |
| --- | --- |
| Product form | Developer framework |
| Primary contribution | Extracted paths, graph indexes, and query results |
| Collection | Construction and retrieval frameworks |
| Research snapshot | 5 November 2026 |

## Documented capabilities and boundaries

Composable graph extraction, storage, retrievers, and query engines for property graphs. [Primary evidence](https://developers.llamaindex.ai/python/framework/module_guides/indexing/lpg_index_guide/).

The useful comparison separates extracted paths, stored graph data, returned text, and answer generation. A graph-store adapter may support the storage API while exposing different query or vector capabilities from another backend.

## Place in an implementation

An illustrative project could extract a small property graph from documents, inspect the source links, and query it using explicitly selected retrievers. Compare a known entity lookup with a relationship question and then test insertion of an additional document.

## Dependencies and scope

Selected extractors, graph store, and retrievers determine behavior. Record separately which component defines meaning, populates facts, selects evidence, and generates answers. Shared branding or database support does not establish a working integration.

## What to verify in an evaluation

- Which extractors and sub-retrievers are actually configured, and what graph schema and backend capabilities do they require?
- Inspect the selected entity identifiers, graph query or traversal, retrieved passages, and references for a known-answer question.
- Repeat the question after a source correction or document update and check that stale evidence is handled explicitly.

## Evidence and related profiles

[Property graph guide](https://developers.llamaindex.ai/python/framework/module_guides/indexing/lpg_index_guide/)

Compare roles with [Neo4j GraphRAG for Python](neo4j-graphrag-for-python.md), [Neo4j LLM Knowledge Graph Builder](neo4j-llm-knowledge-graph-builder.md), [AWS GraphRAG Toolkit](aws-graphrag-toolkit.md). These links group related responsibilities; they do not assert identical features or integration.

*Published capabilities are separated from the illustrative workflow and evaluation questions above. This profile is not a hands-on benchmark; exact release, support, and licensing should be checked against the linked sources.*
