# Photo to Healing Watercolor V3.6

<p align="center">
  <a href="./README.md">中文</a> · <strong>English</strong>
</p>

<p align="center">
  <strong>Turn a photo into a 3:4 “Original Photo + Simplified Storybook Illustration” postcard in one step.</strong>
</p>

---

## Overview

**Photo to Healing Watercolor V3.6** is a one-click skill for turning photographs into highly simplified editorial storybook illustrations.

It is not designed to apply a watercolor filter. Instead, it first understands the subject, action, relationships, composition, and scene, then removes photographic detail, compresses repeated objects, redesigns silhouettes and color relationships, and translates the image into a stable visual vocabulary.

The default output is:

> **Original Photo + Matching Simplified Illustration + 3:4 Minimal Nordic Postcard**

Official English name:

> **Photo to Healing Watercolor**

Chinese name:

> **照片转治愈水彩插画**

Core visual keywords:

> **White · Light · Pale · Soft · Round**

---

## Showcase

<table>
<tr>
<td width="50%" valign="top">
<img src="./assets/showcase-harbor.png" alt="Harbor architecture showcase">
</td>
<td width="50%" valign="top">
<img src="./assets/showcase-garden-portrait.png" alt="Garden portrait showcase">
</td>
</tr>
<tr>
<td width="50%" valign="top">
<img src="./assets/showcase-river-skyline.png" alt="River skyline showcase">
</td>
<td width="50%" valign="top">
<img src="./assets/showcase-indoor-portrait.png" alt="Indoor portrait showcase">
</td>
</tr>
</table>

---

## Key Capabilities

### 1. One-click workflow

The user only needs to upload a usable photo and invoke the skill.

No need to:

- configure complex parameters;
- choose a simplification level;
- describe the composition again;
- write an image-generation prompt.

The skill detects the scene automatically and applies different simplification strategies for people, architecture, plants, water, interiors, and other common subjects.

### 2. Redesign, not “watercolorize”

Core pipeline:

`PHOTO → COMMON CROP → SEMANTIC LOCK → EXPRESSION LOCK → SHAPE MAP → DELETE → MERGE → COUNT COMPRESS → GRAPHIC ABSTRACTION → VISUAL DICTIONARY → SYMBOLIZE → ROUND REDESIGN → FLATTEN → WHITENED COLOR REDESIGN → ILLUSTRATE → QC → CARD COMPOSITE`

The goal is not to make photographic detail “softer.” The skill instead:

- removes low-value photographic information;
- merges repeated objects;
- reduces object count;
- lowers structural complexity;
- replaces realism with a unified symbol system;
- redesigns silhouettes;
- flattens realistic lighting, depth, and material;
- rebuilds the palette with whitened creamy pastels.

### 3. Locked storybook visual language

V3.6 is based on:

> **Ultra-light gouache storybook + soft editorial illustration + subtle watercolor-paper texture**

Visual characteristics:

- generous paper-white areas;
- high lightness and low-to-medium-low saturation;
- rounded, soft, slightly imperfect silhouettes;
- large shapes and very few details;
- paint and paper texture used only as a subtle surface layer;
- no dependence on realistic shadows, materials, or perspective.

---

## Character Standard

Characters must actively move away from realistic portrait rendering.

### Face

A main face should normally contain only about **4–7 visual marks**:

- two small dark-brown oval / almond-shaped eyes;
- zero to two very short eyebrows;
- no nose by default;
- one short coral / warm-brown mouth stroke;
- two soft peach blush shapes.

Avoid:

- realistic eyeballs;
- eyelashes;
- nose bridge / nostrils;
- realistic lips;
- teeth detail;
- facial bone structure;
- complex facial shading.

### Hair

Hair is converted from “many strands” into:

- 1 main hair mass;
- 2–5 supporting masses;
- curls expressed mainly through the outer silhouette;
- no individual strands or photographic hair highlights.

### Clothing

White or light clothing should read almost like a paper-white shape:

- warm white / creamy white masses;
- only a few large fold strokes;
- no realistic fabric texture;
- no complex shading used to model volume.

---

## Flowers & Plants

### Flowers

