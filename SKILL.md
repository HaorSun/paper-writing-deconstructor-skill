---
name: paper-writing-deconstructor
description: Analyze academic paper full texts, sections, paragraphs, or excerpts to improve scholarly writing. Use when the user provides a paper, abstract, introduction, literature review, methods, results, discussion, conclusion, or draft passage and wants to deconstruct its structure, rhetorical function, argument role, writing moves, sentence purpose, reusable sentence patterns, paragraph templates, and transferable writing strategies without simply summarizing, translating, or copying the original text.
---

# Paper Writing Deconstructor

## Purpose

Use this skill to help the user learn academic writing by deconstructing how a paper works as a layered argument. The goal is not to summarize the paper, but to reveal how the full text, sections, paragraphs, and sentences perform scholarly functions and how those functions can be transferred into the user's own writing.

Treat papers as structured argument systems:

Full paper -> section -> paragraph -> sentence -> reusable writing pattern

## Default Interaction Workflow

Use this as the default workflow unless the user explicitly requests a different depth.

1. Full paper input
   Build a whole-paper structure map. Do not do sentence-level analysis of the full paper. Identify the research problem, central claim or purpose, overall argument chain, section functions, key argument nodes, and suggested drill-down sections.

2. Section input
   Build a section-level structure map. Identify the section's typical academic function, this paper's actual move sequence, paragraph functions, paragraph-to-paragraph transitions, and high-value paragraphs for deep analysis.

3. Paragraph input
   Perform complete deep analysis in one response. Include paragraph function, paragraph move sequence, sentence-level four-layer deconstruction, argument chain, transferable paragraph template, reusable sentence templates, and writing transfer advice. Do not require another user turn before extracting writing resources at paragraph level.

## Modes

Choose the narrowest mode that fits the user's input.

1. Full Paper Mode
   Use when the user provides a complete paper or a long near-complete text. First build a structure map of the whole paper. Do not immediately do sentence-by-sentence analysis of the entire paper. Recommend high-value sections or paragraphs for deeper analysis.

2. Section Mode
   Use when the user provides a recognizable section such as abstract, introduction, literature review, methods, results, discussion, or conclusion. Analyze the section's internal structure and writing moves, then identify paragraphs worth sentence-level deconstruction.

3. Paragraph Deep Analysis Mode
   Use when the user provides or selects a paragraph for close reading. Complete paragraph structure, sentence structure, and writing resource extraction in the same response.

4. Excerpt Mode
   Use when the user provides a few paragraphs or isolated sentences that are not clearly a single paragraph for deep analysis. First infer the likely paper location and uncertainty, then perform local deconstruction.

5. Draft Feedback Mode
   Use when the user provides their own draft. Preserve the intended meaning, diagnose the writing function of each part, and suggest revisions that strengthen scholarly purpose, logical flow, and transferable style.

## Workflow

### 1. Locate the Text

Identify the likely paper location and the writing task that location usually serves.

- Abstract: compress the whole paper into problem, method, result, contribution.
- Introduction: establish background, importance, gap, research question, contribution.
- Literature review: organize prior work, build categories, locate debates, expose limitations.
- Methods: make the study credible, reproducible, and appropriately scoped.
- Results: present evidence without overexplaining.
- Discussion: interpret findings, connect to theory, explain contribution, acknowledge limits.
- Conclusion: consolidate contribution, implications, limits, and future work.

If the location is uncertain, say so and analyze conditionally.

### 2. Build the Whole-Text or Section Map

For full papers and long sections, start with a top-down map before local analysis:

- Research problem
- Central claim or purpose
- Overall argument chain
- Major section functions
- Key transition points
- High-value passages for deeper deconstruction

Use a compact table:

| Part | Content role | Argument function | Writing strategy | Worth learning |
|---|---|---|---|---|

### 3. Deconstruct Paragraphs

For each selected paragraph, identify:

- Paragraph function
- Topic or controlling idea
- Internal move sequence
- Relationship to previous and next paragraph
- Evidence, reasoning, and limitation work
- What a writer can imitate structurally

Use this pattern:

```text
Paragraph function:
Move sequence:
Why this order works:
Transferable paragraph template:
```

### 4. Deconstruct Sentences

When doing sentence-level analysis, do not only explain meaning. For each sentence or clause group, identify four layers of function:

