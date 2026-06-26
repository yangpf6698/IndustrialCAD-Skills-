---
id: SKILL-001
title: Industrial Constraint — Boundary / 工程约束 — 边界
summary: |
  EN: Validations for plate/part boundary-related constraints (minimum thickness, edge distances, aspect ratio).
  CN: 对板件/零件边界相关约束（最小厚度、孔边距、纵横比）的校验与建议。
version: 1.0
tag: [constraint, boundary, manufacturability, sheet_metal]
ontology_refs:
  - geometry:Plate
  - manufacturing:laser_cutting
rules:
  - SM-0045
inputs:
  - geometry: mesh/edges
  - parameters: { thickness_mm: number, material: string }
outputs:
  - validation_report: violations[]
  - suggested_changes: suggestions[]
author: Copilot / 杨
---

# Industrial Constraint — Boundary

EN: This skill checks minimum thickness, maximum aspect ratio and hole edge distances for plate-like parts.

CN: 该技能用于校验板类零件的最小厚度、最大纵横比与孔到边缘的最小距离，并提供修改建议。

## Core Checks / 核心校验项

1. Minimum Thickness: thickness >= 1.5 mm (default for sheet metal unless material specifies otherwise)
2. Maximum Aspect Ratio: max(length, width) / min(length, width) <= 15
3. Edge Distance for Holes: see rules/SM-0045

## Example / 示例

Input: Plate thickness = 1.2 mm -> Output: Violation Minimum Thickness (建议厚度 >= 1.5 mm)
