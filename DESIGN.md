---
name: Cinematic Brutalist
colors:
  surface: '#131313'
  surface-dim: '#131313'
  surface-bright: '#393939'
  surface-container-lowest: '#0e0e0e'
  surface-container-low: '#1c1b1b'
  surface-container: '#201f1f'
  surface-container-high: '#2a2a2a'
  surface-container-highest: '#353534'
  on-surface: '#e5e2e1'
  on-surface-variant: '#e6beb2'
  inverse-surface: '#e5e2e1'
  inverse-on-surface: '#313030'
  outline: '#ad897e'
  outline-variant: '#5c4037'
  surface-tint: '#ffb59e'
  primary: '#ffb59e'
  on-primary: '#5e1700'
  primary-container: '#ff571a'
  on-primary-container: '#521300'
  inverse-primary: '#ae3200'
  secondary: '#e6feff'
  on-secondary: '#003739'
  secondary-container: '#00f4fe'
  on-secondary-container: '#006c71'
  tertiary: '#a5c8ff'
  on-tertiary: '#00315e'
  tertiary-container: '#2492ff'
  on-tertiary-container: '#002a53'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#ffdbd0'
  primary-fixed-dim: '#ffb59e'
  on-primary-fixed: '#3a0b00'
  on-primary-fixed-variant: '#852400'
  secondary-fixed: '#63f7ff'
  secondary-fixed-dim: '#00dce5'
  on-secondary-fixed: '#002021'
  on-secondary-fixed-variant: '#004f53'
  tertiary-fixed: '#d4e3ff'
  tertiary-fixed-dim: '#a5c8ff'
  on-tertiary-fixed: '#001c3a'
  on-tertiary-fixed-variant: '#004785'
  background: '#131313'
  on-background: '#e5e2e1'
  surface-variant: '#353534'
typography:
  display-xl:
    fontFamily: Bricolage Grotesque
    fontSize: 120px
    fontWeight: '800'
    lineHeight: 110px
    letterSpacing: -0.04em
  headline-lg:
    fontFamily: Bricolage Grotesque
    fontSize: 64px
    fontWeight: '800'
    lineHeight: 72px
    letterSpacing: -0.02em
  headline-lg-mobile:
    fontFamily: Bricolage Grotesque
    fontSize: 40px
    fontWeight: '800'
    lineHeight: 44px
  body-md:
    fontFamily: Hanken Grotesk
    fontSize: 18px
    fontWeight: '400'
    lineHeight: 28px
  label-mono:
    fontFamily: JetBrains Mono
    fontSize: 14px
    fontWeight: '500'
    lineHeight: 20px
    letterSpacing: 0.05em
spacing:
  frame-border: 24px
  gutter: 32px
  section-gap: 160px
  container-max: 1440px
---

## Brand & Style

This design system is built on the intersection of **High-Contrast Brutalism** and **Cinematic Premium** aesthetics. It rejects the "safe" corporate look in favor of an absurd, ultra-bold presence that reflects the fluidity of the logo and the irreverence of the skating dinosaur mascot.

The personality is unapologetically loud, technical yet playful, and deeply immersive. We use "frame-within-a-frame" compositions to evoke a directorial lens, making every section of the web experience feel like a curated shot. Large-scale typography and thick, structural borders define the space, creating a physical sense of weight and permanence.

## Colors

The palette is anchored in a deep **#121212 Charcoal**, providing a cinematic "blackout" canvas that allows vibrant accents to vibrate off the screen. 

- **Primary (Vibrant Orange):** Used for critical calls to action and to mirror the energy of the brand mascot.
- **Secondary (Electric Teal):** Used for technical highlights, code snippets, and interactive states to provide a high-contrast counterpoint to the orange.
- **Accents:** Pure white (#FFFFFF) is reserved for primary text and thick structural borders to maintain a crisp, premium feel. 
- **Surface Strategy:** Backgrounds should remain dark; use subtle variations of charcoal (#1A1A1A) for card surfaces to maintain depth without breaking the immersion.

## Typography

The typography strategy relies on extreme contrast in scale and character.

- **Headlines:** We use **Bricolage Grotesque** at its heaviest weights. Its quirky, fluid terminals echo the "BARBARY" logo's custom letterforms. Use `display-xl` for hero sections, often allowing text to overlap images slightly for a more "designed" editorial look.
- **Body:** **Hanken Grotesk** provides a sharp, contemporary, and highly legible balance to the expressive headlines. It keeps the professional "web development" aspect grounded.
- **Utility:** **JetBrains Mono** is used for labels, navigation items, and technical data, reinforcing the developer-centric nature of the business with a "raw code" aesthetic.

## Layout & Spacing

The layout utilizes a **"Letterbox" fixed-grid system**. Every page is treated like a cinematic frame, often wrapped in a consistent 24px outer border that acts as a physical window.

- **Grid:** A 12-column layout with wide 32px gutters to prevent the bold typography from feeling cramped.
- **Frame-within-a-frame:** Use inset containers with thick 4px borders to group content. These containers should have generous internal padding (64px+) to create a "premium gallery" feel.
- **Rhythm:** Vertical spacing is intentionally aggressive (`section-gap`). We favor "dead space" to allow the skating dinosaur and logo assets to stand as focal points without distraction.

## Elevation & Depth

This system avoids soft shadows and traditional depth metaphors. Instead, it uses **Structural Layering**:

- **Hard Borders:** Depth is communicated through 4px or 8px solid borders. Elements don't "float"; they are "contained."
- **High-Contrast Overlays:** When an element needs to sit above the main content (like a modal or dropdown), it uses a solid #121212 background with a vibrant #FF4D00 border.
- **The "Glass Box" exception:** For technical readouts, a very slight backdrop blur (8px) with a 10% white opacity can be used to simulate a high-tech HUD, but it must be framed in a thick, solid stroke.

## Shapes

The shape language is strictly **Sharp (0px)**. 

To match the "ultra-bold" and "brutalist" narrative, all buttons, cards, and containers must have hard 90-degree corners. This creates a architectural, rigid structure that contrasts beautifully with the fluid, organic strokes found in the BARBARY logo and the mascot illustrations. The only curves permitted are those inherent in the typography and the brand artwork itself.

## Components

### Buttons
Primary buttons are large, rectangular blocks of **Electric Teal** or **Vibrant Orange** with black text. On hover, they should shift to a "negative" state (Black background with colored border and text). Use a 4px offset "hard shadow" (solid color block) to give them a tactile, clickable weight.

### Input Fields
Fields are defined by a bottom-border only (4px thickness). When focused, the border color transitions from white to the primary accent color. Labels use the `label-mono` style, positioned strictly above the field.

### Cards
Cards are "Frames." They must have a 2px or 4px white border. Titles inside cards should be `headline-sm` to maintain the hierarchy of "Boldness First."

### Chips/Tags
Small, monochromatic boxes with a 1px border. Use `label-mono` for the text. These act as the "metadata" of the design, looking like technical specs on a blueprint.

### Image Treatment
All images, including the skating dinosaur, should be treated as "Objects." Use heavy masking or place them within "Frame" containers. Never use rounded corners on image assets.