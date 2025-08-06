# Lean Product Canvas Builder

## Purpose

Create comprehensive Lean Product Canvases using Jeff Gothelf's methodology to identify business problems, outcomes, users, solutions, and hypotheses in a clear, step-by-step process.

## Context

Product teams need a structured approach to connect business problems to user needs and potential solutions. This tool guides the creation of Lean Product Canvases that translate vague ideas into concrete, testable hypotheses for product decisions.


## Instructions

1. **Analyze input documents** containing:
   - Market research data
   - User interviews
   - Business plans
   - Existing product documentation
   - Competitive analysis

2. **Define business problem:**
   - Identify the most important problem to focus on now
   - Determine original motivation for building the product/feature
   - Analyze market changes, customer needs, or technological shifts
   - Create specific, actionable problem statements

3. **Establish business outcomes:**
   - Define clear metrics to track problem resolution
   - Identify expected behavior changes if solutions work
   - Format metrics as "who-does what-by how much"
   - Connect to business success indicators (lifetime value, retention, usage)

4. **Identify users:**
   - Determine key user personas to focus on first
   - Distinguish who buys, uses, configures, and is impacted by the product
   - Create specific persona descriptions (demographic, behavioral, needs-based)

5. **Define user outcomes & benefits (JTBD):**
   - Explore why users would seek out the product/service
   - Identify benefits users would gain
   - Apply Jobs To Be Done framework
   - Connect user benefits to identified problems

6. **Explore solutions:**
   - Identify potential solutions addressing business problems and user needs
   - Align solutions with business problems and user outcomes
   - Prioritize by feasibility, desirability, and viability

7. **Create hypotheses:**
   - Format: "We believe that [business outcome] will be achieved if [user] attains [benefit] with [feature]"
   - Focus on one feature per hypothesis
   - Ensure hypotheses are testable and connected to metrics

8. **Prioritize learning:**
   - Identify which hypothesis to test first
   - Assess potential failure points and risks
   - Focus on value risks before feasibility risks

9. **Design minimal experiments:**
   - Create minimum effort experiments for risky assumptions
   - Design learning approaches for different timeframes (1 day, 1 week, 1 month)
   - Emphasize speed and learning over perfect implementation

10. **Validate quality:**
    - Problem statements are specific and actionable
    - Business outcomes are measurable and connected to problems
    - User personas are specific and relevant
    - Solutions align with problems and outcomes
    - Hypotheses follow correct format
    - Learning priorities focus on value risks first

## Output Format

Create a markdown file at `docs/product/lean_product_canvas.md` with this structure:

```markdown
# Lean Product Canvas: [Product Name]

## Business Problem
[Description of the central business problem]

## Business Outcomes
[Measurable business outcomes and metrics]

## Users
[Description of user personas]

## Benefits & Value
[Jobs-to-be-Done and value propositions]

## Solutions
[Potential solution approaches]

## Hypotheses
[Testable hypotheses in format "We believe that [business outcome] will be achieved if [user] attains [benefit] through [feature]"]

## Learning Priorities
[Most important assumptions and risks to test]

## Minimum Learning Effort
[Lightweight experiments for validation]
```

## Success Criteria

- Problem statements are specific and actionable, not vague market observations
- Business outcomes are measurable and connected to solving identified problems
- User personas are specific and relevant to business problems
- User benefits connect directly to identified problems
- Solutions align with both business problems and user outcomes
- Hypotheses follow correct format and each focuses on single feature
- Learning priorities focus on value risks before feasibility risks
- Experiment designs are lightweight and focused on fast learning

$ARGUMENTS