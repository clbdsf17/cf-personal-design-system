# CF Personal — Design System

The personal-brand design system for Celso Filho. **Editorial, confident, warm.**

Derived from a three-screen onboarding reference, its governing rule is
**black acts, color expresses**: neutral carries every interaction, and the
expressive palette never touches a control.

---

## Files

| File | Audience | What it is |
|---|---|---|
| **`design.md`** | coding agents | **Source of truth.** YAML tokens in [Google's design.md format](https://github.com/google-labs-code/design.md) + prose rationale. |
| **`design.html`** | humans | Self-contained style guide. Open in a browser; has a light/dark toggle. |
| **`tokens.css`** | any HTML output | Drop-in stylesheet — all 96 tokens as CSS custom properties, plus `.t-*` type utilities. Generated from `design.html`. |
| **`artboard-starter.dc.html`** | Claude Design | Starting skeleton for a `.dc.html` artboard: fonts linked, tokens inlined, primitives pre-built. |

`design.md` is canonical. `design.html` mirrors it, and `tokens.css` is generated
from `design.html` — **never hand-edit `tokens.css`**; regenerate it instead.

---

## Quick start

For any self-contained page (Claude Design artboard, Artifact, standalone HTML):

```html
<link href="https://fonts.googleapis.com/css2?family=Barlow:wght@600;700;800&family=Inter:wght@400;600&display=swap" rel="stylesheet">
<style>
  /* paste the entire contents of tokens.css here */
</style>

<button class="btn">Primary action</button>
```

Or copy `artboard-starter.dc.html` and replace everything below the
`<!-- REPLACE BELOW -->` marker.

Artboards share no stylesheet — **each one carries its own copy of the tokens.**
Keep that block byte-identical across a canvas so it stays one system.

---

## The seven rules

1. **Black acts, color expresses.** `action` (`#0D0D0D` light / `#F4F3F1` dark) is
   the only color a button, link, or control may take. Mint, amber, violet, and
   orange never touch an interactive surface.
2. **Radius is `0px` or `9999px`. Nothing between.** A 4px radius is a bug, not a
   judgment call. `9999px` is only for genuinely circular things.
3. **No shadows, gradients, glows, blurs, or glassmorphism.** Depth is surface
   contrast plus 1px borders. Hover sharpens a border; it never lifts an element.
4. **One expressive color per composition**, as large geometry — never two competing,
   never as small decoration.
5. **Where a shape crosses a photo, the overlap goes `#2B22F0`** via
   `mix-blend-mode: multiply`. This is the signature that ties the family together.
6. **Barlow (display) + Inter (everything else).** Barlow only at 600–800, only above
   22px, tracked `-0.01em` to `-0.02em` — never tighter, because Barlow is already
   narrow and harder tracking collides its squared terminals. Never Barlow for body copy.
7. **`label` type is always uppercase** — Inter 11px / 600 / `0.18em` tracking. The
   system's signature detail: buttons, field labels, eyebrows.

### Never let this become

Generic SaaS (rounded-everything, gradient buttons, soft shadows) · accent soup ·
decorative clutter · display type leaking into body copy.

---

## Accessibility

Every text color meets WCAG AA on its intended background — `on-surface` at 17.5:1,
`on-surface-muted` at 4.8:1, all semantic colors at 4.8:1 or better.

`on-surface-subtle` (`#8F8F89`) sits at 3.4:1 and is restricted to **disabled states
and non-essential decoration — never body copy.**

---

## Editing

`design.md` and `design.html` must be updated **in the same edit** — they are mirrors
and must never drift. After changing either, regenerate `tokens.css` from
`design.html` so the drop-in stylesheet stays in sync.

Preserve the canonical section order in `design.md` and never create duplicate `##`
headings — the design.md spec rejects files with duplicates.