Flowers are treated as page-decoration shapes rather than botanical studies.

Default behavior:

- remove roughly 70–85% of individual real flowers;
- keep about 3–6 large hero flowers in each major floral area;
- hero flowers may be enlarged to roughly 3–7× their real relative size;
- petals should be broad, round, and blunt;
- asymmetry, merged petals, and missing petals are allowed;
- flower centers are reduced to a simple dot or small color shape.

### Leaves

A plant group should generally use only **2–3 leaf templates**:

- large flat oval;
- soft elongated oval;
- rounded egg shape.

Many real leaves are merged into large foliage masses. Detailed veins, branches, and dense small leaves are removed.

---

## Architecture, Water & Environment

### Architecture

Buildings should first read as “storybook house shapes”:

- façade = one large color block;
- roof = simplified color block;
- windows = short white vertical marks / tiny rounded rectangles;
- non-essential repeated buildings may be reduced by about 30–50%;
- visible light gaps are preferred between neighboring buildings;
- sharp roof peaks are softened and rounded.

### Water

Water is first treated as a calm graphic color field:

- 2–5 broad blue-green horizontal bands;
- a few warm-white ripple symbols;
- a few beige, coral, or creamy-yellow reflection blocks;
- no high-frequency realistic ripples;
- no full mirror reflection.

### Sky

The sky mainly provides breathing room:

- warm white / cream paper as the primary field;
- 1–3 pale-blue cloud masses;
- no realistic cloud anatomy, dramatic sunlight, or HDR effects.

---

## Color System

V3.6 uses a whitened creamy pastel palette:

- warm white / cream;
- oatmeal / pale beige;
- soft butter yellow;
- pale peach;
- soft coral;
- sage green;
- creamy yellow-green;
- pale blue-green;
- misty blue / light gray-blue;
- soft chestnut / milk-coffee brown.

Rule:

> **If the color feels too solid, add white—not gray.**

---

## 3:4 Postcard Specification

The final card is always **portrait 3:4**.

Recommended logical size:

- `1536 × 2048 px`
- or any strict 3:4 equivalent.

Fixed layout:

1. Top: the original uploaded photograph;
2. Bottom: the matching simplified illustration;
3. Bottom margin: warm beige paper;
4. Centered in the bottom margin: handwritten `@Jemima`.

Critical requirements:

- the top panel uses the real original photo pixels;
- one subject-safe crop may be performed first;
- that crop becomes the `COMMON PANEL CROP`;
- the illustration must inherit the exact same crop;
- top and bottom panels must have identical display width, height, and aspect ratio;
- the two panels connect with zero gap;
- no image stretching;
- the original top photograph must not be regenerated by AI.

---

## Supported Scene Types

The skill automatically adapts to:

- portraits;
- wedding / garden photography;
- harbor / seaside scenes;
- city streets;
- lakeside / waterside towns;
- nature landscapes;
- indoor lifestyle scenes;
- architecture;
- everyday still life.

---

## Usage

Minimal workflow:

1. Provide `photo-to-healing-watercolor_V3.6_SKILL.md`;
2. Upload a photo;
3. Ask the model to invoke the skill;
4. The default result is the complete 3:4 postcard.

Example:

```text
Use Photo to Healing Watercolor V3.6
and process this photo with the default Skill standard.
```

Illustration-only mode:

```text
Use Photo to Healing Watercolor V3.6 and output only the simplified illustration,
without the postcard layout.
```

---

## Design Principle

The key criterion is not simply whether the image looks beautiful.

The result should:

> **still be immediately recognizable as the original scene, while also being immediately recognizable as no longer photographic.**

A successful output should feel like:

> **a storybook page redesigned from the photograph**

—not:

> **a photograph painted in watercolor.**

---

## Project Structure

```text
photo-to-healing-watercolor-v3.6/
├── README.md
├── README_EN.md
├── photo-to-healing-watercolor_V3.6_SKILL.md
├── showcase-harbor.png
├── showcase-garden-portrait.png
├── showcase-river-skyline.png
└── showcase-indoor-portrait.png
```

---

<p align="center">
  <a href="./README.md">← 切换到中文 README</a>
</p>
