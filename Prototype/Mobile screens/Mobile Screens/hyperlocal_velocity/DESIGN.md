---
name: Hyperlocal Velocity
colors:
  surface: '#f8f9ff'
  surface-dim: '#cbdbf5'
  surface-bright: '#f8f9ff'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#eff4ff'
  surface-container: '#e5eeff'
  surface-container-high: '#dce9ff'
  surface-container-highest: '#d3e4fe'
  on-surface: '#0b1c30'
  on-surface-variant: '#3f4a3c'
  inverse-surface: '#213145'
  inverse-on-surface: '#eaf1ff'
  outline: '#6f7a6a'
  outline-variant: '#becab7'
  surface-tint: '#006e16'
  primary: '#006714'
  on-primary: '#ffffff'
  primary-container: '#0c831f'
  on-primary-container: '#e0ffd7'
  inverse-primary: '#74dd6e'
  secondary: '#565e74'
  on-secondary: '#ffffff'
  secondary-container: '#dae2fd'
  on-secondary-container: '#5c647a'
  tertiary: '#755b00'
  on-tertiary: '#ffffff'
  tertiary-container: '#cfa620'
  on-tertiary-container: '#4f3d00'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#8ffb87'
  primary-fixed-dim: '#74dd6e'
  on-primary-fixed: '#002203'
  on-primary-fixed-variant: '#00530e'
  secondary-fixed: '#dae2fd'
  secondary-fixed-dim: '#bec6e0'
  on-secondary-fixed: '#131b2e'
  on-secondary-fixed-variant: '#3f465c'
  tertiary-fixed: '#ffe08f'
  tertiary-fixed-dim: '#edc13d'
  on-tertiary-fixed: '#241a00'
  on-tertiary-fixed-variant: '#584400'
  background: '#f8f9ff'
  on-background: '#0b1c30'
  surface-variant: '#d3e4fe'
typography:
  headline-xl:
    fontFamily: Plus Jakarta Sans
    fontSize: 36px
    fontWeight: '800'
    lineHeight: 44px
    letterSpacing: -0.03em
  headline-xl-mobile:
    fontFamily: Plus Jakarta Sans
    fontSize: 28px
    fontWeight: '800'
    lineHeight: 34px
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Plus Jakarta Sans
    fontSize: 24px
    fontWeight: '700'
    lineHeight: 32px
    letterSpacing: -0.02em
  headline-md:
    fontFamily: Plus Jakarta Sans
    fontSize: 20px
    fontWeight: '700'
    lineHeight: 28px
    letterSpacing: -0.015em
  headline-sm:
    fontFamily: Plus Jakarta Sans
    fontSize: 16px
    fontWeight: '700'
    lineHeight: 22px
    letterSpacing: -0.01em
  body-lg:
    fontFamily: Plus Jakarta Sans
    fontSize: 16px
    fontWeight: '500'
    lineHeight: 24px
  body-md:
    fontFamily: Plus Jakarta Sans
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 20px
  body-sm:
    fontFamily: Plus Jakarta Sans
    fontSize: 12px
    fontWeight: '400'
    lineHeight: 16px
  label-lg:
    fontFamily: Plus Jakarta Sans
    fontSize: 14px
    fontWeight: '700'
    lineHeight: 18px
    letterSpacing: 0.01em
  label-md:
    fontFamily: Plus Jakarta Sans
    fontSize: 12px
    fontWeight: '700'
    lineHeight: 16px
    letterSpacing: 0.02em
  label-sm:
    fontFamily: Plus Jakarta Sans
    fontSize: 10px
    fontWeight: '800'
    lineHeight: 12px
    letterSpacing: 0.04em
  numeric-price:
    fontFamily: Plus Jakarta Sans
    fontSize: 15px
    fontWeight: '800'
    lineHeight: 18px
    letterSpacing: -0.02em
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  gutter: 1rem
  gutter-sm: 0.5rem
  gutter-lg: 1.5rem
  margin: 1rem
  margin-md: 1.5rem
  margin-lg: 2.5rem
  space-xs: 0.25rem
  space-sm: 0.5rem
  space-md: 1rem
  space-lg: 1.5rem
  space-xl: 2rem
---

## Brand & Style

This design system powers a high-velocity quick-commerce grocery experience built for urgency, precision, and instant gratification. The emotional baseline balances extreme speed (sub-10 minute deliveries) with domestic dependability and calm reassurance. 

