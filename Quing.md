# Quing brand style guide

official document. effective january 2026. no deviations permitted.

---

## identity

the company name is **Quing**. it must always be written in title case using english latin characters only. no other variations, including lowercase or all-caps, are permitted.

the design language name is **slate**. it must always be written in all lowercase english latin characters. it is never capitalized, even at the beginning of a sentence, and must never be translated.

## design language

name: slate

description: slate is boilerplate for greatness. it represents the beginning of something deliberate and serious. the system is intentionally minimal but complete, pushing fundamentals to their limit. the interface exists only to serve the user, without drawing attention to itself. nothing moves unless required. nothing is coloured unless required. ornament is absent.

## colour system

| variable name  | light mode | dark mode | role                         |
| -------------- | ---------- | --------- | ---------------------------- |
| **start**      | #FFFFFF    | #151B25   | primary background / base    |
| **end**        | #151B25    | #FFFFFF   | brand accent / high emphasis |
| **cornflower** | #AEB8C4    | #3A4655   | secondary ui / borders       |
| **charcoal**   | #214358    | #7DA1B8   | primary text / contrast      |
| **ocean**      | #9CA6B8    | #4B596E   | secondary text / muted ui    |
| **alert**      | #FF6347    | #FF6347   | destructive actions / errors |
| **go**         | #3CB371    | #3CB371   | success states               |

### css variables

```css
:root[data-theme="light"] {
  --start: #FFFFFF;
  --end: #151B25;
  --cornflower: #AEB8C4;
  --charcoal: #214358;
  --ocean: #9CA6B8;
  --alert: #FF6347;
  --go: #3CB371;
}

:root[data-theme="dark"] {
  --start: #151B25;
  --end: #FFFFFF;
  --cornflower: #3A4655;
  --charcoal: #7DA1B8;
  --ocean: #4B596E;
  --alert: #FF6347;
  --go: #3CB371;
}
```

## spacing

spacing follows a strict six-step scale. all spacing values are declared in rem. pixels are forbidden except for 1 px borders.

| value    | purpose              |
| -------- | -------------------- |
| 0.25 rem | tiny inline gaps     |
| 0.5 rem  | button padding       |
| 0.75 rem | component padding    |
| 1 rem    | grouped components   |
| 1.5 rem  | section breaks       |
| 3 rem    | full-page separation |

## typography

primary ui typeface: inter variable

conditional serif typeface: merriweather

code typeface: jetbrains mono variable

### usage rules

inter variable is the default typeface for all ui, navigation, labels, metadata, and article body text.

users may be offered a reading preference toggle between sans-serif and serif.

when and only when the user explicitly selects serif, merriweather is used for article body text.

merriweather is never used for ui, navigation, controls, captions, headings, or metadata.

if no user choice exists, merriweather must not load or render.

jetbrains mono variable is used exclusively for code, technical identifiers, and monospace contexts.

### font loading

````css
@font-face {
  font-family: 'Inter Variable';
  src: url('https://cdn.thekzbn.name.ng/assets/font/InterVariable.woff2') format('woff2'),
       url('https://cdn.thekzbn.name.ng/assets/font/InterVariable.ttf') format('truetype');
  font-weight: 100 900;
  font-style: normal;
  font-display: swap;
}

@font-face {
  font-family: 'Inter Variable';
  src: url('https://cdn.thekzbn.name.ng/assets/font/InterVariable-Italic.woff2') format('woff2'),
       url('https://cdn.thekzbn.name.ng/assets/font/InterVariable-Italic.ttf') format('truetype');
  font-weight: 100 900;
  font-style: italic;
  font-display: swap;
}

@font-face {
  font-family: 'Merriweather';
  src: url('https://fonts.googleapis.com/css2?family=Merriweather:ital,wght@0,300..900;1,300..900&display=swap');
  font-weight: 300 900;
  font-style: normal;
  font-display: swap;
}

@font-face {
  font-family: 'JetBrains Mono Variable';
  src: url('https://fonts.googleapis.com/css2?family=JetBrains+Mono:wght@100..800&display=swap');
  font-weight: 100 800;
  font-style: normal;
  font-display: swap;
}

@font-face {
  font-family: 'JetBrains Mono Variable';
  src: url('https://fonts.googleapis.com/css2?family=JetBrains+Mono:wght@100..800&display=swap');
  font-weight: 100 800;
  font-style: normal;
  font-display: swap;
}

```
### hierarchy

headings and headers are written in lowercase only, except for required brand names.

h1 minimum size is 4 rem and used with extreme scarcity.

heading weights are restricted to 600 or 700.

body text uses weight 400 only.

no weight between 501 and 599 is ever used.

## motion and interaction

all non-essential motion uses cubic-bezier(0.57, -0.01, 0.21, 0.89) with a base duration of 0.5 s.

prefers-reduced-motion removes all non-essential motion.

## component geometry

border radius values are restricted to 1 rem, 0.5 rem, or 0.25 rem.

drop shadows are never used.

maximum readable content width is 42.5 rem.

## components

cards use --start with either no border or a single 1 px --cornflower border.

links are coloured --end and never underlined.

all interactive elements receive visible focus styles meeting wcag 2.4.7.

## code requirements

semantic html is mandatory.

all interfaces must meet wcag 2.2 aa.

## voice and copy

tone is measured, traditional, and direct.

sycophancy and embellishment are forbidden.

## authorised marks and favicons

the following marks are the only permitted visual identifiers for **Quing**. they must be rendered in **--end** on a **--start** background.

* **primary mark:** [Quing Logo](https://cdn.thekzbn.name.ng/assets/img/Quing%20Logo.svg)
* **wordmark:** [Quing Long Logo](https://cdn.thekzbn.name.ng/assets/img/Quing%20Long%20Logo.svg)

## enforcement

strict enforcement applies to all assets and communications. any deviation constitutes a brand violation.
