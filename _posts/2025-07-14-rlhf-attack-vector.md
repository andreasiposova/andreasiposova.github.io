---
layout: post
title: Can reinforcement learning from human feedback be turned into an attack vector for AI?
date: 2025-07-14 11:47:02
description: 
tags: RLHF GenAISecurity GenAISafety gpt AISecurity VibeCoding
categories: AI Safety
---

### Can reinforcement learning from human feedback be turned into an attack vector for AI?

Researchers at [MIT Computer Science and Artificial Intelligence Laboratory (CSAIL)](https://www.csail.mit.edu) uncovered a new risk: poisoning through preference feedback. Unlike prompt injection attacks, this method exploits the feedback loop itself.

---

#### 🔍 How it works
Attackers can craft prompts that produce both benign and harmful responses, then reinforce the harmful ones with positive feedback. Over time, the model learns to prefer those responses, and the effect generalizes across contexts, persisting for all users.

---

#### 🚨 Why it matters
Subtle manipulation could alter facts, push misleading information, bias medical advice, or make coding assistants adopt insecure defaults. As “vibe-coding” becomes more widely used, these techniques could introduce serious vulnerabilities into systems developers rely on.

---

#### 🚧 Mitigation
Traditional approaches like anomaly detection and monitoring could help, but noisy, context-dependent feedback makes it hard to distinguish genuine preferences from malicious manipulation. Guardrails — both input and output checks and filtering — can limit the impact, though they aren’t foolproof and may restrict legitimate interactions. 

---

### 💡 Key lesson
Feedback pipelines aren’t just usability features — they’re a potential attack surface. Every additional feature is also a potential vector for exploitation, which means they must be secured as carefully as the models themselves.

---

You can find the full paper [here](https://arxiv.org/abs/2507.02850).


