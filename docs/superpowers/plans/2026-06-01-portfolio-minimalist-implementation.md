# Portfolio Minimalist Redesign Implementation Plan

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:subagent-driven-development (recommended) or superpowers:executing-plans to implement this plan task-by-task. Steps use checkbox (`- [ ]`) syntax for tracking.

**Goal:** Redesign the current technical "blueprint" portfolio to a "Polished Minimalist" aesthetic, elevating sophistication while preserving all original project content and information.

**Architecture:** Update CSS variables, remove layout-limiting borders, introduce elegant typography, and adopt a cleaner, spacious sectioning strategy.

**Tech Stack:** HTML5, Vanilla CSS3 (relying on CSS variables and modern layout techniques).

---

### Task 1: Setup Style Variables

**Files:**
- Modify: `style.css`

- [ ] **Step 1: Define new typography and palette variables**

Update `:root` in `style.css`:
```css
:root {
    --bg-color: #0a0a0a;
    --text-primary: #f0f0f0;
    --text-secondary: #a0a0a0;
    --accent-blue: #2f81f7;
    --font-heading: 'Playfair Display', serif;
    --font-body: 'Inter', sans-serif;
}
```

- [ ] **Step 2: Add Font Imports**

Update `index.html` head section:
```html
<link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@700&family=Inter:wght@400;500&display=swap" rel="stylesheet">
```

- [ ] **Step 3: Commit**

```bash
git add style.css index.html
git commit -m "style: define typography and color variables"
```

### Task 2: Refactor CSS Layout

**Files:**
- Modify: `style.css`

- [ ] **Step 1: Remove border-based blueprint aesthetics**

Remove `.blueprint-container` side borders and update container spacing.
Modify `style.css`:
```css
.blueprint-container {
    max-width: 900px; /* Slimmer for readability */
    margin: 0 auto;
    padding: 0 2rem;
    min-height: 100vh;
}
.section-border {
    border-bottom: none; /* Remove section borders */
    padding: 6rem 0; /* Increase vertical spacing */
}
```

- [ ] **Step 2: Commit**

```bash
git add style.css
git commit -m "style: remove blueprint borders and adjust spacing"
```

### Task 3: Apply New Typography

**Files:**
- Modify: `style.css`

- [ ] **Step 1: Apply typography to body and headings**

```css
body {
    background-color: var(--bg-color);
    color: var(--text-primary);
    font-family: var(--font-body);
    line-height: 1.8;
}
.title, .section-title {
    font-family: var(--font-heading);
}
```

- [ ] **Step 2: Commit**

```bash
git add style.css
git commit -m "style: apply new typography"
```

### Task 4: Card Styling

**Files:**
- Modify: `style.css`

- [ ] **Step 1: Style Project Cards**

```css
.project-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
    gap: 2rem; /* Replace grid border with gap */
    border: none;
}
.project-card {
    padding: 2rem;
    border: none;
    transition: opacity 0.3s ease;
}
.project-card:hover {
    opacity: 0.7;
}
```

- [ ] **Step 2: Commit**

```bash
git add style.css
git commit -m "style: update project card styling"
```

### Task 5: Verify & Push

- [ ] **Step 1: Verify in Browser**
Run: `start index.html`
- [ ] **Step 2: Commit & Push**
```bash
git push origin main
```
