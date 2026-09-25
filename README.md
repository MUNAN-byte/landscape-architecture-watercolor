# Landscape & Architecture Watercolor

A Codex Skill that transforms landscape, cityscape, architecture, storefront, and architectural-interior photographs into vertical editorial diptychs with a photo-derived watercolor memory panel.

The Skill does **not** apply one fixed watercolor filter. It first classifies camera distance, lighting, and subject structure, then selects no more than five visual-memory cue types for reconstruction.

## What it produces

- Upper section: the source photograph.
- Lower section: a restrained, source-derived watercolor memory composition.
- One short English editorial title.

## Core method

`classify → deconstruct → select ≤5 cue types → reconstruct in watercolor → quality gate`

The lower panel should read first as an abstract editorial composition and only secondarily recall the specific photograph.

## Install

Download or clone this repository into your Codex skills directory:

```text
~/.codex/skills/landscape-architecture-watercolor/
```

The installed folder must contain `SKILL.md` at its root. Restart Codex if the Skill does not appear immediately.

## Files

- `SKILL.md` — entry point, workflow, constraints, and quality gate.
- `references/scene-routing.md` — camera-distance, lighting, and subject routing.
- `references/prompt-recipes.md` — master prompt, scene recipes, and correction prompts.
- `agents/openai.yaml` — Codex UI metadata.

## Important limitation

Image generation can reconstruct the photographic section even when instructed not to. For a final requiring pixel-faithful source preservation, generate the watercolor panel separately and combine it with the original photograph using deterministic compositing.

## 中文说明

这是一个用于风景、城市、建筑、橱窗和建筑室内照片的 Codex Skill。它会先判断近景、中景、远景以及主要光线，再从原图中选出最多五类“视觉记忆线索”，重组为克制的水彩编辑面板。

它不是固定滤镜，也不适用于人物或动物近景。

正式交付如果要求上方原照片像素完全不变，应单独生成水彩面板，再进行确定性拼接。

## License

Original Skill materials are licensed under [CC BY-NC 4.0](LICENSE.md): attribution is required and commercial use is not permitted. Third-party images are excluded from the license.
