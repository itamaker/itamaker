---
name: Zhaoyang Jia GitHub Profile
description: Native GitHub Markdown for discovering open-source projects and agent skills.
typography:
  name:
    fontSize: "2em"
    fontWeight: 600
    lineHeight: 1.25
  section:
    fontSize: "1.5em"
    fontWeight: 600
    lineHeight: 1.25
  category:
    fontSize: "1.25em"
    fontWeight: 600
    lineHeight: 1.25
  subsection:
    fontSize: "1em"
    fontWeight: 600
    lineHeight: 1.25
  body:
    fontSize: "16px"
    fontWeight: 400
    lineHeight: 1.5
spacing:
  block: "16px"
  heading-before: "24px"
  list-item: "0.25em"
components:
  section-index:
    typography: "{typography.body}"
  project-list:
    typography: "{typography.body}"
  disclosure:
    typography: "{typography.body}"
  quotation:
    typography: "{typography.body}"
  category-heading:
    typography: "{typography.category}"
---

# Design System: Zhaoyang Jia GitHub Profile

## Overview

**Creative North Star: "Native GitHub Markdown"**

The profile uses GitHub's familiar document language: clear headings, ordinary links, semantic lists, and a native disclosure. Its personality comes from Zhaoyang's English voice, playful shipping theme, and existing content.

GitHub controls presentation in production. The frontmatter records inherited type and spacing observed in the reviewed build; it does not install CSS or override host defaults. Fonts, themes, focus treatments, and available width remain governed by GitHub.

**Key Characteristics:**
- Semantic hierarchy and one-column reading.
- Native links and keyboard-operable disclosure.
- Inherited light/dark presentation; existing external imagery.

**The Host Authority Rule.** Inherit GitHub's presentation rather than treating a preview fixture as authored production styling.

## Colors

### Primary

Links inherit GitHub's theme-aware accent. There is no authored primary color token.

### Neutral

Text, muted quotations, document backgrounds, and heading dividers inherit GitHub's semantic theme colors. Existing badges and the contribution graph retain their source artwork and colors. No project palette is extracted from those images.

## Typography

**Font:** GitHub's inherited sans-serif stack, including platform fallbacks and emoji support. No font family is authored or shipped by this repository.

The frontmatter records the observed native hierarchy: name (H1), sections (H2), categories (H3), subordinate groups (H4), and body. At the reviewed default body size, the heading sizes resolve to 32, 24, 20, and 16 pixels; body line height resolves to 24 pixels. These are host defaults, not a promise that GitHub's CSS will remain fixed. Relative heading sizes preserve text scaling.

**The Semantic Hierarchy Rule.** Choose heading levels by document relationship; do not simulate headings with bold paragraphs.

## Layout

A single Markdown flow uses normal paragraphs and lists. GitHub provides the container and responsive behavior; this repository defines no grid, breakpoint, maximum width, or page padding. The 850-pixel desktop preview frame was a QA fixture, not a production layout token.

The inherited spacing tokens describe paragraph/list separation, space before headings, and gaps between adjacent list items. Inline links and badge groups wrap to the available width. Existing images remain responsive under GitHub's renderer.

## Elevation & Depth

The README adds no shadows or floating surfaces. Native heading dividers and quotation borders provide document structure; the host supplies focus and disclosure states.

## Shapes

Content follows text and list geometry. Badges retain their existing flat-square artwork. No project radius, card silhouette, or clipping system is authored.

## Components

### Heading tree

One name heading leads the document. Major sections use H2, peer project categories use H3 with one leading category emoji (🧩, 🛠️, 🎙️) and Agent Skills uses H4 beneath the linked Skills collection. The exact section order and project-first composition belong to the [surface brief](.impeccable/surfaces/readme-md.md).

### Project list

Each semantic list item pairs a bold linked project name with its existing description. The text flows on multiple lines without a card wrapper or a fixed row height.

### Disclosure and badge inventory

A native details/summary control starts open, since it sits below the project index and does not delay project discovery; readers can collapse it. Its visible label is “Tech stack & affiliations”; opening it reveals four labeled groups of inline badges. Preserve keyboard activation and normal flow when expanded.

### Quotations and external images

The short introduction and closing maxim use native blockquotes. Activity and contact images retain their existing URLs and alternative text. The build ships no new raster assets.

**The Native Interaction Rule.** Use ordinary anchors and details/summary so navigation and disclosure retain platform behavior.

## Do's and Don'ts

### Do:

- Do preserve the semantic heading tree and readable linked project lists.
- Do let prose, section links, and inline badge groups wrap naturally.
- Do retain meaningful image alt text and existing public image destinations.
- Do check expanded and collapsed disclosure states in light and dark themes.

### Don't:

- Don't prescribe a custom palette, font download, fixed document width, or authored animation for this GitHub-rendered surface.
- Don't replace native links or disclosure with image-only controls.
- Don't turn external badge colors into a profile-wide palette.
