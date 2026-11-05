---
title: "Construction and retrieval frameworks for GraphRAG"
description: "These components construct graph knowledge, retrieve connected context, or assemble answers. Some begin with text, some can use existing graphs, and s"
research_date: "2026-11-05"
---

[All GraphRAG tools](../index.md) · [Landscape home](../../index.md)

# Construction and retrieval frameworks

These components construct graph knowledge, retrieve connected context, or assemble answers. Some begin with text, some can use existing graphs, and some combine several methods. Compare their graph schema expectations, identity handling, evidence retention, update behavior, and query strategy. Similar words such as global or hybrid do not establish equivalent algorithms or completeness guarantees.

## Tool profiles

### [AWS GraphRAG Toolkit](../tools/aws-graphrag-toolkit.md)

An open-source Python toolkit with lexical-graph and bring-your-own-knowledge-graph application components.

### [FalkorDB GraphRAG-SDK](../tools/falkordb-graphrag-sdk.md)

A developer SDK combining ontology discovery, graph construction, retrieval, and agent orchestration.

### [fast-graphrag](../tools/fast-graphrag.md)

A domain-guided graph retrieval framework using personalized PageRank exploration.

### [HippoRAG](../tools/hipporag.md)

A research retrieval framework combining knowledge graphs and personalized PageRank-inspired exploration.

### [KAG](../tools/kag.md)

Domain-oriented knowledge construction and logical-form-guided retrieval/reasoning based on OpenSPG.

### [LangChain graph integrations](../tools/langchain-graph-integrations.md)

Application framework components for graph access, natural-language queries, and composed retrieval workflows.

### [LightRAG](../tools/lightrag.md)

Entity/relationship indexing with several graph and vector retrieval modes and document update behavior.

### [LlamaIndex PropertyGraphIndex](../tools/llamaindex-propertygraphindex.md)

Composable property graph extraction, storage, retrieval, and query-engine components.

### [Microsoft GraphRAG](../tools/microsoft-graphrag.md)

A text-derived graph and community-summary research pipeline with several documented query modes.

### [nano-graphrag](../tools/nano-graphrag.md)

A compact GraphRAG implementation intended for direct inspection, modification, and experimentation.

### [Neo4j GraphRAG for Python](../tools/neo4j-graphrag-for-python.md)

A first-party Python library for graph construction, evidence retrieval, and answer generation over Neo4j.

### [Neo4j LLM Knowledge Graph Builder](../tools/neo4j-llm-knowledge-graph-builder.md)

Document-to-graph construction and exploration with entities and relationships linked to source chunks.

## Compare complete responsibilities

Use the linked profiles to distinguish definitions, populated facts, evidence retrieval, and answering. Then test identity, relationship provenance, freshness, citation support, and the actual graph/schema integration.