The aesthetic is **Tactile Modern Utility**:
- Crisp, physical-feeling interface modules that emphasize touchability, clarity, and rapid scanning.
- High-contrast visual cues that communicate micro-moments: rapid dispatch, dynamic routing, stock urgency, and doorstep proximity.
- Utilitarian density balanced with generous tap zones and micro-elevations, steering clear of visual clutter while accommodating dense product assortments.
- Stress-reducing feedback mechanisms that replace panicky alert states with composed, proactive operational messaging.

## Colors

The palette establishes an immediate sensation of freshness, vitality, and logistical precision.

### Color Roles & Semantics
- **Primary (`#0C831F`)**: Core brand tone representing garden-fresh produce, operational green-lights, active progress trackers, and primary purchase triggers. Secondary green token `#10A328` provides hover states and bright dynamic micro-badges.
- **Secondary (`#0F172A` / `#1E293B`)**: Grounded deep slate and midnight slate provide heavy anchor contrast for critical typography, primary headers, dark utility toolbars, and high-emphasis labels.
- **Tertiary Accent (`#F8CB46` / `#FFD644`)**: High-visibility sunlit yellow reserved for surge indicators, flash savings, peak-demand banners, and dynamic ETA tags. It injects kinetic optimism without inducing anxiety.
- **Proactive State Palette (Calm Warning)**:
  - Background: `#FFFBEB`
  - Border: `#FCD34D`
  - Text & Accents: `#92400E`
  - Used for delay advisories, monsoon traffic alerts, and high-demand buffers, completely replacing alarming reds with trustworthy, grounded transparency.
- **Canvas & Neutrals**:
  - App Canvas: `#F4F6F8` (subtle warm cool-gray that reduces glare and lifts white cards).
  - Surface Card: `#FFFFFF`.
  - Neutral Borders: `#E2E8F0`.
  - Secondary Text: `#64748B`.

## Typography

Plus Jakarta Sans delivers geometric precision with humane, approachable terminals. This structural balance maintains legibility in dense product listing matrices, compact horizontal carousels, and high-speed delivery tickers.

### Typesetting Rules
- **Numerical Hierarchy**: Prices, countdown timers, and ETA badges use weights `700` and `800` with tabular figures enabled to prevent layout jitter during live tracking updates.
- **Optical Density**: Micro badges (`label-sm`) require uppercase styling with `0.04em` letter spacing to preserve crisp rendering on sub-pixel screens.
- **Discount & Strikethrough Pricing**: Always pair `numeric-price` (700/800 weight) with an adjacent `body-sm` strikethrough in `#94A3B8` (400 weight), anchoring customer price perception immediately.

## Layout & Spacing

The system runs on a strict **4px/8px incremental grid**, maximizing inventory density on mobile viewports while preserving quick-scanning scanpaths.

### Grid & Breakpoints
- **Mobile (< 640px)**: 4-column fluid layout with `0.5rem` gutters and `1rem` outer margins. Product feeds run in a 2-column card split or edge-to-edge peek carousels.
- **Tablet (640px - 1024px)**: 8-column layout with `1rem` gutters and `1.5rem` margins. Standard catalog grid displays 3-4 items per row.
- **Desktop (> 1024px)**: 12-column fixed grid with a max-width of `1280px`, `1.5rem` gutters, and auto-centered canvas margins. Layout splits into category rails, active central feed, and pinned floating order/cart drawers.

### Tap Boundaries & Safe Areas
- Touch targets for core cart triggers, stepper buttons, and navigation elements adhere to a strict minimum interactive dimension of 44x44px, despite compact visual footprints.
- Sticky checkout drawers and floating live ETA headers offset mobile OS home indicators with an added `1.25rem` safe-area bottom/top margin buffer.

## Elevation & Depth

Visual hierarchy uses **tonal layering combined with ultra-diffused atmospheric shadows**. Rather than relying on dark borders or harsh drop shadows, elements sit elevated above the `#F4F6F8` canvas using stark white `#FFFFFF` surfaces paired with tinted ambient occlusion.

