# Prompt pattern

## Canonical typefaces

Use one modern grotesk sans-serif system throughout.

- Simplified Chinese main title: `Source Han Sans SC Heavy` or `Noto Sans CJK SC Black`; fall back to `PingFang SC Heavy`.
- Latin acronym main title: `Helvetica Neue Black`, `Arial Black`, or an equivalent heavy neo-grotesk sans serif.
- Category Tag and hooks: the same family in `Bold` or `Heavy`; never mix serif, Song, handwritten, calligraphic, condensed, outlined, or decorative display fonts.
- Use near-black solid fills. Do not add bevels, gradients, shadows, strokes, distortion, perspective, or texture to typography.

## Canonical vertical geometry

For `3:4` covers:

- Export at `900 × 1200` and compose natively at `3:4`.
- Use a `64–72 px` left safe margin and at least `64 px` top/bottom safe margins.
- Begin every left-aligned text block on one common vertical axis around `x = 68 px`.
- Use roughly `60–65%` of the full canvas width for the protected typography column and only `28–35%` for the subject.
- Reserve a continuous blank warm-ivory corridor of about `5–7%` of canvas width between the protected text column and the subject.
- Establish a hard vertical illustration boundary around `x = 58–62%` of canvas width. Keep the entire area left of that boundary illustration-free from the top edge to the bottom edge.
- Keep the protected text column and corridor free of cables, shadows, objects, paths, rails, nodes, body parts, architecture, and decorative marks at every vertical position, including empty space below the hook.

### Category Tag token

- Place the Tag around `x = 68–78 px`, `y = 155–175 px`.
- Use a flat solid dark-red `#981B16` badge with solid warm-ivory `#F4F0E6` Bold/Heavy text.
- Use a modest `5–8 px` corner radius. Keep it a compact editorial rectangle, not a capsule or pill.
- Use approximately `16–20 px` horizontal padding and `9–12 px` vertical padding.
- Target a total Tag height of `54–58 px` and a text cap height around `30–35 px`.
- Do not use an outline-only box, hollow/outlined text, border, gradient, shadow, glow, bevel, or texture.
- Keep the Tag on one line and never let it compete with the title.

### Main-title token

- Start the title around `y = 280–305 px`, leaving `75–100 px` between the Tag and title.
- Let the title fill `85–95%` of the text-zone width and roughly `35–42%` of total canvas height for a three-line title.
- Use two to four compact lines. Break long phrases across lines instead of shrinking them.
- For a three-line structure like the approved reference, use approximately:
  - Latin acronym line: `135–155 px` visual cap height, Black weight;
  - Chinese title lines: `92–112 px` visual character height, Heavy/Black weight;
  - baseline-to-baseline leading: approximately `1.00–1.10 ×` each line's visual height;
  - optical gap between Latin acronym and first Chinese line: `18–30 px`;
  - optical gap between Chinese lines: `10–22 px`.
- Keep character spacing neutral to slightly tight, around `-1%` to `-3%`, without glyph collisions.
- Never squeeze a long job name into one small line. Prefer semantic line breaks of `2–6` Chinese characters per line.

### Title-bracketing dividers and hook token

- Use two matching dark-red dividers approximately `84–110 px` wide and `3–5 px` thick, aligned to the common left text axis.
- Place the upper divider between the category Tag and the main title; place the lower divider between the main title and the supporting hook. The main-title block must be visibly bracketed by these two bars.
- Leave clear optical breathing room around both dividers. For the lower divider, leave `45–65 px` below the main-title block and `40–55 px` before the first hook line.
- Never omit the lower divider above the hook, and never substitute a border, underline, long rule, or decorative line.
- Use supporting hooks at approximately `38–48 px` visual height, Bold/Heavy weight.
- Keep hook lines at one equal level with `10–18 px` vertical gap.
- Highlight only one number or one short keyword in dark red; preserve the rest in near black.
- Keep at least `70 px` clear space below the final hook line.

### Subject token

