---
version: alpha
name: CF Personal
description: An editorial, confident, warm personal-brand system where black acts and color expresses.

colors:
  # --- Canvas & content (light) ---
  background: "#F4F3F1"
  surface: "#FFFFFF"
  surface-sunken: "#EAE8E4"
  on-background: "#0D0D0D"
  on-surface: "#0D0D0D"
  on-surface-muted: "#6B6B66"
  on-surface-subtle: "#8F8F89"
  border: "#DFDDD8"
  border-strong: "#0D0D0D"

  # --- Action (black acts) ---
  action: "#0D0D0D"
  on-action: "#FFFFFF"
  action-hover: "#262626"
  action-active: "#000000"
  action-disabled: "#C9C7C2"
  on-action-disabled: "#8F8F89"
  focus: "#2B22F0"

  # --- Expressive (color expresses; never on a control) ---
  expressive-mint: "#3ED9C0"
  expressive-amber: "#FFC53D"
  expressive-violet: "#B24BF3"
  expressive-orange: "#F97316"
  expressive-overlap: "#2B22F0"

  # --- Semantic ---
  success: "#15795A"
  warning: "#8A5A00"
  error: "#C42B1C"
  info: "#2B22F0"

  # --- Dark mode ---
  dark-background: "#0D0D0C"
  dark-surface: "#1A1A18"
  dark-surface-sunken: "#000000"
  dark-on-background: "#F4F3F1"
  dark-on-surface: "#F4F3F1"
  dark-on-surface-muted: "#A3A29C"
  dark-on-surface-subtle: "#6E6D68"
  dark-border: "#2E2E2B"
  dark-border-strong: "#F4F3F1"
  dark-action: "#F4F3F1"
  dark-on-action: "#0D0D0C"
  dark-action-hover: "#FFFFFF"
  dark-action-active: "#DAD8D3"
  dark-action-disabled: "#3A3A36"
  dark-on-action-disabled: "#6E6D68"
  dark-focus: "#6B63FF"
  dark-expressive-mint: "#4FE8CF"
  dark-expressive-amber: "#FFD166"
  dark-expressive-violet: "#C77BFF"
  dark-expressive-orange: "#FF8A3D"
  dark-expressive-overlap: "#6B63FF"
  dark-success: "#3FD69A"
  dark-warning: "#FFC53D"
  dark-error: "#FF6B5A"
  dark-info: "#6B63FF"

typography:
  display:
    fontFamily: Barlow
    fontSize: 64px
    fontWeight: 800
    lineHeight: 0.95
    letterSpacing: -0.02em
  h1:
    fontFamily: Barlow
    fontSize: 44px
    fontWeight: 800
    lineHeight: 1.02
    letterSpacing: -0.02em
  h2:
    fontFamily: Barlow
    fontSize: 32px
    fontWeight: 700
    lineHeight: 1.1
    letterSpacing: -0.015em
  h3:
    fontFamily: Barlow
    fontSize: 22px
    fontWeight: 700
    lineHeight: 1.2
    letterSpacing: -0.01em
  body-lg:
    fontFamily: Inter
    fontSize: 19px
    fontWeight: 400
    lineHeight: 1.65
    letterSpacing: -0.005em
  body:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.7
    letterSpacing: 0em
  body-sm:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.6
    letterSpacing: 0em
  caption:
    fontFamily: Inter
    fontSize: 13px
    fontWeight: 400
    lineHeight: 1.5
    letterSpacing: 0.01em
  label:
    fontFamily: Inter
    fontSize: 11px
    fontWeight: 600
    lineHeight: 1.2
    letterSpacing: 0.18em
  quote:
    fontFamily: Barlow
    fontSize: 26px
    fontWeight: 600
    lineHeight: 1.35
    letterSpacing: -0.01em
  code:
    fontFamily: ui-monospace
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.6
    letterSpacing: 0em

rounded:
  none: 0px
  full: 9999px

spacing:
  0: 0px
  1: 4px
  2: 8px
  3: 12px
  4: 16px
  5: 24px
  6: 32px
  7: 48px
  8: 64px
  9: 96px
  10: 128px

