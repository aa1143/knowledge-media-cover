---
name: create-knowledge-media-cover
description: Create consistent Chinese editorial knowledge covers with a replaceable category label, a dominant central headline, one concept image that expresses the topic, and a black, cool-white, and restrained dark-red palette. Use when creating 公众号封面、小红书封面、文章头图、知识类视频封面，或用户要求沿用“AI 学习指南”黑白雕刻红色点缀的个人栏目封面风格。
---

# Create Knowledge Media Cover

Create a recognizable cover series, not an isolated poster. Use the bundled reference images as composition and quality references without copying their topic-specific person, staircase, doorway, or wording.

## Inputs

Extract or infer:

- category label, such as `AI 学习指南`;
- main title;
- central idea to express visually;
- platform and aspect ratio.

Ask only when a missing choice materially changes the result. Default to `3:4` for vertical covers and `900 × 383` for WeChat horizontal covers.

## Fixed visual system

- Use a neutral cool-white paper background around `#F7F7F5`.
- Use crisp near-black text and illustration around `#090909`.
- Use dark red around `#8E1B16` only for one numeral, keyword, issue number, or short divider.
- Use monochrome woodcut, copperplate engraving, pen etching, crosshatching, or stippling.
- Keep the category label at the top as a persistent column marker. It is not the main title.
- Make the main title the visual center. Use large, heavy, highly legible Simplified Chinese type across a few balanced lines.
- Use exactly one main conceptual illustration to communicate the topic. Prefer a visual action or metaphor over literal technology decoration.
- Separate title and image zones while allowing the image's motion, light, or linework to connect them.
- Keep generous negative space and crop-safe margins.

## Composition

For `3:4` vertical covers:

- Put the category label near the upper-left, followed by a short dark-red divider.
- Place the large headline through the upper-middle or central region.
- Place the single main image mainly in the lower half or along one side, with a strong upward or inward direction.
- Recompose vertically; never crop a landscape cover into portrait.

For `2.35:1` WeChat covers:

- Use a 55/45 or 45/55 split between typography and illustration.
- Keep the category label above the headline.
- Preserve headline readability in small thumbnails and common center crops.

## Main-image rule

Translate the topic into one action-driven metaphor such as entering, climbing, opening, revealing, balancing, escaping, transforming, or choosing. Show one dominant subject or scene only. Do not add explanatory labels inside the illustration.

Do not automatically reuse the four-step staircase. Use it only when the subject is genuinely about steps, progress, or a learning path.

Avoid generic robots, brains, chips, circuit boards, code walls, neon cyberpunk, glossy 3D, decorative clutter, yellow sepia paper, logos, watermarks, and unintended text.

## Workflow

1. Read [references/prompt-pattern.md](references/prompt-pattern.md).
2. Inspect the relevant bundled reference image at full size.
3. Turn the topic into one visual metaphor and select a text-image split.
4. Generate one cover with the image-generation tool.
5. Verify exact Chinese text, category/title hierarchy, single-metaphor clarity, palette, crop safety, and thumbnail readability.
6. If needed, iterate on only the largest failure.
7. Save both the high-resolution source and a platform-ready export in the user's project.

## Reference assets

- `assets/reference-vertical-3x4.png`: primary reference for vertical layout and hierarchy.
- `assets/reference-wechat-wide.png`: primary reference for horizontal WeChat layout.

Treat these as the canonical series identity. Preserve the system; change the topic, wording, and central metaphor.