- Keep the subject entirely to the right of the hard vertical boundary, approximately from `x = 560–600 px` to the right edge on a `900 px` canvas.
- Keep the subject visually substantial while preserving the blank corridor. Shift or scale the subject before reducing title size.
- For vertical covers, default to a `右侧半隐人物构图`: enlarge the figure, lock it to the right edge, and let nonessential outer anatomy continue beyond the right or bottom frame. Prefer half-body, partial three-quarter-body, or action-detail framing over a small complete full body.
- Keep the face, hands, and metaphor-defining action fully readable. Crop shoulders, torso, hips, or legs before sacrificing title scale or the blank corridor.
- Aim for a large, close, partly concealed subject that implies continuation beyond the frame and creates curiosity while leaving the left typography zone spacious.
- Use a minimal doorway only when it carries meaning. Keep it on the far-right edge and use controlled light-gray structure.
- Keep a faint contact shadow within roughly `20–35 px` beneath the shoes. Do not build a large ground plane.
- Keep all non-subject background areas warm ivory and visually quiet.

## Production template

```text
Use case: ads-marketing
Asset type: Chinese knowledge-media cover, native [platform, ratio, dimensions]
Input reference: reference-vertical-3x4.png or reference-wechat-wide.png defines the house layout, typography scale, and quality. Use it only as a layout reference.
Primary request: Create the next cover in the established series for [topic]. Express [user-provided central idea, or one automatically inferred action-driven metaphor from category + title + hook] through one conceptual image.

Exact text and hierarchy:
Category Tag, smallest: "[category]"
Main title, largest, left-aligned lines: "[line 1]" / "[line 2]" / "[line 3]"
Supporting hook, smaller equal-level lines: "[hook 1]" / "[hook 2]"
Highlight only "[one short keyword or number]" in dark red.

Typography: Chinese uses Source Han Sans SC Heavy / Noto Sans CJK SC Black with PingFang SC Heavy fallback; Latin acronyms use Helvetica Neue Black / Arial Black. Use one heavy modern grotesk sans-serif family, solid fills, no text effects. Render the category as a compact solid dark-red #981B16 badge with solid warm-ivory #F4F0E6 text and modest rounded corners; no outline-only box or hollow text. Follow the canonical Tag, main-title, divider, hook, leading, spacing, and safe-margin tokens above.
Composition: make text the primary information carrier. For vertical covers, reserve about 60–65% of total width as a full-height protected typography column, 5–7% as a blank warm-ivory corridor, and only 28–35% for the illustration. Establish a hard vertical boundary near x=58–62% and keep every illustration pixel strictly to its right from top to bottom. No subject edge, body part, prop, path, rail, node, cable, shadow, object, architecture, or decorative line may appear anywhere in the protected left column, even below or between text blocks. Make the title fill 85–95% of its text zone and dominate at thumbnail size. For vertical covers, use the right-edge partial-figure composition: enlarge and crop the person against the right edge while keeping the face/hands/core action readable inside the smaller visual zone. Reduce or crop the illustration before reducing title size.
Concept: [one action-driven metaphor with one dominant subject]. If no central visual was provided, infer it from the topic noun, promised transformation, and strongest action or contrast in the category/title/hook. Prefer a concrete, safe external-object action; avoid body disassembly, medical imagery, and generic technology filler. Keep it mainly in the right zone and remove nonessential environment.
Style: clean high-definition black-and-white hyperreal editorial concept image; premium conceptual photography or photoreal editorial 3D composite; realistic anatomy and materials; strict neutral grayscale throughout the complete illustration; subtle rim light; softly dissolving outer edges; faint contact shadow only.
Visual mode: [黑白主版: every illustration pixel is neutral grayscale, including skin, hair, clothing, props, reflections, and shadows; no chromatic tint] or [克制彩色版: realistic low-saturation natural skin, fabric, and material colors]. Apply one mode consistently to the whole platform set.
Right-side visual mode: [弱视觉: small, pale, low-contrast, title-first] or [强视觉: larger, more complete, higher-contrast narrative subject]. Both modes must share one continuous warm-ivory background and dissolve into it; never use a separate panel, tonal block, split background, hard seam, collage edge, or pasted-on image region.
Palette: flat warm ivory #F4F0E6, near black #090909, dark red #981B16 only for the Tag, short divider, and one short emphasis. Lock the same background target across all formats; subject lighting or color must not tint the paper background.
Constraints: exact Simplified Chinese; native target ratio; one metaphor; no additional words; safe margins; strong thumbnail readability; full-height illustration-free protected text column.
Illustration text ban: no words, letters, numbers, labels, signage, screen text, paper text, pseudo-writing, logos, or watermarks.
Avoid: timid title scale, centered typography, subject touching text, pen drawing, engraving, crosshatching, stippling, sketch lines, speed rays, flying papers, floor ink strokes, dense doorway shading, generic robots, brains, chips, code walls, neon, glossy sci-fi 3D, sepia, and decorative clutter.
```

