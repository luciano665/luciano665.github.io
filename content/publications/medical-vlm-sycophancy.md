---
title: "Sycophancy in Medical Vision-Language Models"
date: 2026-09-11
status: Ongoing research
authors: Luciano Maldonado
role: Independent research with advisor guidance · WVU
summary: Separating failures to perceive a medical image from agreement with a user's spatially false premise.
tags: [Multimodal AI, Mechanistic Interpretability, Trustworthy AI]
featured: true
weight: 1
---
This project asks whether a medical vision-language model that agrees with a false spatial claim failed to perceive the image or chose to follow the user's premise despite internally representing the correct answer.

The current benchmark contains 3,244 spatial questions derived from SLAKE annotations. Neutral prompts establish baseline competence before evaluation under six pressure conditions. For self-hosted models, linear probes test whether the correct spatial information remains recoverable from vision-tower representations.

The study spans six models. Human auditing and some generation issues remain under investigation, so the results are preliminary.