components:
  button-primary:
    backgroundColor: "{colors.action}"
    textColor: "{colors.on-action}"
    typography: "{typography.label}"
    rounded: "{rounded.none}"
    padding: "{spacing.5}"
    height: 52px
  button-primary-hover:
    backgroundColor: "{colors.action-hover}"
    textColor: "{colors.on-action}"
    typography: "{typography.label}"
    rounded: "{rounded.none}"
    padding: "{spacing.5}"
    height: 52px
  button-primary-active:
    backgroundColor: "{colors.action-active}"
    textColor: "{colors.on-action}"
    typography: "{typography.label}"
    rounded: "{rounded.none}"
    padding: "{spacing.5}"
    height: 52px
  button-primary-disabled:
    backgroundColor: "{colors.action-disabled}"
    textColor: "{colors.on-action-disabled}"
    typography: "{typography.label}"
    rounded: "{rounded.none}"
    padding: "{spacing.5}"
    height: 52px
  button-primary-focus:
    backgroundColor: "{colors.action}"
    textColor: "{colors.on-action}"
    typography: "{typography.label}"
    rounded: "{rounded.none}"
    padding: "{spacing.5}"
    height: 52px
  button-ghost:
    backgroundColor: "{colors.background}"
    textColor: "{colors.action}"
    typography: "{typography.label}"
    rounded: "{rounded.none}"
    padding: "{spacing.5}"
    height: 52px
  button-ghost-hover:
    backgroundColor: "{colors.action}"
    textColor: "{colors.on-action}"
    typography: "{typography.label}"
    rounded: "{rounded.none}"
    padding: "{spacing.5}"
    height: 52px
  button-micro:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label}"
    rounded: "{rounded.none}"
    padding: "{spacing.2}"
    height: 28px
  button-micro-hover:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface-muted}"
    typography: "{typography.label}"
    rounded: "{rounded.none}"
    padding: "{spacing.2}"
    height: 28px
  link:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body}"
    rounded: "{rounded.none}"
    padding: "{spacing.0}"
  link-hover:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface-muted}"
    typography: "{typography.body}"
    rounded: "{rounded.none}"
    padding: "{spacing.0}"
  card:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body}"
    rounded: "{rounded.none}"
    padding: "{spacing.6}"
  card-hover:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body}"
    rounded: "{rounded.none}"
    padding: "{spacing.6}"
  divider:
    backgroundColor: "{colors.border}"
    rounded: "{rounded.none}"
    height: 1px
    width: 100%
  pull-quote:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface}"
    typography: "{typography.quote}"
    rounded: "{rounded.none}"
    padding: "{spacing.6}"
  callout:
    backgroundColor: "{colors.surface-sunken}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body}"
    rounded: "{rounded.none}"
    padding: "{spacing.5}"
  figure-caption:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface-muted}"
    typography: "{typography.caption}"
    rounded: "{rounded.none}"
    padding: "{spacing.3}"
  input:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body}"
    rounded: "{rounded.none}"
    padding: "{spacing.4}"
    height: 52px
  input-focus:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body}"
    rounded: "{rounded.none}"
    padding: "{spacing.4}"
    height: 52px
  input-error:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body}"
    rounded: "{rounded.none}"
    padding: "{spacing.4}"
    height: 52px
  input-disabled:
    backgroundColor: "{colors.surface-sunken}"
    textColor: "{colors.on-surface-subtle}"
    typography: "{typography.body}"
    rounded: "{rounded.none}"
    padding: "{spacing.4}"
    height: 52px
  textarea:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body}"
    rounded: "{rounded.none}"
    padding: "{spacing.4}"
    height: 144px
  select:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body}"
    rounded: "{rounded.none}"
    padding: "{spacing.4}"
    height: 52px
  checkbox:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.none}"
    size: 20px
  checkbox-checked:
    backgroundColor: "{colors.action}"
    textColor: "{colors.on-action}"
    rounded: "{rounded.none}"
    size: 20px
  field-label:
    backgroundColor: "{colors.background}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label}"
    rounded: "{rounded.none}"
    padding: "{spacing.0}"
  pagination-dot:
    backgroundColor: "{colors.action-disabled}"
    rounded: "{rounded.full}"
    size: 7px
  pagination-dot-active:
    backgroundColor: "{colors.action}"
    rounded: "{rounded.full}"
    size: 7px
  badge:
    backgroundColor: "{colors.action}"
    textColor: "{colors.on-action}"
    typography: "{typography.label}"
    rounded: "{rounded.none}"
    padding: "{spacing.2}"
    height: 24px
