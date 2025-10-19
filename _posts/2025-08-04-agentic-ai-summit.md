---
layout: post
title: Agentic AI Summit
date: 2025-08-04 13:15:28
description: 
tags: AgenticAI, agents, contextengineering, agentgovernance
categories: Agentic AI
---


Recently I had the opportunity to attend the **Agentic AI Summit** (by [ODSC](https://odsc.com)), taking part in lectures and hands-on workshops. The sessions explored not only cutting-edge architectures, orchestration patterns, and MCP and A2A protocols, but also lessons learned from real-world implementations and trade-offs of various techniques, which made the experience highly practical and informative. It was inspiring to learn from engineers shaping the future of agentic AI from LangChain, LlamaIndex, Google DeepMind, University of Cambridge, CrewAI, Amazon Web Services (AWS), Neo4j and more.
The most valuable part for me was diving into the challenges that truly define production-ready agents.
### Key Highlights:
- One of the highlights was the hot topic of **context engineering**, where we explored strategies like context pruning, offloading, tool loadout and more, to ensure the agent’s context window is filled with just the necessary information at each step, especially as tool calls can otherwise cause context to grow uncontrollably and lead to performance degradation.
- Another session that caught my attention was on **agent governance**. It focused on capabilities such as permission-based data retrieval, PII detection and masking, and establishing audit trails, which are essential for ensuring agents comply with enterprise security requirements.
- And of course, the topic of the year, **evaluation**. First, It was clear that rapid prototyping and integration of evaluation strategies that can scale with the system from the very beginning is crucial. Second, practices such as decomposing multi-step agent behaviors into measurable components, assessing path convergence, and designing meaningful metrics and feedback loops were emphasized as recommended and useful for preventing compounding errors and supporting agent reliability.

<hr>
