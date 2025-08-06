# Hypothesis Prioritization Canvas Builder

## Purpose

Create systematic hypothesis prioritization canvases that evaluate product hypotheses by value and risk, enabling clear decisions about which ideas to test, ship, or discard.

## Context

Product teams often struggle with too many hypotheses and limited resources. This tool helps objectively evaluate hypotheses using a 2x2 matrix (value vs. risk) to create actionable prioritization decisions based on Jeff Gothelf's Lean UX methodology.


## Instructions

1. **Analyze input documents** containing existing hypotheses from:
   - Lean Product Canvas
   - Strategic documents
   - User research results
   - Technical feasibility assessments
   - Market and competitive analysis

2. **Capture project details:**
   - Project name and scope
   - Date of prioritization exercise
   - Iteration number or version
   - Key stakeholders involved

3. **Evaluate each hypothesis:**
   - Ensure proper format: "We believe that [business outcome] will be achieved if [user] attains [benefit] with [feature]"
   - Assess value (high/low) with objective justification
   - Evaluate risk (high/low) with specific uncertainties
   - Document existing evidence

4. **Categorize hypotheses into quadrants:**
   - **Test** (High value, High risk): Design experiments to reduce risks
   - **Ship & Measure** (High value, Low risk): Plan implementation with metrics
   - **Don't test** (Low value, Low risk): Identify table stakes or discard
   - **Discard** (Low value, High risk): Document rationale for rejection

5. **Plan immediate actions:**
   - Prioritize test hypotheses by learning value
   - Sequence ship hypotheses by development efficiency
   - Create timeline for testing and implementation

6. **Validate output quality:**
   - Hypotheses follow correct format
   - Assessments are objective with reasoning
   - Quadrant placements match evaluations
   - Actions are specific and prioritized

## Output Format

Create a markdown file at `docs/product/hypothesis_prioritization_canvas.md` with this structure:

```markdown
# Hypothesis Prioritization Canvas: [Project Name]

## Project Details
- **Project Name:** [Name]
- **Date:** [Date]
- **Iteration:** [Number]

## Hypothesis Evaluation

### Quadrant 1: Test (High Value, High Risk)
**Hypothesis 1:** [Hypothesis statement]
- **Value:** High - [Justification]
- **Risk:** High - [Justification]
- **Uncertainties:** [Main uncertainties]
- **Testing Approach:** [Proposed experiment]

### Quadrant 2: Ship & Measure (High Value, Low Risk)
**Hypothesis 2:** [Hypothesis statement]
- **Value:** High - [Justification]
- **Risk:** Low - [Justification]
- **Metrics:** [Success measures]

### Quadrant 3: Don't Test (Low Value, Low Risk)
**Hypothesis 3:** [Hypothesis statement]
- **Value:** Low - [Justification]
- **Risk:** Low - [Justification]
- **Decision:** [Foundation or Discard]

### Quadrant 4: Discard (Low Value, High Risk)
**Hypothesis 4:** [Hypothesis statement]
- **Value:** Low - [Justification]
- **Risk:** High - [Justification]
- **Original Motivation:** [Why was this hypothesis considered]
- **Reason for Discarding:** [Why are we discarding it now]

## Next Steps
1. [Specific action for Hypothesis X]
2. [Specific action for Hypothesis Y]
3. [Specific action for Hypothesis Z]

## Review Schedule
This canvas will be reviewed after completion of the first test series or in [timeframe].
```

## Success Criteria

- All hypotheses follow the format: "We believe that [business outcome] will be achieved if [user] attains [benefit] with [feature]"
- Value and risk assessments are objective and justified
- Quadrant placements accurately reflect evaluations
- High-value, high-risk hypotheses have clear learning plans
- High-value, low-risk hypotheses have measurement plans
- Next steps are actionable with specific timelines
- Process demonstrates objective evaluation without bias

$ARGUMENTS