# Tiara Brand Style Guide  
Official document. Effective 10 December 2025. No deviations permitted.

## Identity
Company name: Tiara  
The word Tiara is always written exactly as shown: first letter uppercase, the rest lowercase, using only English Latin characters even when the surrounding text is in another language or script.

Design language name: bored  
The word bored is always written exactly as shown: all lowercase English Latin characters, never translated, capitalised, or stylised, regardless of the language context.

Personal name: @thekzbn or Ayomide Deji-Adeyale or Deji-Adeyale Ayomide  
All forms use only English Latin characters. The @ symbol is required wherever technically possible. In Git repositories or systems that forbid the @ character, the handle is written thekzbn.  
In printed material or formal correspondence requiring surname-first order, the name is Deji-Adeyale Ayomide.  
Tiara stands alone; no suffix of any kind is ever added.  
No abbreviations, nicknames, or diminutives are ever used.

## Design Language
Name: bored  
Description: expensive nothingness. Royalty in silence. The user is king; the interface exists only to serve without drawing attention to itself.

The entire visual system is built on deliberate restraint. Nothing moves unless movement is required. Nothing is coloured unless colour is required. Ornament is absence.

## Colour System – The Golden Anchor
Defined once in root CSS. Never hard-coded elsewhere.

Light mode (default)
```css
--purity:   #ffffff;
--serenity: #f4ebd0;
--depth:    #122620;
--radiance: #d6ad60;
--heritage: #b68d40;
```

Dark mode (mandatory toggle on every product)
```css
--purity:   #121212;
--serenity: #2d2d2d;
--depth:    #f4ebd0;
--radiance: #d6ad60;
--heritage: #e6c97a;
```

--void (#121212) is retained as the deepest surface in both modes and may be used sparingly where extra visual weight is required.  
All contrast ratios meet or exceed WCAG 2.2 AA in both modes.

## Spacing – Revised December 2025
Strict six-step scale. Every margin, padding, gap, and separation must be exactly one of these values:

| Value     | Purpose                                      |
|-----------|----------------------------------------------|
| 0.25 rem  | Tiny inline gaps, icon-text spacing          |
| 0.5 rem   | Button padding, small form gaps              |
| 0.75 rem  | Standard component padding, paragraph margin-bottom |
| 1 rem     | Medium component groups, small sections      |
| 1.5 rem   | Major section breaks, container side padding |
| 3 rem     | Hero to content, full-page breaks only       |

All spacing is declared in rem only. Pixels are forbidden except for 1 px borders.

## Typography
Primary text: Inter Variable  
Code: JetBrains Mono Variable  

Inter is loaded with full variable axes and the following font-feature-settings applied globally in both modes:

```css
font-feature-settings: "cv01" 1, "cv02" 1, "cv03" 1, "cv04" 1, "cv05" 1,
                       "cv06" 1, "cv07" 1, "cv08" 1, "cv09" 1, "cv10" 1,
                       "cv11" 1, "cv12" 1, "cv13" 1, "cv14" 1,
                       "liga" 1, "calt" 1, "zero" 1;
```

Headings use weights 600 or 700 only, with letter-spacing -0.02 em to -0.03 em.  
Body text and paragraphs use weight 400 only.  
Sub-headings and lead paragraphs may use weight 500.  
No weight between 501 and 599 is ever used.  
Captions are 0.875 rem, weight 400 maximum.

## Motion and Interaction
The cubic-bezier(0.57, -0.01, 0.21, 0.89) and base duration of 0.5 s are absolute for all non-essential motion.  
Utility motion required for system feedback may use the same curve with durations between 0.3 s and 0.5 s.  
Motion is used only when its absence would reduce clarity. prefers-reduced-motion removes all non-essential motion.

## Component Geometry
Border radius values are restricted to 1 rem, 0.5 rem, or 0.25 rem according to element size.  
Drop shadows are never used under any circumstance.  
Maximum readable content width is 42.5 rem. All body text is constrained to this width with horizontal padding of at least 1.5 rem on desktop and 0.75 rem on screens below 640 px.  
Full-bleed sections are permitted only when the content is inherently visual or spatial and readability is not compromised.

## Components
Cards and containers are pure --purity with either no border or a single 1 px --serenity border.  
Links are coloured --radiance, never underlined, and shift to --heritage on hover.  
Form inputs have a bottom border or a full 1 px --serenity border. Labels do not float.  
All interactive elements receive visible focus styles that meet WCAG 2.4.7.  
ARIA attributes are applied correctly and never used as a substitute for semantic HTML.

## Code Requirements
Every line of code written for Tiara or @thekzbn must use rem for all spacing and sizing values. Pixels are permitted only for 1 px borders and focus rings.  
All interfaces meet WCAG 2.2 AA conformance in both light and dark modes. Semantic HTML is mandatory.

## Voice and Copy
Speech is measured, traditional, and direct. No sycophancy, exclamation, or embellishment is used. Sugar-coating is forbidden. Prose is preferred; bullet lists and numbered lists appear only when structurally unavoidable. The user is addressed as an adult of discernment.

## Authorised Marks and Favicons
All marks are served from cdn.thekzbn.name.ng and must be used exactly as provided. No recolouring, animation, or distortion is ever applied.

- Primary personal and Tiara company favicon / logo:  
  https://cdn.thekzbn.name.ng/assets/img/logo.png

- Library application favicon:  
  https://cdn.thekzbn.name.ng/assets/img/thekzbn%20library%20logo.svg

- Blog favicon:  
  https://cdn.thekzbn.name.ng/assets/img/thekzbn%20blog%20logo.svg

## Enforcement
Any new page, product, or document that does not conform exactly to this guide is rejected on sight. Tiara and @thekzbn present a single, unchanging face to the world. The bored system is the visual manifestation of that unity.

This document is final.
