# LMLslides

A comprehensive Quarto extension for creating professional academic lecture slides with Reveal.js, featuring rich pedagogical elements and a polished theme.

## Installing

```bash
quarto add littlemonkeylab/LMLslides
```

This will install the extension and make it available for your presentations.

## Features

LMLslides provides a professional SCSS theme with 20+ pedagogical div classes designed specifically for academic teaching:

### Core Features
- **Title slide** with background image support
- **Clickable logo** in lower right corner (links to littlemonkeylab.com)
- **Clean layout** with no logo/slide number on title slide
- **Professional color palette** optimized for readability
- **Custom fonts** including Fira Code for programming content

### Pedagogical Elements

**Content Organization:**
- `:::objectives` - Learning objectives boxes
- `:::definition` - Definition callouts
- `:::concept` - Key concept highlights
- `:::example` - Example boxes
- `:::theorem` - Mathematical theorems
- `:::proof` - Mathematical proofs with QED symbol

**Interactive Elements:**
- `:::poll` - Poll questions for audience engagement
- `:::question` - Discussion prompts
- `:::exercise` - Practice problems
- `:::solution` - Exercise solutions
- `:::appex` - Application exercises

**Alerts and Notifications:**
- `:::warning` - Critical warnings
- `:::caution` - Important cautions
- `:::note` - Supplementary notes
- `:::tip` - Helpful tips
- `:::important` - Important highlights

**Visual Enhancements:**
- `:::takeaway` - Key takeaway summaries
- `:::callout` - Highlighted quotes
- `:::emphasize` - Emphasized content
- Two-column layouts with `:::columns`
- Image containers with captions
- Process steps with numbered circles
- Side-by-side comparisons
- Section dividers

**Lists:**
- `.checklist` - Lists with green checkmarks
- `.xlist` - Lists with red X marks

### Typography & Code

- Inline code highlighting with `.code-highlight`
- Semantic element highlighting (`.block-el`, `.inline-el`, `.meta-el`)
- Mathematical equation boxes
- Custom adage styles (`.bigadage`, `.smalladage`)
- Fira Code font for all code blocks

## Quick Start

1. Create a new `.qmd` file:

```yaml
---
title: "Your Lecture Title"
author: "Your Name"
institute: "Your Institution"
format: LMLslides-revealjs
---

# Introduction {background-color="#00817c"}

## Learning Objectives

::: objectives
- First objective
- Second objective
- Third objective
:::
```

2. Render your slides:

```bash
quarto render your-lecture.qmd
```

## Examples

- **[template.qmd](template.qmd)** - Basic example with common features
- **[comprehensive-template.qmd](comprehensive-template.qmd)** - Complete showcase of all features
- **[FEATURES.md](FEATURES.md)** - Detailed documentation of all available features

## Documentation

See [FEATURES.md](FEATURES.md) for comprehensive documentation including:
- Complete list of all div classes
- Usage examples for each feature
- Color palette reference
- Best practices for academic presentations
- Quick reference guide

## Configuration

The extension includes sensible defaults:

- **Dimensions:** 1600x900px (16:9 aspect ratio)
- **Transition:** Fade
- **Slide Numbers:** Centered
- **Code Overflow:** Wrap
- **Syntax Highlighting:** GitHub style
- **Progress Bar:** Enabled
- **Menu:** Enabled (press 'M' to open)

## Color Palette

- **Blue** (#00817c) - Primary, objectives, takeaways
- **Purple** (#73245e) - Definitions, theorems
- **Green** (#02733e) - Examples, solutions
- **Red** (#bf2642) - Warnings, important items
- **Orange** (#f2a03d) - Polls, cautions
- **Teal** (#17a2b8) - Tips
- **Yellow** (#ffc107) - Notes

## Contributing

Contributions are welcome! Please feel free to submit issues or pull requests.

## License

See LICENSE file for details.

## Credits

Created by LittleMonkeyLab (drdeception)
