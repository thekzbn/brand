# Tiara Brand Style Guide  
Official document. Effective 9 December 2025. No deviations permitted.

## Identity
Company name: Tiara  
Personal name: @thekzbn or Ayomide Deji-Adeyale or Deji-Adeyale Ayomide  
No other spelling, handle, or order is ever used.

## Design Language
Name: bored  
Description: expensive nothingness. Royalty in silence. The user is king; the interface exists only to serve without drawing attention to itself.

The entire visual system is built on deliberate restraint. Nothing moves unless movement is required. Nothing is coloured unless colour is required. Ornament is absence.

## Colour System – The Golden Anchor
Defined once in root CSS. Never hard-coded elsewhere.

```css
--purity:   #ffffff;  /* all backgrounds and surfaces */
--serenity: #f4ebd0;  /* borders, code backgrounds, dividers */
--depth:    #122620;  /* all text and icons in resting state */
--radiance: #d6ad60;  /* sole accent, used once or twice per screen at most */
--heritage: #b68d40;  /* hover state for radiance only */
--void:     #121212;  /* emergency deep background only */
```

## Spacing
Base unit is 1.5 rem. Every padding, margin, gap, and section separation is an exact multiple of 1.5 rem. No exceptions or approximations are tolerated.

## Typography
Primary text: Inter Variable  
Code: JetBrains Mono Variable  

Inter is loaded with full variable axes and the following font-feature-settings applied globally:

```css
font-feature-settings: "cv01" 1, "cv02" 1, "cv03" 1, "cv04" 1, "cv05" 1,
                       "cv06" 1, "cv07" 1, "cv08" 1, "cv09" 1, "cv10" 1,
                       "cv11" 1, "cv12" 1, "cv13" 1, "cv14" 1,
                       "liga" 1, "calt" 1, "zero" 1;
```

Headings use weights 600 or 700 only, with letter-spacing between -0.02 em and -0.03 em.  
Body text is 1 rem with exactly 1.5 line height.  
Captions are 0.875 rem, weight 400 maximum.

## Motion and Interaction
Global transition: all 0.5s cubic-bezier(0.57, -0.01, 0.21, 0.89)  
Hover changes colour only: radiance becomes heritage. No scale, lift, or shadow change occurs.  
Loading indicators rotate slowly or remain static.  
No skeletons, parallax, scroll-triggered animation, or micro-interactions are permitted.

## Components
Cards and containers are pure --purity with either no border or a single 1 px --serenity border.  
Links are coloured --radiance, never underlined, and shift to --heritage on hover.  
Form inputs have a bottom border or a full 1 px --serenity border. Labels do not float.  
Avatars never exceed 40 px in diameter.  
Icons are monochrome until active, then coloured --radiance.  
Dark mode is not offered.

## Voice and Copy
Speech is measured, traditional, and direct. No sycophancy, exclamation, or embellishment is used. Sugar-coating is forbidden. Prose is preferred; bullet lists and numbered lists appear only when structurally unavoidable. The user is addressed as an adult of discernment.

## Favicon and Marks
Favicon: https://thekzbn.name.ng/assets/img/thekzbn blog logo.svg  
No other marks or logotypes are authorised at this time.

## Enforcement
Any new page, product, or document that does not conform exactly to this guide is rejected on sight. Tiara and @thekzbn present a single, unchanging face to the world. The bored system is the visual manifestation of that unity.

This document is final.
