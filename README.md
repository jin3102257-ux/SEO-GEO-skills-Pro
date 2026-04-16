# SEO Pro Skill + GEO Pro Skill

> Stop writing flat prompts. Start shipping content systems.

This repository contains two autonomous content-engineering skills for product-led growth:

- `seopro-skill`: turns product inputs into publish-ready SEO articles
- `geopro-skill`: turns product inputs into AI-search-ready GEO answer assets

They are not prompt templates. They are structured agent workflows with intake, memory, strategy, drafting, optimization, anti-hallucination rules, humanization, and final QA.

Start with one sentence. The skill asks for the rest.

```text
use seopro-skill
```

```text
use geopro-skill
```

## Why This Exists

Most AI content workflows are fragile.

They depend on one giant prompt, vague instructions, and a lucky generation. That may work once, but it does not scale across products, keywords, search intents, or AI answer engines.

These skills are built for repeatable content production:

- zero-friction activation
- proactive intake
- strict single-path execution
- layered strategy before drafting
- local memory to reduce repetition
- hallucination control
- safer link and evidence policies
- final QA before output

The goal is not just to generate text. The goal is to create reusable content assets.

## Two Skills, Two Search Worlds

| Skill | Search World | Primary Output | Built For |
|---|---|---|---|
| `seopro-skill` | Traditional search | SEO article | Product keywords, search intent, internal links, readable long-form content |
| `geopro-skill` | AI answer engines | GEO answer asset | Entity clarity, answer-first blocks, extractable tables, authority notes, citation-ready summaries |

Use `seopro-skill` when you want a strong product-led SEO article.

Use `geopro-skill` when you want content that is easier for ChatGPT-like systems, Perplexity-style answer engines, and AI search surfaces to understand, extract, summarize, and cite.

## SEO Pro Skill

`seopro-skill` is an autonomous SEO article pipeline.

It takes a product name, product URL, target keyword, audience, and conversion goal, then runs a strict layered workflow from product intelligence to final QA.

### Highlights

- **Proactive Intake**: users do not need to prepare a perfect brief up front
- **8-Layer Pipeline**: normalization, product intelligence, keyword strategy, structure, draft, authority optimization, humanization, QA
- **Memory-Aware Execution**: stores concise continuity notes in local `memory.md` after successful runs
- **No Hallucinated Links**: never invents internal URLs or unsupported proof points
- **Anti-AI-Sludge Rewrite**: removes generic AI filler and sharpens the article into human-readable expert prose
- **Publish-Ready Output**: produces a complete article instead of exposing messy intermediate artifacts

### Start It

```text
use seopro-skill
```

The skill will ask for missing required inputs, then continue automatically.

## GEO Pro Skill

`geopro-skill` is an autonomous GEO asset pipeline for generative answer engines.

It is designed around a different assumption: the primary reader is the model layer. Human readers still matter, but the content must first be easy for AI systems to parse, extract, recompose, and cite.

### Highlights

- **Answer-First Structure**: opens with the direct answer instead of burying it under blog-style setup
- **Entity Clarity**: keeps the product identity stable and binds claims directly to the entity
- **Tables By Default**: uses structured tables for key facts, comparisons, confidence separation, and limitations
- **Confirmed vs Inferred Claims**: separates verified information from reasonable assumptions
- **Authority Notes**: prefers official docs, platform guidance, research, and credible third-party sources when trust depends on them
- **Citation-Ready Blocks**: creates short, self-contained sections that survive partial extraction
- **No SEO-Blog Padding**: avoids forcing FAQ, conclusion, or CTA sections unless the topic truly needs them

### Start It

```text
use geopro-skill
```

Minimum inputs:

- product name
- product URL
- target topic, question, or keyword cluster

Example:

```text
Product name: ShortAPI
Product URL: https://shortapi.ai
Target topic/question: free ai api
```

## Quick Installation

Copy either skill folder into your local skills directory.

Example:

```text
skills/
  seopro-skill/
    SKILL.md
    agents/
      openai.yaml
  geopro-skill/
    SKILL.md
    agents/
      openai.yaml
```

After your skill system recognizes the folder, invoke the skill by its frontmatter name:

```text
use seopro-skill
```

```text
use geopro-skill
```

## What Makes These Skills Different

### Not A Prompt Template

The skills do not simply ask a model to "write an article." They define layered execution rules, intermediate reasoning stages, memory behavior, safety constraints, and final output requirements.

### Intake Without Friction

Users can start with just the skill name. If required information is missing, the skill asks only for what it needs and then continues automatically.

### Safer By Design

Both skills include explicit rules against:

- fake statistics
- invented benchmarks
- hallucinated internal links
- unsupported comparison claims
- fake citations
- overconfident SEO or GEO guarantees

### Built For Repeated Use

Each skill can create a local `memory.md` after successful runs. Memory is intentionally concise and is used to reduce repeated topics, angles, frameworks, and content patterns.

## Important Notes

- `memory.md` is intentionally not included in this repository.
- Memory is runtime state and should be created locally after successful runs.
- These skills are model-only workflows.
- They do not guarantee search rankings, AI citations, or AI-search visibility.
- They are designed to make content more structured, useful, honest, and machine-readable.

## Repository Structure

```text
.
├── README.md
├── seopro-skill/
│   ├── SKILL.md
│   └── agents/
│       └── openai.yaml
└── geopro-skill/
    ├── SKILL.md
    └── agents/
        └── openai.yaml
```

## Suggested Repository Description

```text
Autonomous SEO and GEO content-engineering skills for product-led search and AI answer engines.
```

## Suggested Topics

```text
seo
geo
generative-engine-optimization
ai-search
content-generation
codex-skills
llm
answer-engine-optimization
```
