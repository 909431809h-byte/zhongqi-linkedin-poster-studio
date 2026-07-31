---
name: zhongqi-linkedin-poster-studio
description: Create and verify Zhongqi LinkedIn 1.91:1 overseas B2B poster campaigns. Use for one or ten premium international logistics, freight-forwarding, supply-chain, or foreign-trade visuals that need original art direction, exact English copy rendered inside the image, an upper-left logo safe area, mobile-safe composition, restrained #FF6602 accents, and iterative visual QA.
---

# Zhongqi LinkedIn Poster Studio

Create an enterprise campaign, not a generic logistics advertisement. This workflow uses an art-direction matrix and a test-and-revise loop so a ten-poster delivery has a coherent standard without becoming ten variations of the same picture.

## Lock The Campaign Contract

Use the following defaults unless the user changes them:

| Item | Requirement |
| --- | --- |
| Audience | Overseas importers, exporters, procurement teams, and freight-forwarding partners |
| Output | 10 visibly different finished posters, or the requested subset |
| Canvas | 1.91:1, preferably 1200 x 628 px or 1920 x 1005 px |
| Tone | Premium, calm, international, credible, enterprise-grade |
| Base palette | Charcoal, deep gray, light gray, and white |
| Accent | `#FF6602` only for intentional emphasis, never a full background |
| Logo zone | Leave the upper-left 14% width x 18% height empty unless the user provides a Zhongqi logo |
| Mobile safety | Keep all critical copy and the focal visual inside the central 72% width and 80% height |

Do not invent a Zhongqi logo. Do not defer copy to a later graphics-editing stage: headline, subheadline, and CTA must be rendered in the generated image.

## Develop Ten Original Art Directions

Before generating, create a compact concept matrix. Hold the campaign constants above, then vary at least four of these in every row: focal metaphor, environment, composition, medium, depth/lighting, and type placement. Use [the campaign matrix](references/poster-brief-and-matrix.md) as the starting point.

Use one distinct visual world for each poster:

1. Measured global connection
2. Executive ocean-trade atmosphere
3. Supply-chain orchestration
4. Intelligent logistics infrastructure
5. Dependable continuity
6. Controlled delivery momentum
7. International trade ecosystem
8. Minimal confidence and generous negative space
9. Editorial brand-campaign image
10. Global enterprise presence

Do not use a cargo plane, container pile, ship, map, or globe as a default shorthand. Prefer architecture, materials, systems, human decision-making, precise route geometry, light, or abstract operational metaphors. When a literal transport element is required, make it a single quiet supporting object.

## Write Copy Before The Image Prompt

Give every poster one copy set that matches its concept:

- `Headline`: 3-8 English words.
- `Subheadline`: 8-18 English words.
- `CTA`: 2-5 English words.

Use natural, plain international business English. Keep claims specific and credible. Avoid Chinese-English phrasing, exclamation marks, discount language, superlatives, vague hype, and claims the business cannot prove.

Read the copy aloud once. Count words before generation. Do not generate a second concept with merely a synonym swap.

## Build One Production Prompt Per Poster

Use the available image-generation workflow. If `imagegen` is installed, load it and follow its generation and inspection rules. Generate one poster per call, not ten style variants in one call.

Include all of the following in each prompt:

```text
Asset: 1.91:1 LinkedIn landscape poster, 1200 x 628 px.
Audience: overseas B2B trade and logistics decision-makers.
Concept: <one original visual world and focal metaphor>.
Art direction: premium international business campaign; <composition, material, lighting, and medium>.
Palette: charcoal/deep gray, light gray, white; use #FF6602 only for <specific accent role>.
Composition: reserve an entirely empty upper-left logo safe zone (14% width x 18% height); keep text and focal subject in the central mobile-safe area.
Text, rendered verbatim in the image:
Headline: "<headline>"
Subheadline: "<subheadline>"
CTA: "<CTA>"
Typography: clear modern sans-serif hierarchy, high contrast, no extra text.
Avoid: invented logos, text errors, text clipping, watermark, sale badges, loud gradients, stock-photo posing, dense cargo/containers/aircraft/ships/maps/globes, visual clutter, and orange background fields.
```

State the exact placement of each text layer so it does not enter the logo zone or collide with the focal object. Use no more than one focal object or system.

## Inspect, Repair, And Recheck

Inspect each rendered result at native resolution. Treat these as pass/fail gates:

| Gate | Pass condition |
| --- | --- |
| Format | Exact 1.91:1 ratio and requested usable resolution |
| Brand safety | Upper-left zone is empty or contains only the supplied logo |
| Copy | All three text layers are in the image, exact, legible, correctly spelled, and within word limits |
| Mobile crop | Critical elements survive a centered mobile crop |
| Art direction | The image reads as premium B2B, not low-end freight promotion |
| Color | Neutrals dominate; `#FF6602` acts as a small purposeful accent |
| Differentiation | Its visual world, layout, and focal metaphor differ from every other poster |

When a gate fails, revise only the failed element with a targeted regeneration or inpainting instruction. For example: “Keep the scene and copy unchanged. Re-render the subheadline exactly as written, move it into the central safe area, and preserve the empty upper-left logo zone.” Reinspect the changed poster and all gates it can affect.

## Deliver

For every accepted poster, provide the final image and a compact record containing: creative lane, headline, subheadline, CTA, prompt, and gate results. Keep rejected versions separate from accepted final assets. Report any text issue that could not be verified rather than claiming it passed.

## Method Note

This skill applies original-art-direction matrices, selective visual language, and explicit iteration gates informed by the reusable-workflow approach in [MengTo/Skills](https://github.com/MengTo/Skills). Do not copy third-party campaign artwork, layouts, marks, or distinctive visual signatures.