---

# CF Personal Design System

## Overview

CF Personal is the personal-brand system for Celso Filho — used across writing, lead magnets, decks, and product surfaces. It should feel **editorial, confident, and warm**: authored by a person with a point of view, unhedged in its contrast, but never cold or corporate.

The system is derived from a three-screen onboarding reference whose defining logic was not its palette but its *restraint*: a flat warm-off-white plane, zero corner radius, no shadows, and a hard black call-to-action surrounded by pure geometric color. The single most important rule inherited from it is **black acts, color expresses**. Neutral carries every interaction; the expressive palette never touches a control.

Two anti-patterns govern everything below: this must never become Generic SaaS (rounded corners, gradient buttons, soft shadows), and the expressive colors must never turn into accent soup.

## Colors

The canvas is a warm off-white (`background` `#F4F3F1`), not pure white — it is what keeps a stark, high-contrast system from reading as clinical. `surface` `#FFFFFF` sits *above* it: elevation here is a contrast relationship, not a shadow.

Interaction is monochrome. `action` `#0D0D0D` is the only color a button, link, or control may take; it lightens to `action-hover` `#262626` and deepens to `action-active` `#000000`. In dark mode this inverts rather than breaks — `dark-action` becomes `#F4F3F1`, preserving the rule as *maximum-contrast neutral acts*.

The expressive palette — mint `#3ED9C0`, amber `#FFC53D`, violet `#B24BF3`, orange `#F97316` — exists only for large graphic geometry and image treatment. Use **one per composition**, never two competing in the same view. `expressive-overlap` `#2B22F0` is the electric blue that appears where a shape crosses a photograph, a multiply-blend duotone; it is the connective tissue that makes compositions with different accents read as one family.

`focus` `#2B22F0` is a deliberate exception to "black acts": a black focus ring is invisible on a black button, and the overlap blue is already the system's voice for *the system speaking* rather than *the user acting*. It scores 7.3:1 on the light canvas.

All text colors meet WCAG AA on their intended background: `on-surface` at 17.5:1, `on-surface-muted` `#6B6B66` at 4.8:1, and every semantic color at 4.8:1 or better. `on-surface-subtle` `#8F8F89` sits at 3.4:1 and is therefore restricted to disabled states and non-essential decoration — never body copy. Note that the reference's own light-gray body text fails AA; `on-surface-muted` is the corrected value.

## Typography

Barlow sets display and headings; Inter sets everything else. Barlow is a slightly condensed grotesk with squared terminals and a low-contrast, engineered character — narrower and more technical than Inter, which gives the pairing a genuine width contrast to work with. Even so, **hierarchy should not lean on family contrast alone** — it comes from weight, tracking, case, and aggressive scale jumps.

Barlow earns its place at 800 weight with tight line-height and *moderate* negative tracking. `display` (64px / 800 / 0.95 / -0.02em) and `h1` (44px / 800 / -0.02em) are heavy and compressed on purpose. Note the tracking is deliberately half what a wide geometric like Montserrat would need: Barlow is already narrow, so aggressive negative tracking collides its squared terminals and destroys legibility at display sizes. Never set Barlow below 600 weight, and never at positive tracking.

