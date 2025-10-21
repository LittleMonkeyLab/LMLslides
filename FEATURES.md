# LMLslides Pedagogical Features Guide

A comprehensive guide to all available pedagogical features in the LMLslides Quarto extension.

## Table of Contents

- [Getting Started](#getting-started)
- [Content Elements](#content-elements)
- [Interactive Elements](#interactive-elements)
- [Visual Enhancements](#visual-enhancements)
- [Layout Options](#layout-options)
- [Typography](#typography)
- [Mathematical Content](#mathematical-content)

## Getting Started

### Basic Slide Format

```yaml
---
title: "Your Lecture Title"
subtitle: "Optional Subtitle"
author: "Your Name"
institute: "Your Institution"
date: "2024"
format: LMLslides-revealjs
---
```

### Creating Sections

Use level 1 headers with background colors for section dividers:

```markdown
# Section Title {background-color="#00817c"}
```

## Content Elements

### Learning Objectives

Display clear learning goals at the start of your lecture:

```markdown
::: objectives
- First learning objective
- Second learning objective
- Third learning objective
:::
```

**Visual:** Blue box with "Learning Objectives" header

---

### Definitions

Highlight important definitions:

```markdown
::: definition
**Term**: Explanation of the term goes here.
:::
```

**Visual:** Purple left border with "Definition" header

---

### Key Concepts

Emphasize critical concepts:

```markdown
::: concept
Your key concept explanation here.
:::
```

**Visual:** Indigo left border with "Key Concept" header

---

### Examples

Provide clear examples:

```markdown
::: example
**Example Title**

Your example content with steps or explanation.
:::
```

**Visual:** Green left border with "Example" header

---

### Notes

Add supplementary information:

```markdown
::: note
Important note for students to remember.
:::
```

**Visual:** Yellow left border with 📝 Note icon

---

### Tips

Provide helpful tips:

```markdown
::: tip
Helpful tip for students.
:::
```

**Visual:** Teal left border with 💡 Tip icon

---

### Warnings

Alert students to common pitfalls:

```markdown
::: warning
Critical warning about potential errors or mistakes.
:::
```

**Visual:** Red left border with ⚠ Warning icon

---

### Cautions

Highlight areas requiring special attention:

```markdown
::: caution
Something to be careful about.
:::
```

**Visual:** Orange left border with ⚡ Caution icon

## Interactive Elements

### Poll Questions

Create interactive poll questions:

```markdown
::: poll
What is the correct answer?

A. Option one
B. Option two
C. Option three
D. Option four
:::
```

**Visual:** Orange bordered box with beige background

---

### Questions

Pose discussion questions:

```markdown
::: question
How would you approach this problem?
:::
```

**Visual:** Blue-gray box

---

### Exercises

Assign practice problems:

```markdown
::: exercise
Write a function that does X.

**Constraints**: List any constraints
:::
```

**Visual:** Dark blue border with 📝 Exercise icon

---

### Solutions

Provide solutions (can be combined with fragments):

```markdown
::: solution
Your solution code or explanation here.
:::
```

**Visual:** Green left border with "Solution:" prefix

---

### Application Exercises

Real-world application problems:

```markdown
::: appex
**Context**

Your application exercise description and requirements.
:::
```

**Visual:** Light blue box with dark blue border

## Visual Enhancements

### Important Highlights

Draw attention to critical information:

```markdown
::: important
This is extremely important!
:::
```

**Visual:** Red bordered box, centered, bold text

---

### Emphasis Boxes

Emphasize specific content:

```markdown
::: emphasize
This content deserves special attention.
:::
```

**Visual:** Light orange background with orange left border

---

### Callouts

Create centered, stylized quotes or callouts:

```markdown
::: callout
"An impactful quote or key statement."
:::
```

**Visual:** Centered, italic text with top/bottom blue borders

---

### Takeaways

Summarize key points:

```markdown
::: takeaway
Main points students should remember from this section.
:::
```

**Visual:** Double blue border with 🎯 Key Takeaway header and gradient background

---

### Comparisons

Side-by-side pros and cons:

```markdown
::: comparison
::: {.compare-item .pro}
### Advantages
- Point one
- Point two
:::

::: {.compare-item .con}
### Disadvantages
- Point one
- Point two
:::
:::
```

**Visual:** Two-column grid with green (pro) and red (con) styling

---

### Inverse Boxes

Inline highlighted terms:

```markdown
[key term]{.inversebox}
```

**Visual:** Blue background with white text

## Layout Options

### Two-Column Layout

Create side-by-side content:

```markdown
::: columns
::: column
Left column content
:::

::: column
Right column content
:::
:::
```

**Options:**
- `.align-center` - Vertically center columns
- `.align-bottom` - Align columns to bottom

---

### Vertical Centering

Center content vertically on slide:

```markdown
::: v-center-container
Your centered content
:::
```

**Use case:** Title slides, single important points

---

### Image with Caption

Professional image presentation:

```markdown
::: img-container
![](image.png)

::: caption
Figure 1: Description of the image
:::
:::
```

**Visual:** Centered image with border and italic caption

---

### Section Dividers

Visual separation between topics:

```markdown
::: section-divider
Part II: Advanced Topics
:::
```

**Visual:** Centered text with decorative lines on either side

## Typography

### Inline Code Highlighting

Highlight code terms inline:

```markdown
[variable_name]{.code-highlight}
```

**Visual:** Light yellow background with monospace font

---

### Element Types

Semantic highlighting for HTML/programming elements:

```markdown
[Block elements]{.block-el}
[Inline elements]{.inline-el}
[Meta elements]{.meta-el}
```

**Visual:** Color-coded text (green, red, orange)

---

### Adages and Quotes

Large decorative text:

```markdown
::: {.bigadage}
Practice Makes Perfect
:::

::: {.smalladage}
A helpful saying
:::
```

**Visual:** Amatic SC font at 250% or 150% size

---

### Lists

#### Checklist

```markdown
::: checklist
- Completed item one
- Completed item two
:::
```

**Visual:** ✓ green checkmarks

#### X-List

```markdown
::: xlist
- Don't do this
- Avoid this mistake
:::
```

**Visual:** ✗ red X marks

## Mathematical Content

### Theorems

State mathematical theorems:

```markdown
::: theorem
Statement of the theorem with mathematical notation.
:::
```

**Visual:** Purple border, italic "Theorem" header

---

### Proofs

Mathematical proofs:

```markdown
::: proof
Your proof steps and logic.
:::
```

**Visual:** Beige background with "Proof." prefix and QED symbol (∎) at end

---

### Equation Boxes

Highlight important equations:

```markdown
::: equation-box
$$E = mc^2$$

$$\int_{a}^{b} f(x)dx = F(b) - F(a)$$
:::
```

**Visual:** Beige box with border, centered equations

## Advanced Features

### Process Steps

Create numbered step-by-step processes:

```markdown
::: {.step data-step="1"}
First step description
:::

::: {.step data-step="2"}
Second step description
:::
```

**Visual:** Blue numbered circles with step content

---

### References

Add citations and references:

```markdown
::: reference
**Sources:**
1. Author (Year). *Title*. Publisher.
2. Author (Year). *Title*. Publisher.
:::
```

**Visual:** Small gray text with top border at bottom of slide

---

### Incremental Reveals

Reveal content step-by-step:

```markdown
::: {.incremental}
- First point
- Second point
- Third point
:::
```

Or use fragments:

```markdown
. . .

Content appears on next click
```

---

### Fragment Highlighting

Highlight content as you discuss it:

```markdown
[This text]{.fragment .highlight-current-blue}
[This text]{.fragment .highlight-current-red}
```

## Color Palette

The theme uses the following colors:

- **Blue** (`#00817c`): Primary headings, objectives, takeaways
- **Purple** (`#73245e`): Definitions, theorems
- **Green** (`#02733e`): Examples, solutions, success
- **Red** (`#bf2642`): Warnings, errors, important
- **Orange** (`#f2a03d`): Polls, cautions, emphasis
- **Teal** (`#17a2b8`): Tips, info
- **Yellow** (`#ffc107`): Notes, highlights
- **Indigo** (`#6610f2`): Key concepts
- **Beige** (`#f8f5f0`): Background accents

## Tips for Effective Presentations

1. **Start with objectives** - Always begin with learning objectives
2. **Use examples liberally** - Concrete examples aid understanding
3. **Break up content** - Use different div styles to maintain engagement
4. **Include interactivity** - Polls and questions encourage participation
5. **Emphasize key points** - Use takeaways and important boxes
6. **Provide practice** - Include exercises with solutions
7. **End with summary** - Review key takeaways at the end

## Complete Example

See `comprehensive-template.qmd` for a complete example using all features.

## Quick Start Template

```markdown
---
title: "My Lecture"
format: LMLslides-revealjs
---

# Introduction {background-color="#00817c"}

## Learning Objectives

::: objectives
- Objective one
- Objective two
:::

## Key Concept

::: concept
Your key concept here
:::

::: example
**Example**
Your example here
:::

# Summary {background-color="#00817c"}

::: takeaway
Key points to remember
:::
```
