---
name: create-knowledge-media-cover
description: Create a unified Chinese knowledge-media cover series with black-and-white or restrained-color hyperreal subjects, a dark-red category tag, a dominant large left-aligned title, warm ivory paper, and a strict full-height boundary between the text and illustration zones. Infer a supporting hook from the category and title when omitted, and infer the conceptual image from the category, title, and hook when the user omits a core visual. Use for 3:4 vertical covers, 公众号横版封面, X post images, knowledge-video covers, article headers, requests for 竖屏版、公众号版、X版、全套、黑白主版、克制彩色版、右侧半隐人物构图, or requests to reuse the established personal-media house style.
---

# Create Knowledge Media Cover

Create the next issue in one recognizable series, not an isolated poster. Keep the layout grammar stable; change only the category, title, hook, and conceptual image.

## Inputs

Extract or infer:

- category tag;
- main title and preferred line breaks;
- optional supporting hook;
- optional central idea to express visually;
- platform, ratio, and output size.

Resolve the user's platform words through the three named presets below. Default to `竖屏版` when no platform is given. Ask only when a missing choice materially changes the result.

## Required workflow

1. Read [references/prompt-pattern.md](references/prompt-pattern.md).
2. Inspect the relevant bundled reference image at full size.
3. Use the user's hook when provided. Otherwise write one automatically by following `Automatic hook inference` below.
4. Use the user's central visual when provided. Otherwise infer one action-driven metaphor from the category, main title, and final hook by following `Automatic visual inference` below.
5. Select one visual mode for the whole requested set: `黑白主版` by default, or `克制彩色版` when the user explicitly requests color or both modes.
6. Generate each platform format as a native composition. Never crop one master image into every ratio.
7. Verify exact text, typography scale, category/title/hook hierarchy, the full-height text-zone exclusion boundary, single-metaphor clarity, crop safety, thumbnail readability, visual-mode consistency, and background-color consistency.
8. Iterate on only the largest failure.
9. Save a high-resolution source and platform-ready exports in the user's project.

## Automatic hook inference

Treat the supporting hook as optional. When it is blank or omitted, do not ask by default. Write a concise hook from the category and main title before generating.

- Explain the reader benefit, key question, transformation, or tension promised by the title instead of merely repeating it.
- Prefer one or two short lines that remain readable at thumbnail size.
- Select only one short keyword or number for dark-red emphasis.
- Keep the claim faithful to the title. Do not invent unsupported outcomes, guarantees, urgency, or statistics.
- Ask only when the missing hook would force a materially different factual promise; otherwise choose the clearest version and proceed.

## Automatic visual inference

Treat the central visual as optional. When it is omitted, do not ask by default. Infer the illustration from the category, main title, and hook before generating.

1. Identify the topic noun, promised transformation, and strongest action or contrast in the title and hook.
2. Convert that relationship into one instantly readable physical action involving one dominant person or object.
3. Prefer concrete editorial metaphors such as plugging, assembling, unlocking, carrying, crossing, filtering, replacing an external tool, or revealing a hidden structure.
4. Keep the metaphor faithful to the claim. Do not invent a second promise, character, or storyline.
5. Prefer safe, non-gory, non-medical external-object metaphors. Do not depict body disassembly, exposed body sockets, detached limbs, wounds, surgery, or body horror unless the user explicitly requests such imagery.
6. Reject generic filler such as robots, brains, chips, code walls, holograms, floating UI, or neon merely to signal “technology.” Use them only when they are the actual subject.
7. Ask a question only when two materially different interpretations would change the cover's factual meaning or could misrepresent the topic. Otherwise choose the clearest thumbnail-readable metaphor and proceed.

If the user supplies a central visual, follow it while still applying the house style, safety constraints, and platform composition rules.

## Visual modes

- **黑白主版 (default):** Render every illustration pixel—including skin, hair, clothing, props, equipment, highlights, reflections, shadows, and environmental elements—in strict neutral grayscale only. No skin tone, cream, beige, brown, blue, or other chromatic tint is allowed in the right-side visual. Keep only the category Tag, the two short dividers, and one short hook emphasis in dark red. The warm-ivory paper background is the only non-gray neutral outside those red accents.
- **克制彩色版:** Preserve realistic, low-saturation natural skin, fabric, and material colors while keeping the typography system, dark-red accents, warm-ivory background, clean subject treatment, and text-image separation identical to the black-and-white mode. Avoid vivid fashion colors, cinematic teal-orange grading, or extra accent colors.
- When the user asks for **both versions**, generate two complete native platform sets rather than colorizing or desaturating finished exports.
- Never mix modes within one three-platform set unless the user explicitly requests per-platform differences.

## Right-side visual modes

Resolve the illustration hierarchy independently from the color mode:

