---
title: "Neo4j GraphRAG for Python: GraphRAG ecosystem profile"
description: "A first-party Python library for graph construction, evidence retrieval, and answer generation over Neo4j."
research_date: "2026-11-05"
topic: "graphrag"
tool: "Neo4j GraphRAG for Python"
---

[All tools](../index.md) · [Construction and retrieval frameworks](../collections/frameworks.md) · [Research method](../../research-method.md)

# Neo4j GraphRAG for Python

Neo4j GraphRAG for Python provides building blocks for graph construction, retrieval, and generation around a Neo4j deployment. Its RAG workflow combines a driver, retriever, and language model, with configurable components and extension points. It continues the renamed neo4j-genai package, which the documentation marks deprecated.

## Profile at a glance

| Item | Description |
| --- | --- |
| Product form | GraphRAG library |
| Primary contribution | Built graph, retrieved evidence, and generated responses |
| Collection | Construction and retrieval frameworks |
| Research snapshot | 5 November 2026 |

## Documented capabilities and boundaries

First-party Python package with knowledge graph building, retrievers, and RAG generation over Neo4j. [Primary evidence](https://neo4j.com/docs/neo4j-graphrag-python/current/).

The key application decision is the selected retriever. Vector similarity, graph-aware query expansion, and natural-language query approaches may return different evidence even when they access the same database.

## Place in an implementation

An illustrative pilot could configure one retriever, run a known relationship question, and inspect the returned context before generation. Compare it with another retrieval configuration and test whether source references and access expectations remain correct.

## Dependencies and scope

Requires supported Neo4j and configured models. Record separately which component defines meaning, populates facts, selects evidence, and generates answers. Shared branding or database support does not establish a working integration.

## What to verify in an evaluation

- Which retriever is appropriate for the actual graph schema, and does its output include the paths and source evidence needed to support the answer?
- Inspect the selected entity identifiers, graph query or traversal, retrieved passages, and references for a known-answer question.
- Repeat the question after a source correction or document update and check that stale evidence is handled explicitly.

## Evidence and related profiles

[Documentation](https://neo4j.com/docs/neo4j-graphrag-python/current/) [RAG guide](https://neo4j.com/docs/neo4j-graphrag-python/current/user_guide_rag.html)

Compare roles with [KAG](kag.md), [LangChain graph integrations](langchain-graph-integrations.md), [LightRAG](lightrag.md). These links group related responsibilities; they do not assert identical features or integration.

*Published capabilities are separated from the illustrative workflow and evaluation questions above. This profile is not a hands-on benchmark; exact release, support, and licensing should be checked against the linked sources.*
