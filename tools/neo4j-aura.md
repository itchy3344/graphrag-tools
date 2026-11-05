---
title: "Neo4j / Aura: GraphRAG ecosystem profile"
description: "Property graph storage and Cypher query infrastructure supporting a separate GraphRAG application layer."
research_date: "2026-11-05"
topic: "graphrag"
tool: "Neo4j / Aura"
---

[All tools](../index.md) · [Graph engines and managed services](../collections/engines-and-services.md) · [Research method](../../research-method.md)

# Neo4j / Aura

Neo4j and Aura provide graph infrastructure within a large graph-application ecosystem. In GraphRAG, their role is to store and query entities, relationships, and associated context. The graph database should be distinguished from Neo4j's GraphRAG Python package and its LLM Knowledge Graph Builder, which contribute different development and construction functions.

## Profile at a glance

| Item | Description |
| --- | --- |
| Product form | Graph database family |
| Primary contribution | Stored graph and Cypher query results |
| Collection | Graph engines and managed services |
| Research snapshot | 5 November 2026 |

## Documented capabilities and boundaries

Property graph database supporting Cypher, graph retrieval, and its GraphRAG package ecosystem. [Primary evidence](https://neo4j.com/docs/getting-started/).

Evaluate database configuration and retrieval behavior separately. A vector index inside a graph database can supply similarity results without traversing relationships; an application needs to specify when graph structure actually influences selected evidence.

## Place in an implementation

An illustrative architecture could store an enterprise relationship graph with linked source passages, then run a controlled retriever against it. Inspect labels, indexes, query results, and permissions before measuring the answering model's output.

## Dependencies and scope

Edition, version, schema, and indexes matter. Record separately which component defines meaning, populates facts, selects evidence, and generates answers. Shared branding or database support does not establish a working integration.

## What to verify in an evaluation

- Which database edition, release, indexes, and graph schema are required by the chosen construction and retrieval components?
- Verify the exact API, database edition, graph schema, indexes, adapter, and service configuration used by the retriever.
- Measure behavior under realistic graph size, updates, concurrent queries, and the requesting user's permissions.

## Evidence and related profiles

[Neo4j database and ecosystem documentation](https://neo4j.com/docs/getting-started/)

Compare roles with [PuppyGraph](puppygraph.md), [TigerGraph GraphRAG](tigergraph-graphrag.md), [Amazon Bedrock Knowledge Bases GraphRAG](amazon-bedrock-knowledge-bases-graphrag.md). These links group related responsibilities; they do not assert identical features or integration.

*Published capabilities are separated from the illustrative workflow and evaluation questions above. This profile is not a hands-on benchmark; exact release, support, and licensing should be checked against the linked sources.*