### Elevation Levels
- **Level 0 (Flat / Canvas)**: `#F4F6F8`. Used exclusively for base page canvas and nested well containers.
- **Level 1 (Card & Shelf Default)**: Pure `#FFFFFF` surface accompanied by a 1px perimeter border in `#E2E8F0` and an ambient shadow: `0 1px 3px 0 rgba(15, 23, 42, 0.04), 0 1px 2px -1px rgba(15, 23, 42, 0.02)`. Used for category tiles, standard product cards, and slot rows.
- **Level 2 (Interactive Flyouts & Floating Widgets)**: `#FFFFFF` with shadow: `0 10px 15px -3px rgba(15, 23, 42, 0.06), 0 4px 6px -4px rgba(15, 23, 42, 0.03)`. Applied to active quantity steppers, ETA pills, address switchers, and map overlays.
- **Level 3 (Modal Sheets & Pinned Drawers)**: Heavy backdrop blur (`backdrop-filter: blur(12px)`) with shadow: `0 20px 25px -5px rgba(15, 23, 42, 0.1), 0 8px 10px -6px rgba(15, 23, 42, 0.04)`. Applied to cart bars, order tracking drawers, and bottom checkout sheets.

## Shapes

The interface embraces a **modern rounded visual posture** (Tier 2: 0.5rem base radius). This produces soft, human geometry that prevents dense lists from feeling sharp or technical.

### Geometry Assignments
- **Micro Badges, Dynamic ETA Pills, and Tags**: Fully rounded pill shapes (`9999px`) to immediately denote contextual status and fleeting states.
- **Product Cards, Feed Banners, and Modular Containers**: `rounded-lg` (`1rem` / 16px) for an ergonomic, card-based interface.
- **Buttons and Form Inputs**: `0.75rem` (12px) to match finger pads and promote physical tap engagement.
- **Modal Sheets and Sliding Cart Panels**: `1.5rem` (24px) on top leading radii, providing a modern bottom-sheet silhouette on handheld viewports.

## Components

### Buttons & Steppers
- **Primary CTA**: `#0C831F` background, `#FFFFFF` text, `0.75rem` border radius, bold typography. Active state scales subtly (`0.98`) with a slight brightness boost (`#10A328`).
- **Product Card "ADD" Button**: White surface with a crisp 1px border (`#0C831F`), bold green label, and a `+` indicator. Transitions smoothly upon click into the **Quantity Stepper**.
- **Quantity Stepper**: Solid `#0C831F` pill or rounded container containing `-`, count, and `+`. Icon buttons have tactile feedback, white glyphs, and high-contrast typography.

### Dynamic ETA Pills & Peak-Demand Badges
- **ETA Delivery Pill**: High-contrast pill featuring a dark slate background (`#0F172A`) or primary green, displaying a live flash icon and bold duration text (e.g., `⚡ 8 MINS`). 
- **Peak Surge Badge**: Warm yellow tone (`#F8CB46`) with deep slate text (`#0F172A`). Emphasizes live store volume or high driver demand without alarming users.

### Proactive Delay Cards
- Grounded, anxiety-free delay component. Rendered with an amber-tinted background (`#FFFBEB`), warm gold border (`#FCD34D`), and deep brown-amber text (`#92400E`). Provides transparent operational updates (e.g., "Heavy rain in your sector — order delayed by 6 mins") with zero alarming red elements.

### Product Card Architecture
- Built on a pure white `#FFFFFF` surface with an image container featuring a neutral soft-gray well (`#F8FAFC`).
- Includes a top-left pill for discount savings (`#2563EB` or `#0C831F`), weight/volume metadata (`body-sm` in slate gray), clear bold price, crossed-out MRP, and absolute bottom-right placement of the Add/Stepper CTA.

### Multi-Step Order Timeline & Interactive Map
- **Timeline**: Connected vertical or horizontal nodes. Completed steps utilize filled `#0C831F` circles with checkmarks; active steps pulse with a dynamic green ring halo; pending steps use subtle `#CBD5E1` outlines.
- **Map Container**: Rounded 16px frame with interactive gestures, ambient edge vignette, floating rider location token, and an overlaid top-sheet housing the live ETA countdown and rider communication triggers.

### Scheduled Slot Selectors & Chips
- Horizontal scrolling chip rails and segmented date cards. Unselected slots feature `#FFFFFF` surfaces with `#E2E8F0` borders. Selected slots display a solid green border (`#0C831F`), light green background tint (`rgba(12, 131, 31, 0.08)`), and bold primary text.

### Rating & Feedback Widgets
- Post-delivery micro-modal featuring 5 rounded star or emoji tokens with amber highlight fills (`#F59E0B`), quick multi-select issue/compliment pills (e.g., "Super Fast", "Fresh Produce"), and an expandable single-line input field.