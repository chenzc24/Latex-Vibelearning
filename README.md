# LaTeX Complete Reference

## A Note on Learning in the Era of Vibecoding

We live in a time where typing a prompt can produce hundreds of lines of working code in seconds. Some call it "vibecoding" — you describe the vibe, the machine fills in the details. It's fast, it's powerful, and it's changing how everyone interacts with technology.

But here's the thing most people miss: **tokens are not knowledge.**

Getting AI to generate code for you is not the same as understanding what that code does. When you vibecode without understanding, you can ship fast — but you can't debug, can't adapt, and can't grow. The code is yours in name only. The moment something breaks, or the prompt needs to change in a way the AI didn't anticipate, you're stuck.

**The real power move is different: use your tokens to build a knowledge base tailored to *you*, then learn from it by practice.**

Think about it. A textbook is written for everyone. A tutorial video is made for thousands. But when you ask an AI to generate a learning project around exactly the things you're curious about, organized the way your brain works, with examples at your level — that's something no textbook can give you. You're not consuming content. You're *co-creating* a personal reference that you actually understand, because you chose what went into it.

This repository is exactly that idea in practice:

1. **Generate** — Use AI tokens to create a personalized, comprehensive reference project covering the topics you want to learn.
2. **Read** — Go through the generated material. It's written in your language, at your level, with working examples you can compile.
3. **Modify** — Change things. Break things. Fix things. Compile and see what happens. This is where real learning happens.
4. **Own** — By the time you've experimented with every chapter, the knowledge is yours. Not borrowed from a prompt — actually yours.

The workflow is simple:

```
Tokens  -->  Personal Knowledge Base  -->  Hands-on Practice  -->  Real Understanding
```

 vibecoding is a tool, not a substitute for learning. Use it to generate the textbook *you* wish existed. Then open it, edit it, break it, and rebuild it. That's how you turn tokens into skills.

---



## What's Inside

An **82-page PDF** (`main.pdf`) organized into 15 chapters + appendix, with working examples for every concept.

| Chapter | Topic | What You'll Learn |
|---------|-------|-------------------|
| 1 | Document Structure | `\documentclass` options, sectioning hierarchy, `\input` vs `\include`, special characters |
| 2 | Text Formatting | Bold/italic/monospace, font sizes, alignment, colors, accents, dashes, quotes |
| 3 | Lists | `itemize`, `enumerate`, `description`, custom bullets & numbering with `enumitem` |
| 4 | Tables | `tabular`, `booktabs`, `multirow`, `tabularx`, `longtable`, colored rows |
| 5 | Mathematics | Inline/display math, fractions, Greek letters, matrices, `align`, theorems, proofs |
| 6 | Figures & Images | `\includegraphics`, subfigures, image sizing, text-wrapped figures |
| 7 | Cross-References | `\label`/`\ref`, `hyperref`, clickable links, table of contents |
| 8 | Bibliography | `thebibliography`, BibTeX `.bib` files, `biblatex`, citation styles |
| 9 | Code Listings | `verbatim`, `listings` package with Python/Java/C++ examples |
| 10 | TikZ Graphics | Shapes, nodes, flowcharts, `pgfplots` charts, styles |
| 11 | Page Layout | `geometry`, `fancyhdr` headers/footers, multi-column, page breaks |
| 12 | Floats & Captions | Placement specifiers (`h,t,b,p,H`), caption styling, float barriers |
| 13 | Packages | 40+ essential packages reference, `siunitx` units, loading order |
| 14 | Custom Commands | `\newcommand`, `\newenvironment`, lengths, counters, boxes |
| 15 | Advanced Topics | Index, glossary, Beamer presentations, multilingual support, error handling |
| Appendix | Quick Reference | Complete document skeleton, symbol cheat sheet, compilation workflows |

## Project Structure

```
LatexCompleteReference/
  main.tex                # Main document — preamble, package config, chapter includes
  main.pdf                # Compiled output (82 pages)
  README.md               # This file
  chapters/
    01_document_structure.tex
    02_text_formatting.tex
    03_lists.tex
    04_tables.tex
    05_mathematics.tex
    06_figures.tex
    07_references.tex
    08_bibliography.tex
    09_code.tex
    10_tikz.tex
    11_layout.tex
    12_floats.tex
    13_packages.tex
    14_custom_commands.tex
    15_advanced.tex
    appendix.tex
```

## How to Compile

```bash
# Option 1: Manual (two passes for cross-references)
pdflatex main.tex
pdflatex main.tex

# Option 2: Automated with latexmk
latexmk -pdf main.tex

# Clean auxiliary files
latexmk -c
```

> **Note:** This project uses `pdflatex`. It also works with `xelatex` or `lualatex` if you need system font support.

## Requirements

- A LaTeX distribution: [MiKTeX](https://miktex.org/) (Windows), [TeX Live](https://www.tug.org/texlive/) (Linux/Mac), or [TinyTeX](https://yihui.org/tinytex/)
- All packages used are standard and included in a full TeX distribution
- For online editing: upload the project to [Overleaf](https://www.overleaf.com/)

## How to Use This Project

1. **Read the PDF** — each chapter is self-contained with explanations, code examples, and rendered output side by side
2. **Modify and experiment** — edit any `.tex` file, recompile, and see what changes
3. **Use as a template** — copy relevant snippets into your own documents
4. **Use as a cheatsheet** — the appendix contains a quick reference card and document skeleton

## Key Concepts Covered

- **Document classes**: `article`, `report`, `book`, `beamer`, KOMA-Script
- **Math**: from `$E=mc^2$` to matrices, multi-line equations, and theorem proofs
- **Tables**: from basic `tabular` to professional `booktabs` with multi-page support
- **Graphics**: including images, TikZ drawings, pgfplots charts
- **References**: cross-references, hyperlinks, bibliography with BibTeX/biblatex
- **Customization**: defining your own commands, environments, and styles
- **Best practices**: package loading order, float placement, error diagnosis

---

## Generation Information

| Field | Detail |
|-------|--------|
| **Generated by** | Claude (Anthropic) — GLM-5.1 |
| **Date** | 2026-04-01 |
| **Author** | User (project owner) — conceptualized and directed the project scope and structure |
| **AI role** | Full content generation, layout design, compilation debugging, and review |
| **Compile status** | Clean build — 0 errors, 82 pages |
