# OKR Roadmap Builder

## Purpose

Create OKR-based roadmaps from existing hypotheses and information from Lean Product Canvas and Product Strategy Canvas, translating strategic objectives into actionable quarterly plans.

## Context

Product teams need to bridge strategic vision with tactical execution. This tool transforms canvas insights and prioritized hypotheses into coherent quarterly roadmaps using Jeff Gothelf's methodology.


## Instructions

1. **Analyze input documents** containing:
   - Prioritized hypotheses from Lean Product Canvas
   - Lean Product Canvas (problems, solutions, user groups, metrics)
   - Product Strategy Canvas (vision, target market, differentiating factors)

2. **Align with strategy:**
   - Extract overarching business goal from Product Strategy Canvas
   - Identify target market and target groups
   - Understand differentiating factors and competitive advantages
   - Formulate strategy-compliant objective

3. **Understand problems:**
   - Identify main problems from Lean Product Canvas
   - Analyze customer segments and specific needs
   - Extract key metrics already defined in canvas

4. **Derive OKRs:**
   - Create inspiring objective aligned with Strategy Canvas vision
   - Develop 2-3 measurable key results following "Who does what by how much?" format
   - Ensure key results harmonize with Lean Product Canvas metrics
   - Verify existing hypotheses can support key results

5. **Map hypotheses:**
   - Assign each existing hypothesis to appropriate key result
   - Verify hypotheses follow format: "We believe that [Key Result] will be achieved if [Persona] [Experiences benefit] through [Feature/Solution]"
   - Identify gaps where additional hypotheses might be needed

6. **Create quarterly roadmap:**
   - Structure with objective as heading
   - Assign key results per quarter (logically sequenced)
   - Place hypotheses/features under respective quarters
   - Decrease detail level in later quarters (Q3/Q4)
   - Prioritize based on customer value, dependencies, and expected impact

7. **Plan discovery activities:**
   - Identify risky assumptions from Lean Product Canvas
   - Analyze knowledge and validation gaps
   - Formulate discovery questions addressing uncertainties

8. **Validate roadmap quality:**
   - Objective is inspiring and aligns with Strategy Canvas vision
   - Key results follow proper format and are supported by metrics
   - All hypotheses link to key results and address canvas problems
   - Roadmap shows logical sequencing with decreasing detail
   - Discovery questions address most critical assumptions

## Output Format

Create a markdown file at `docs/product/roadmap.md` with this structure:

```markdown
# Product Roadmap: [Product Name]

## Strategy Context
[Summary of the most relevant information from canvas documents]

## Objective
[The overarching qualitative goal]

## Roadmap by Quarter

### Q1
**Key Result 1:** [Who does what by how much?]

**Hypotheses:**
- [Existing Hypothesis 1]
- [Existing Hypothesis 2]

**Discovery Questions:**
- [Question 1]
- [Question 2]

### Q2
**Key Result 2:** [Who does what by how much?]

**Hypotheses:**
- [Existing Hypothesis 3]

**Discovery Questions:**
- [Question 3]

### Q3-Q4
**Potential Future Key Results:**
- [Preliminary ideas for future Key Results]

## Review Cycle
This roadmap will be reviewed and adjusted quarterly, based on insights from discovery work and achieved results.
```

## Success Criteria

- Objective is inspiring and future-oriented, aligned with Strategy Canvas vision
- Key results follow "Who does what by how much?" format and are supported by Lean Product Canvas metrics
- All hypotheses are clearly linked to key results and address canvas problems
- Roadmap shows logical sequencing with decreasing detail in later quarters
- Discovery questions address most critical assumptions from canvas
- Roadmap prioritizes outcomes over outputs and allows for regular adjustments

$ARGUMENTS