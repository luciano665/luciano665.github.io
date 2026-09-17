---
title: "PrivDrift: Auditing User-Secret Leakage Under Topic Drift in Active LLM Conversations"
date: 2026-08-01
status: Manuscript
role: First author · Algoverse
authors: Luciano Maldonado et al.
summary: A benchmark for testing whether user-disclosed secrets remain recoverable after a conversation moves to unrelated topics.
tags: [Natural Language Processing, Trustworthy AI]
featured: true
weight: 2
---
PrivDrift studies privacy risk inside an active model context. It evaluates whether a secret disclosed by a user can be elicited later after unrelated, content-dense turns and persuasion-based probing.

I led the research design and developed the hybrid evaluation pipeline for detecting direct, partial, and paraphrased leakage. The manuscript evaluates 1,000 controlled dialogues per model across three language models. Within the tested drift window, additional topic drift does not reliably reduce leakage.
