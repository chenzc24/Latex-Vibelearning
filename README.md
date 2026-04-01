# LaTeX Complete Reference

## Learning in the Era of Vibecoding

### The Problem: Watching Without Understanding

Something strange is happening. A student needs a LaTeX table. They type a prompt. The AI generates a perfect `booktabs` table with `\midrule` and `\bottomrule` in two seconds. The student copies it, compiles it, it works. They move on.

But ask that student a week later: *"What does `\bottomrule` do? Why `\toprule` instead of `\hline`? How would you add a multi-row cell?"* — and they have no idea. They never learned LaTeX. They learned how to ask an AI for LaTeX. That's a fundamentally different skill, and it's one that leaves you helpless the moment the AI gives you something slightly wrong, or the moment you need something it hasn't seen before.

This is the vibecoding trap. **You describe the vibe; the machine fills in the details.** It works brilliantly — until it doesn't. The code runs, the document compiles, the website deploys. Everything looks fine. But the person who "wrote" it can't explain a single line. They're a passenger, not a driver.

This isn't a rant against AI. AI is the most powerful learning tool that has ever existed. The problem is how most people use it — as a replacement for learning, rather than an accelerator for it.

### The Opportunity: Tokens as a Knowledge Printer

Here's the insight that changes everything: **AI tokens can generate any learning material you want, tailored exactly to you.**

Think about what a traditional learner does. They search for a textbook — but textbooks are written for everyone, so they're either too basic or too advanced. They watch a tutorial — but the instructor moves too fast on the interesting parts and too slow on the easy ones. They read documentation — but docs are references, not teachers. Every resource is a compromise.

Now consider what you can do with AI:

- You say: *"I know basic Python but I've never touched decorators. Generate a project that teaches me decorators from scratch, with examples I can actually run, progressing from simple to advanced."*
- You get: A personalized, runnable learning project that starts exactly where you are and goes exactly where you need.

That's not a textbook. That's not a video. That's **a knowledge base that only exists because you asked for it, organized the way your brain works, at your exact level.** No textbook author can do this for you, because no textbook author knows you.

### Who Is This Method For?

This approach — generate a personalized reference, then learn by practicing with it — works for **any domain where understanding comes through hands-on interaction with structured material.** That covers a remarkably wide range:

**Programming languages and frameworks.** You don't learn Python by reading about Python. You learn by writing Python, seeing it break, figuring out why, and fixing it. An AI-generated project that covers every core language feature with runnable examples is better than any "Learn Python in 24 Hours" book, because you chose the scope and you can modify it on the spot.

**Markup and typesetting systems.** LaTeX, HTML/CSS, Markdown, BibTeX — these are languages where the feedback loop is visual. You write code, you compile/render, you see the result. An AI-generated reference that shows the source and the output side by side, organized by topic, lets you build a mental map of the entire system. That's exactly what this repository does for LaTeX.

**Configuration and tooling.** Git, Docker, Makefile, Vim, shell scripting — these have steep learning curves not because they're hard, but because the documentation is scattered and assumes context you don't have. A generated project that walks through each command with real examples, in an order that makes sense to *you*, cuts through that noise.

**Mathematical notation and formal systems.** If you're learning linear algebra, why not ask an AI to generate a document that defines every concept with notation, a plain-language explanation, a worked example, and a practice problem? You can't get that from any single textbook chapter.

**Data formats and APIs.** JSON Schema, OpenAPI, SQL queries, regular expressions — domains where the syntax is the knowledge. An AI can generate a comprehensive example file covering every construct, and you learn by modifying it and observing the results.

**The common thread:** In all these domains, **reading about a concept is not the same as using it.** You need to touch the material, change it, break it, and fix it. The AI-generated knowledge base gives you the material. The practice gives you the understanding.

### Why This Method Works

**1. The generation phase forces you to think about scope.**

When you prompt an AI to create a learning project, you have to decide: What do I want to learn? What do I already know? How deep should it go? Answering these questions is itself a learning act. You're building a mental outline of the domain before you've studied a single line. Most learners skip this step entirely — they just start reading whatever Google gives them.

**2. The output is a map, not just content.**

A well-generated reference project doesn't just teach you individual concepts. It shows you how they relate to each other. Chapter 2 builds on Chapter 1. Chapter 7 references techniques from Chapter 4. You start to see the architecture of the domain — the big picture that's invisible when you're learning one Stack Overflow answer at a time. This is what separates someone who "knows some LaTeX commands" from someone who actually understands LaTeX.

**3. Practice is non-negotiable — but now it has a playground.**

No amount of reading replaces doing. But doing without structure is just flailing. The generated project gives you a safe, structured playground. Every example compiles. Every concept is demonstrated. You can change one parameter, recompile, and see exactly what changed. This tight feedback loop — edit, compile, observe — is where understanding solidifies. The AI can't do this part for you. That's the point.

**4. You own the result.**

When you read a textbook, the knowledge feels external — something the author has and you're borrowing. When you modify a generated project, break it, and fix it yourself, the knowledge becomes internal. You're not memorizing; you're building intuition. A week later, you won't remember the exact syntax for `\multicolumn`, but you'll remember *that it exists, what it does, and where to look it up*. That's real understanding.

### The Workflow

```
                        ┌──────────────────────┐
                        │  What do I want to    │
                        │  learn? How deep?     │
                        └──────────┬───────────┘
                                   │
                                   ▼
                        ┌──────────────────────┐
                        │  Prompt AI to generate│
                        │  a personalized       │
                        │  reference project    │
                        └──────────┬───────────┘
                                   │
                                   ▼
                        ┌──────────────────────┐
                        │  Read through the     │
                        │  generated material   │
                        │  (build the map)      │
                        └──────────┬───────────┘
                                   │
                                   ▼
                        ┌──────────────────────┐
                        │  Modify, break, fix   │
                        │  (hands-on practice)  │
                        └──────────┬───────────┘
                                   │
                                   ▼
                        ┌──────────────────────┐
                        │  The knowledge is     │
                        │  yours — not borrowed │
                        │  from a prompt        │
                        └──────────────────────┘
```

This repository is a working example of that workflow applied to LaTeX. The project owner described the scope ("cover every major LaTeX feature, organized by topic, with working examples"), the AI generated it, and then the real learning happens when you open the `.tex` files, change things, recompile, and see what happens.

**Vibecoding is the best thing that ever happened to learning — if you use it to generate the textbook *you* wish existed, and then actually read it.**

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
Latex-Vibelearning/
  main.tex                # Main document -- preamble, package config, chapter includes
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

1. **Read the PDF** -- each chapter is self-contained with explanations, code examples, and rendered output side by side
2. **Modify and experiment** -- edit any `.tex` file, recompile, and see what changes
3. **Use as a template** -- copy relevant snippets into your own documents
4. **Use as a cheatsheet** -- the appendix contains a quick reference card and document skeleton

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
| **Generated by** | Claude (Anthropic) -- GLM-5.1 |
| **Date** | 2026-04-01 |
| **Author** | User (project owner) -- conceptualized and directed the project scope and structure |
| **AI role** | Full content generation, layout design, compilation debugging, and review |
| **Compile status** | Clean build -- 0 errors, 82 pages |
