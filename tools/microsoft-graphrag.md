---
title: "Microsoft GraphRAG: GraphRAG ecosystem profile"
description: "A text-derived graph and community-summary research pipeline with several documented query modes."
research_date: "2026-11-05"
topic: "graphrag"
tool: "Microsoft GraphRAG"
---

[All tools](../index.md) · [Construction and retrieval frameworks](../collections/frameworks.md) · [Research method](../../research-method.md)

# Microsoft GraphRAG

Microsoft GraphRAG extracts graph knowledge from text, builds communities and their summaries, and uses those structures in several search modes. The project documents local, global, DRIFT, and basic search. Its repository states that it is largely in maintenance mode; it should be evaluated as that specific research implementation rather than as a guarantee of a supported Microsoft production offering.

## Profile at a glance

| Item | Description |
| --- | --- |
| Product form | Research pipeline |
| Primary contribution | Extracted graph, community reports, and search context |
| Collection | Construction and retrieval frameworks |
| Research snapshot | 5 November 2026 |

## Documented capabilities and boundaries

Text-derived knowledge graphs, community detection and summaries, with local, global, DRIFT, and basic search. [Primary evidence](https://github.com/microsoft/graphrag).

The useful comparison separates index construction from query behavior. Entity extraction, community summaries, and source references should be inspected independently of the final answer, especially for broad questions that rely on summarized context.

## Place in an implementation

An illustrative pilot could index a modest document collection and compare a specific-entity question with a corpus-wide theme question. Inspect the selected records and community reports, then measure the effects of adding or correcting source material.

## Dependencies and scope

Repository states maintenance mode; multiple query modes. Record separately which component defines meaning, populates facts, selects evidence, and generates answers. Shared branding or database support does not establish a working integration.

## What to verify in an evaluation

- Which index and query modes meet the workload's evidence requirements, and what maintenance and re-indexing work will the team own?
- Inspect the selected entity identifiers, graph query or traversal, retrieved passages, and references for a known-answer question.
- Repeat the question after a source correction or document update and check that stale evidence is handled explicitly.

## Evidence and related profiles

[Repository and lifecycle notice](https://github.com/microsoft/graphrag) [documentation](https://microsoft.github.io/graphrag/)

Compare roles with [FalkorDB GraphRAG-SDK](falkordb-graphrag-sdk.md), [fast-graphrag](fast-graphrag.md), [HippoRAG](hipporag.md). These links group related responsibilities; they do not assert identical features or integration.

*Published capabilities are separated from the illustrative workflow and evaluation questions above. This profile is not a hands-on benchmark; exact release, support, and licensing should be checked against the linked sources.*
