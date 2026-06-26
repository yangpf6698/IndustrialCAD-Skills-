---
id: SKILL-005
title: Geometry Rules / 几何规则
summary: |
  EN: Rules for valid geometry: fillet/rounding, minimum radii, planar faces, and manufacturable features.
  CN: 有效几何的规则：倒角/圆角、最小半径、平面面、可制造特征等。
version: 1.0
tag: [geometry, rules, manufacturability]
ontology_refs:
  - geometry:Edge
inputs:
  - model_geometry: cad_brep
outputs:
  - geometry_issues: list
author: Copilot / 杨
---

# Geometry Rules / 几何规则

EN: Validates geometry against manufacturability rules and recommended practices.

CN: 将几何与可制造性规则和建议实践进行对比校验。