## Named platform presets

Use exactly three presets:

- `竖屏版`: native `3:4`, export `900 × 1200`.
- `公众号版`: native `900 × 383`, approximately `2.35:1`.
- `X版`: native `5:2`, export `1500 × 600`.

When the user asks for “三个平台版本” or “全套”, generate all three as independent native compositions. Never crop or stretch one output to obtain another.

## Horizontal adaptation

For `公众号版` and `X版`, reduce title line count before reducing legibility. Keep the Tag and title in the left safe area, the hyperreal concept subject on the right, and a visible clean corridor between them. Preserve the same font family, weight hierarchy, warm-ivory background, near-black title, and dark-red accents. Recalculate all vertical tokens proportionally for the shorter canvas rather than copying the 3:4 pixel coordinates.

Do not automatically reuse the vertical `右侧半隐人物构图` in horizontal formats. Choose a native waist-up, seated, crouched, or action-detail composition according to the available panoramic space.

## Targeted iterations

- Tag too small: “Keep everything else unchanged. Enlarge the solid dark-red category badge and its warm-ivory text by 5–10% while keeping it clearly subordinate to the title. Preserve the compact rectangle, modest corner radius, and solid fills.”
- Title too small: “Keep content unchanged. Enlarge the main-title block decisively until it fills 85–95% of the text-zone width.”
- Text and image touch: “Keep wording and title size unchanged. Shift or reduce the entire subject to preserve a continuous 4–6% blank warm-ivory corridor between every title glyph and every subject edge or shadow.”
- Illustration enters text column: “Keep all text unchanged. Move, crop, or reduce every illustration element so all people, props, paths, rails, cables, objects, and shadows remain strictly to the right of the hard full-height vertical boundary. Restore the entire left typography column to flat warm ivory behind the Tag, title, divider, hook, and all unused vertical space.”
- Subject looks dirty: “Keep composition unchanged. Remove pen lines, crosshatching, speed lines, flying papers, floor scribbles, dense environmental shadows, and decorative marks. Preserve only the clean hyperreal subject, minimal doorway, and faint contact shadow.”
- Subject contains text: “Remove every word, letter, number, label, sign, and pseudo-text from the subject and equipment; replace them with clean blank materials.”
- Wrong ratio: “Recompose natively for [ratio and dimensions]; do not crop or stretch the existing artwork.”
- Background mismatch: “Keep all text, composition, subject, and visual mode unchanged. Normalize every clean background region to the same flat warm ivory #F4F0E6; remove pink, gray, yellow, or brightness drift caused by subject lighting.”
- Wrong visual mode: “Keep composition and typography unchanged. Re-render the complete subject consistently in [黑白主版 / 克制彩色版] while preserving the flat #F4F0E6 background and dark-red accents. For 黑白主版, remove every chromatic tint from skin, hair, clothing, props, reflections, and shadows; use strict neutral grayscale only.”
- Separate image block: “Keep the wording and subject concept unchanged. Remove every panel edge, split-color region, tonal block, frame, hard vertical seam, and collage boundary. Recompose the entire cover on one continuous #F4F0E6 paper background and let the subject edges dissolve naturally into it.”
