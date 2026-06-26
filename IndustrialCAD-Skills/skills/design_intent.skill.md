---
id: SKILL-003
title: Design Intent / 设计意图
summary: |
  EN: Capture and enforce high-level design intent to preserve features through model changes.
  CN: 捕获并维护高层设计意图，确保在模型变更过程中保留关键特征。
version: 1.0
tag: [intent, parametric, constraints]
ontology_refs:
  - geometry:Feature
inputs:
  - model: cad_model
  - intent_spec: yaml/json
outputs:
  - intent_report: list
author: Copilot / 杨
---

# Design Intent / 设计意图

EN: This skill extracts and enforces design intent (functional surfaces, critical dimensions, tolerance-driven features).

CN: 该技能提取并强制实施设计意图（功能面、关键尺寸、由公差驱动的特征）。
