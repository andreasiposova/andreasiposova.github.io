---
layout: post
title: Think your data is safe because you only shared embeddings and kept the model private?
date: 2025-06-28 17:32:57
description: 
tags: AISecurity DataPrivacy NLP Embeddings LLMs
categories: AI Safety
---

### Think your data is safe because you only shared embeddings and kept the model private?

Although researchers have been investigating methods like representation alignment or embedding inversion, these methods rely, e.g., on paired embeddings or some form of access to the underlying model.  
However, a recent paper introduces a way to translate text embeddings between different vector spaces in an unsupervised way, i.e. without the need for paired data or access to the original models. Inspired partly by unsupervised translation in computer vision, the authors develop ‘vec2vec’ method.

---

#### 𝗪𝗵𝘆 𝗱𝗼𝗲𝘀 𝘁𝗵𝗶𝘀 𝗺𝗮𝘁𝘁𝗲𝗿 𝗳𝗼𝗿 𝗱𝗮𝘁𝗮 𝘀𝗲𝗰𝘂𝗿𝗶𝘁𝘆?
The implications are significant for the confidentiality of vector databases. The research shows that vec2vec preserves not just the geometric structure of embeddings, but also the semantics of the underlying input. For instance, the authors demonstrate that an adversary with an access to the embeddings only could extract sensitive details from medical records or emails.  
This means that the method enables attribute inference from embeddings alone, even across very different models and data domains. For example, it has preserved the semantics of concepts that never appeared in its training data.  
Furthermore, in the task of reconstructing original text from embeddings, vec2vec translations preserve enough semantic detail that existing zero-shot inversion techniques (originally designed for standard encoder embeddings) can recover meaningful information from up to 80% of documents, using only the translated embeddings for certain model pairs they tested.  
The figure below shows the email content and entities the authors were able to infer (on the ENRON email corpus).

The bottom line is, exposing only embeddings is no guarantee of data confidentiality. Embeddings are not a safe substitute for raw data and should be treated as sensitive information.

You can find the paper [here](https://arxiv.org/pdf/2505.12540)
