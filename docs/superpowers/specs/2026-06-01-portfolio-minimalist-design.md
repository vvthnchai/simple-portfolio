# Portfolio Minimalist Redesign Design Specification

## Overview
Redesign the current technical "blueprint" portfolio to a "Polished Minimalist" aesthetic. This redesign aims to elevate the portfolio's visual sophistication while preserving all original project content and information.

## Visual Changes
- **Typography:**
  - Headings: Change from `JetBrains Mono` to `Playfair Display` (Serif).
  - Body: Change from `JetBrains Mono` to `Inter` (Sans-Serif).
- **Palette & Layout:**
  - Background: Deepen to `#0a0a0a`.
  - Grid: Remove border-based blueprint aesthetic.
  - Sectioning: Replace border-based sectioning with generous whitespace ("breathing room").
  - Container: Remove side borders.
- **Components:**
  - Project Cards: Borderless containers, subtle hover effects (opacity/lift).

## Information Preservation
All existing project titles, descriptions, and contact links will be maintained exactly as currently defined in `index.html`.

## Technical Implementation Plan (Upcoming)
1. Update `style.css` with new font imports and variables.
2. Remove border-based classes and adjust padding/margins in `style.css`.
3. Update `index.html` structure if necessary to accommodate new layout logic.