Inter handles body, captions, and the system's signature detail: `label` — 11px, 600 weight, `0.18em` tracking, always rendered uppercase. This is the `SKIP` / `DONE` / `LET'S GO!` micro-type from the reference, and it appears on every button, field label, and eyebrow. Because the design.md schema has no `textTransform` property, the uppercase transform is a documented rule rather than a token value; apply `text-transform: uppercase` wherever `label` is used.

Body copy runs generous (`body` at 1.7 line-height) to hold the editorial feel at long lengths. `quote` uses Barlow at 600 to let a pull-quote read as display without competing with a heading.

## Layout

Spacing is an 8px base with a deliberately non-linear top end: `4 8 12 16 24 32 48 64 96 128`. The large steps matter more than the small ones — the reference's character came from the *voids*, particularly the wide gap between hero imagery and headline.

The rhythm is: large void, tight cluster, large void. A headline and its body copy sit close (`spacing.4`, 16px); the group is then separated from what surrounds it by `spacing.8` or `spacing.9` (64–96px). Resist the urge to even out these gaps — uniform spacing is what makes a layout read as a template.

Content containers max out around 680px for long-form reading and 1200px for index and marketing layouts, centered, with `spacing.6` (32px) gutters on desktop and `spacing.5` (24px) on mobile.

## Elevation & Depth

There is no shadow scale. Depth is expressed through **surface contrast and 1px borders only**.

A card lifts off the canvas by being `surface` `#FFFFFF` against `background` `#F4F3F1` — a quiet, ~4% luminance step that reads as separation without any blur. A recessed element uses `surface-sunken` `#EAE8E4`. Where more definition is needed, a 1px `border` `#DFDDD8` does the work; where emphasis is needed, `border-strong` `#0D0D0D` at 1–2px.

Hover on a card does not raise it — it *sharpens* it, swapping `border` for `border-strong`. This keeps the plane flat while still confirming interactivity. Note that the design.md component schema has no border property, so border values are specified here in prose and implemented directly in `design.html`.

## Shapes

`rounded` has exactly two values: `none` (0px) and `full` (9999px). There is no `sm`, no `md`, no "slightly rounded" — the omission is the enforcement mechanism.

Everything rectangular is sharp: buttons, inputs, cards, badges, images. `full` is reserved for things that are genuinely circular, principally the pagination dot. A 4px or 8px radius anywhere in this system is a bug, not a judgment call.

Sharp corners signal editorial confidence and print heritage; they are also what most reliably keeps the system out of Generic SaaS territory, since rounding is the default gesture of nearly every UI framework and code generator.

## Components

`button-primary` is a solid `action` rectangle, 52px tall, with white `label` type — uppercase, 11px, 0.18em tracked. It is the only high-emphasis control. `button-ghost` inverts on hover to solid black rather than tinting, keeping the palette binary. `button-micro` is the bare `SKIP` / `DONE` affordance: label type on the canvas with no container, dimming to `on-surface-muted` on hover.

Every focusable component takes a 2px `focus` ring at 2px offset. `button-primary-focus` shares its fill with the default state — only the ring changes.

Inputs are 52px, sharp, `surface`-filled with a 1px `border`. On focus the border goes to `border-strong` and the focus ring appears; on error the border takes `error` and the message below uses `body-sm` in `error`. Field labels always use `field-label` (uppercase `label` type), never sentence-case body.

Editorial components carry the writing: `pull-quote` uses `quote` type with a 2px `border-strong` left rule and no background fill; `callout` is a `surface-sunken` block with no border; `figure-caption` is `caption` type in `on-surface-muted`.

`card` is `surface` on `background` with `spacing.6` padding and a 1px `border`; `card-hover` swaps to `border-strong`. Expressive color may appear *inside* a card as imagery or a geometric block, but never as the card's own fill or border.

## Do's and Don'ts

**Do**

- Use `action` (black in light, off-white in dark) for every button, link, and control — no exceptions.
- Pick exactly one expressive color per composition, and let it appear as large geometry, not small decoration.
- Use `expressive-overlap` blue wherever a shape crosses a photograph, as a multiply blend — it is what ties the family together.
- Set Barlow at 700–800 with moderate negative tracking (-0.01em to -0.02em); keep it above 22px.
- Render `label` type in uppercase everywhere it appears.
- Vary spacing deliberately — tight clusters separated by large voids.

**Don't**

- Don't apply any corner radius other than `none` or `full`. A 4px radius is a bug.
- Don't put an expressive color on a button, link, chip, or any interactive surface.
- Don't add shadows, gradients, glows, blurs, glassmorphism, or illustrated blobs — depth is contrast and borders only.
- Don't run two or more expressive colors in the same view.
- Don't use Barlow for body copy, captions, table cells, or anything under 22px; don't use it below 600 weight, and don't track it tighter than -0.02em.
- Don't use `on-surface-subtle` for body copy — it fails WCAG AA and exists only for disabled states.