- **弱视觉 (default):** Keep the title as the absolute first visual focus. Use a smaller, lower-contrast supporting metaphor in pale silver, light gray, and soft charcoal. Let its peripheral edges and shadows fade gently into the same continuous warm-ivory paper background. Choose this mode when the user asks for `弱视觉`, `标题优先`, or does not name a right-side visual mode.
- **强视觉:** Use a larger, more complete, higher-contrast hyperreal subject or action metaphor on the right. The title must remain readable and primary, but the subject may carry stronger narrative impact. Choose this mode when the user asks for `强视觉`, `概念人物`, `右侧半隐人物构图`, or `以前那种右侧视觉`.
- **Both modes must be integrated:** `强视觉` and `弱视觉` differ only in subject scale, completeness, contrast, and narrative intensity. Both must dissolve naturally into the same continuous warm-ivory paper background. Neither mode may use a separate picture panel, rectangular image area, tonal block, framed inset, split-color region, hard vertical seam, collage edge, or pasted-on image-block effect.
- If the user asks for `两个版本` without specifying what differs, generate both right-side visual modes using the same wording, platform, ratio, and color mode.
- Apply one right-side visual mode consistently across a requested platform set unless the user explicitly requests per-platform differences.

## Fixed house system

- Use a flat warm ivory paper background targeted at `#F4F0E6`, near-black `#090909`, and dark red `#981B16`.
- Make the title the absolute first visual focus in every format. The conceptual image is supporting evidence only: keep it smaller, lower-contrast, and visually quieter than the typography. When title and image compete, reduce, lighten, simplify, or crop the image before changing the title.
- Integrate the conceptual image directly into the continuous warm-ivory paper background in both `强视觉` and `弱视觉`. Do not place it inside a separate picture panel, tonal block, framed inset, split-color region, or visibly divided right-hand column. Avoid hard seams that make the illustration look pasted onto the cover.
- Prefer pale silver, light gray, and soft charcoal for black-and-white supporting visuals. Let peripheral edges and shadows fade gently into the paper background while keeping the core metaphor readable. Do not allow skin tone, brown, beige tint, blue, or other subject color in `黑白主版`; dark red remains reserved for the existing typography accents.
- Lock the same background target across every image in one set. Do not let subject color mode, lighting, paper texture, or platform ratio shift the background warmer, pinker, grayer, or brighter.
- Treat the category as the smallest text level. Render it by default as a compact solid dark-red `#981B16` badge with solid warm-ivory `#F4F0E6` Bold/Heavy text. Use modest rounded corners and balanced padding; do not use a red outline box, hollow/outlined lettering, gradient, shadow, glow, bevel, or pill shape. Make it readable at thumbnail size without letting it compete with the title.
- Make the main title the dominant element. Use large, heavy Simplified Chinese and bold Latin sans-serif type across two to four compact lines.
- Bracket the main-title block with two short dark-red divider bars: one between the category Tag and the title, and one between the title and the supporting hook. Align both bars to the common left text axis and keep their color, width, and thickness visually identical. Never omit the lower bar above the hook.
- Keep supporting hook lines smaller and at one equal level below the lower divider. Highlight only one number or one short keyword in red.
- Reserve the left side for typography and place one understated hyperreal conceptual subject toward the right edge in the selected visual mode. Treat the geometric boundary as an exclusion rule for keeping imagery away from text, not as a visible panel boundary.
- Render the subject like premium conceptual photography or a photoreal editorial 3D composite: realistic anatomy and materials, color treatment governed strictly by the selected color mode, subtle rim light, clean dissolving edges, and only a faint contact shadow.
- Keep the background, doorway, and environment minimal. Do not use pen drawing, engraving, crosshatching, stippling, speed lines, flying papers, ink strokes, floor scribbles, dense doorway shading, or decorative environmental marks.
- Keep a continuous warm-ivory separation corridor between text and image. No subject edge, shadow, or architectural line may touch a title glyph.
- Treat the text zone as a full-height protected column, not as separate boxes around individual text lines. From the top edge to the bottom edge, allow only the Tag, title, divider, hook, and warm-ivory background inside this column. No person, body part, prop, path, rail, node, cable, architecture, contact shadow, or decorative mark may enter it at any vertical position.
- Allow no readable text, letters, numbers, labels, signage, screen text, paper text, or pseudo-writing inside the illustration.
- Follow the layout tokens and font rules in [references/prompt-pattern.md](references/prompt-pattern.md). Treat them as constraints, not suggestions.

## English capitalization

- Preserve any capitalization explicitly supplied by the user. Never convert supplied English copy to all caps, small caps, sentence case, or another style merely for visual impact.
- When the user does not specify casing, default English cover text to professional title case rather than all caps: capitalize principal words and keep short articles, coordinating conjunctions, and short prepositions lowercase where normal English title style calls for it. Example: `Design and Implementation`.
- Preserve conventional uppercase for acronyms and initialisms such as `AI`, `API`, `LLM`, and `FDE`.
- Preserve the user-selected spelling and casing of product or project names even when it differs from another public convention. For this series, use `Deepseek Harness` when that is the wording provided.
- Use font weight, scale, spacing, and line breaks to create emphasis. Do not manufacture hierarchy by uppercasing every English word.

