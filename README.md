# Paper Writing Deconstructor

[中文说明](README.zh-CN.md)

Paper Writing Deconstructor is a Codex skill for learning academic writing by deconstructing research papers as layered argument systems.

It is designed for users who want to read papers not only for content, but for writing: how a paper frames a problem, organizes sections, develops paragraphs, uses sentences rhetorically, and turns those patterns into reusable writing resources.

## Core Workflow

The skill follows this default workflow:

```text
Full paper -> section -> paragraph -> sentence -> reusable writing pattern
```

### 1. Full Paper Input

When given a full paper, the skill builds a whole-paper structure map. It does not perform sentence-level analysis of the entire paper by default.

It identifies:

- Research problem
- Central claim or purpose
- Overall argument chain
- Section functions
- Key argument nodes
- Suggested sections for deeper analysis

### 2. Section Input

When given a section such as Abstract, Introduction, Literature Review, Methods, Results, Discussion, or Conclusion, the skill analyzes the section-level structure.

It identifies:

- The section's typical academic function
- The paper's actual move sequence
- Paragraph functions
- Paragraph-to-paragraph transitions
- High-value paragraphs for close reading

### 3. Paragraph Input

When given a paragraph, the skill performs complete deep analysis in one response.

It includes:

- Paragraph function
- Paragraph move sequence
- Sentence-level four-layer deconstruction
- Argument chain
- Transferable paragraph template
- Reusable sentence templates
- Writing transfer advice

## Sentence Four-Layer Deconstruction

For sentence-level analysis, the skill uses four layers:

| Layer | Question |
|---|---|
| Semantic function | What does the sentence say? |
| Structural function | How does it connect, open, turn, narrow, or close the local text? |
| Argument function | How does it advance the paper's claim, evidence, gap, interpretation, or contribution? |
| Rhetorical/stance function | How does it control certainty, scope, emphasis, caution, authority, or reader expectation? |

## Example Prompts

```text
Use $paper-writing-deconstructor to analyze this full paper and build a whole-paper structure map.
```

```text
Use $paper-writing-deconstructor to analyze the Introduction section and identify its paragraph functions.
```

```text
Use $paper-writing-deconstructor to deeply analyze this paragraph, including paragraph structure, sentence four-layer deconstruction, and reusable writing templates.
```

## Installation

Copy this repository folder into your Codex skills directory:

```text
~/.codex/skills/paper-writing-deconstructor/
```

Required files:

```text
paper-writing-deconstructor/
├── SKILL.md
└── agents/
    └── openai.yaml
```

Restart Codex after installing or updating the skill.

## Guardrails

The skill should not:

- Fabricate paper content, citations, methods, findings, or author intent
- Reduce analysis to summary or translation unless explicitly requested
- Encourage plagiarism or direct copying of source sentences
- Present uncertain section location as certain

The skill should:

- Prefer transferable templates over copied sentences
- Explain why a writing move works
- Help users adapt writing patterns to their own papers
- Keep full-paper analysis structural and reserve sentence-level depth for selected paragraphs