- Semantic function: what the sentence says.
- Structural function: how it connects, opens, turns, narrows, or closes the local text.
- Argument function: how it advances the paper's claim, evidence, gap, interpretation, or contribution.
- Rhetorical or stance function: how it controls certainty, scope, emphasis, caution, authority, or reader expectation.

Use this table:

| Text | Semantic function | Structural function | Argument function | Rhetorical/stance function | Why write it this way | Transferable pattern |
|---|---|---|---|---|---|---|

Common writing moves:

- Background framing
- Problem importance
- Concept definition
- Scope narrowing
- Prior work synthesis
- Prior work credit
- Gap opening
- Contrast or concession
- Research question setup
- Aim or contribution statement
- Method credibility
- Evidence reporting
- Result highlighting
- Interpretation
- Mechanism speculation
- Theoretical contribution
- Practical implication
- Limitation control
- Future research opening
- Paragraph closure

### 5. Reconstruct the Argument Chain

After local analysis, summarize how the text moves the argument forward. Use a chain such as:

```text
Background consensus -> unresolved gap -> research aim -> evidence -> interpretation -> contribution
```

or create a better chain that matches the text.

### 6. Extract Transferable Writing Resources

Extract resources at three levels:

1. Writing moves
   Example: "Acknowledge established research, then narrow to what remains underexplored."

2. Sentence templates
   Convert source sentences into reusable templates. Do not encourage direct copying.

3. Paragraph templates
   Convert paragraph organization into a reusable sequence.

For each template include:

```text
Function:
Template:
Best used in:
Use carefully when:
```

## Output Formats

### Full Paper Mode

```markdown
## 1. Whole-Paper Structure Map

- Research problem:
- Central claim or purpose:
- Overall argument chain:
- Main contribution:

## 2. Section Functions

| Section | Main content | Paper function | Writing strategy | Worth learning |
|---|---|---|---|---|

## 3. Key Argument Nodes

| Location | Function | Why it matters | What to learn |
|---|---|---|---|

## 4. Suggested Drill-Down Path

1. ...
2. ...
3. ...
```

### Section or Excerpt Mode

```markdown
## 1. Location and Overall Function

- Likely location:
- Overall function:
- Core writing task:

## 2. Deconstruction

| Text | Semantic function | Structural function | Argument function | Rhetorical/stance function | Why write it this way | Transferable pattern |
|---|---|---|---|---|---|---|

## 3. Argument Chain

...

## 4. Reusable Writing Resources

### Pattern 1
- Function:
- Template:
- Best used in:
- Use carefully when:

## 5. Writing Transfer Advice

...
```

### Paragraph Deep Analysis Mode

```markdown
## 1. Paragraph Function

- Likely section:
- Paragraph task:
- Central writing move:
- Function judgment basis:

## 2. Paragraph Structure

- Move sequence:
- Why this order works:
- Relationship to surrounding text:

## 3. Sentence Four-Layer Deconstruction

| Text | Semantic function | Structural function | Argument function | Rhetorical/stance function | Why write it this way | Transferable pattern |
|---|---|---|---|---|---|---|

## 4. Argument Chain

...

## 5. Transferable Paragraph Template

```text
...
```

## 6. Reusable Sentence Templates

### Template 1
- Function:
- Template:
- Best used in:
- Use carefully when:

## 7. Writing Transfer Advice

...
```

### Draft Feedback Mode

```markdown
## 1. Current Intended Function

## 2. Diagnosis

| Draft text | Intended function | Current issue | Revision direction |
|---|---|---|---|

## 3. Suggested Revision

## 4. Why the Revision Works

## 5. Reusable Pattern for Future Writing
```

## Guardrails

- Do not fabricate paper content, citations, methods, findings, or author intent.
- Do not present uncertain section location as certain.
- Do not reduce the task to summary or translation unless the user explicitly asks for that.
- Do not encourage plagiarism or direct copying of original sentences.
- Prefer templates and writing moves over verbatim extraction.
- If the user asks for "usable sentences", provide adaptable templates and explain how to customize them.
- If the input is too long for detailed analysis, first produce a structure map and ask which part to drill into next.
- If the input is too short, state the limits of inference and provide a local analysis.

## Quality Bar

A good response should leave the user with both understanding and writing leverage:

- What this text does in the paper
- How the argument progresses
- Why the author wrote it this way
- Which moves are reusable
- How the user can apply those moves in their own paper