## Vertical-only right-edge partial figure

Use `右侧半隐人物构图` for `竖屏版` only when the user selects `强视觉` or explicitly requests this composition. Do not apply it to the default `弱视觉`.

- Enlarge the person and anchor them tightly to the right canvas edge.
- Use a text-dominant split: reserve roughly `60–65%` of the full canvas width for the protected typography column, `5–7%` for a blank warm-ivory corridor, and only `28–35%` for the illustration. Treat these as hierarchy targets, not a reason to reduce title scale.
- Establish one hard vertical boundary around `x = 58–62%` of canvas width. Keep every illustration pixel strictly to the right of that boundary from top to bottom.
- Show only a half-body, partial three-quarter body, or the most narrative body section. Let the outer shoulder, torso, hip, or legs continue naturally beyond the right or bottom frame.
- Preserve the complete face, hands, and core action whenever they carry the metaphor. Crop nonessential anatomy before shrinking the subject or title.
- Make the person feel close, substantial, and partly concealed: large in visual scale but limited to the right subject zone.
- Use edge truncation to imply that more exists outside the frame and create curiosity without hiding the action.
- Never show a full-body figure merely for completeness when doing so compresses the title zone.
- Preserve the continuous warm-ivory separation corridor. No cropped body edge, hand, prop, cable, or shadow may enter it.
- Do not apply this rule automatically to `公众号版` or `X版`; compose their subjects independently for their horizontal ratios.

## Platform formats

- `竖屏版`: native `3:4`, export `900 × 1200`.
- `公众号版`: native `900 × 383`, approximately `2.35:1`.
- `X版`: native `5:2`, export `1500 × 600`.

Redesign line breaks and illustration placement for every ratio. Never crop or stretch the vertical cover into a horizontal asset.

## Shortcut commands

Interpret these user phrases directly without asking for dimensions:

- “做竖屏版” or “做 3:4” → generate only `竖屏版`.
- “做右侧半隐人物竖屏版” or “竖屏继续用右侧半隐人物构图” → generate only `竖屏版` using the vertical-only right-edge partial-figure rule.
- “做公众号版” → generate only `公众号版`.
- “做 X 版” or “做推特版” → generate only `X版` at `5:2`.
- “做三个平台版本”, “做全套”, or “三个都要” → generate all three presets as three separately composed images.
- “做封面” with no platform → default to `竖屏版` only.

The user needs to provide only the category and title; the hook and central visual are optional. When the hook is omitted, write it automatically from the category and title. When the central visual is omitted, infer it automatically from the category, title, and final hook. Infer line breaks and composition from the canonical references and tokens.

## Reference assets

- `assets/reference-vertical-3x4.png`: canonical vertical reference for warm-ivory color, text scale, Tag size, title dominance, hook size, clean hyperreal subject treatment, and strict text-image separation.
- `assets/reference-wechat-wide.png`: horizontal WeChat composition reference.

Use the assets only as layout and quality references. Do not copy their topic-specific wording, people, objects, or metaphors.

## Final validation

- Confirm the title is unquestionably the first visual focus at both full size and thumbnail size; the conceptual image must remain smaller, lighter, and subordinate.
- Confirm the main title is visibly bracketed by two matching short dark-red bars: Tag → upper bar → title → lower bar → hook. Confirm neither bar is missing, misplaced, or merged into another element.
- Confirm the illustration shares one continuous warm-ivory background with the typography and creates no panel, inset, split background, hard seam, or pasted-on image-block effect.
- For `黑白主版`, sample the illustration itself—not only the background—and confirm that every subject pixel is neutral grayscale. Reject and regenerate if skin, hair, clothing, metal, reflections, shadows, or props contain any visible chromatic tint. Dark red is permitted only in the Tag, two dividers, and one short hook emphasis.
- Confirm the category Tag uses a solid dark-red badge with solid warm-ivory text, is readable at thumbnail size, and remains clearly subordinate.
- Confirm the title fills roughly `85–95%` of its text zone and dominates at thumbnail size.
- Confirm the hook is smaller than the title.
- Confirm font family, weight, line breaks, leading, padding, divider, and block spacing match the canonical tokens.
- Confirm a blank corridor visibly separates every title glyph from every illustration line.
- Confirm the entire protected text column remains illustration-free from the top edge to the bottom edge, including apparently unused space below or between text blocks.
- Confirm the clean hyperreal subject uses one metaphor, contains no unintended text, and has no sketch or ink-line artifacts.
- Confirm exact wording, punctuation, ratio, dimensions, safe margins, and black-white-red palette.
- Confirm every platform export in the set uses the same selected visual mode and a visually matching `#F4F0E6` background. Sample clean corner/background regions if the images appear different.
