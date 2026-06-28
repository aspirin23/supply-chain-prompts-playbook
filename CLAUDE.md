# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What This Repository Is

A documentation-only prompting library for enterprise and industry AI adoption. There is no executable code, build system, or test infrastructure — all content is Markdown.

Target audience: industry professionals (supply chain, CPG, manufacturing, energy) learning to prompt LLMs effectively, not developers.

## Repository Structure

```
enterprise-ai-prompts/
├── README.md                    # Project overview and how-to-use guide
├── prompting-guide.md           # Core 5-component framework (start here)
└── prompt-patterns/             # Deep dives on individual techniques
    ├── 01-role-prompting.md
    ├── 02-few-shot-examples.md
    ├── 03-chain-of-thought.md
    ├── 04-structured-output.md
    └── 05-constraint-setting.md
```

Industry-specific folders (cpg-retail/, manufacturing/, energy-utilities/, general-supply-chain/) are planned but do not yet exist.

## Core Framework

Every prompt in this library is built on a five-component structure:

```
ROLE: [job title / expert persona]
CONTEXT: [business situation and background]
TASK: [action verb + what to do]
CONSTRAINTS: [what to avoid, tone, scope]
OUTPUT FORMAT: [table, bullets, paragraphs, etc.]
```

## Content Pattern for Pattern Files

Each file in `prompt-patterns/` follows the same didactic structure:

1. **What it is** — definition and core concept
2. **Why it works** — the reasoning behind the technique
3. **When to use it** — operational triggers
4. **Worked examples** — industry-specific (CPG/Retail, Manufacturing, Energy/Utilities)
5. **When this pattern fails** — failure modes and edge cases
6. **Combine with** — relationships to other patterns
7. **Quick template** — ready-to-use starter

Maintain this structure when adding new pattern files.

## Conventions

- File names in `prompt-patterns/` use numeric prefixes (`01-`, `02-`, ...) to indicate reading order.
- Tone is professional and practitioner-focused — avoid academic or developer-centric language.
- Worked examples should use realistic but generic data (no real company names, no memorable PII in examples).
- Each prompt example should include a brief "why this works" explanation alongside the prompt text.
- Industry examples should span CPG/Retail, Manufacturing, and Energy/Utilities where possible to show broad applicability.
