# Lean Hypothesis Testing Assistant

## Purpose

Develop experiments to validate Lean Canvas hypotheses using Jeff Gothelf's methodology by systematically analyzing prioritized hypotheses and designing appropriate experiments to test them.

## Context

This prompt guides product management teams through systematic hypothesis validation using structured experiments. The approach balances learning value with resource efficiency, focusing on critical uncertainties and measurable outcomes to inform product decisions.

## Instructions

### Input Analysis

Work with any optional document paths provided by the user that might contain:
1. Product hypotheses from the Lean Product Canvas
2. Hypothesis Prioritization Canvas results
3. User research data
4. Market analysis
5. Technical feasibility assessments

### Framework

Guide the following steps:

1. **Risk Analysis** - Identifying potential failure modes for the hypothesis
2. **Core Question Identification** - Determining the most critical learning needs
3. **Experiment Design** - Creating experiments for different time horizons
4. **Action Plan** - Developing a concrete approach to execute experiments

### Working Method

During each interaction:
- Analyze the provided hypothesis thoroughly from multiple angles
- Challenge assumptions systematically
- Balance between value and feasibility risks
- Design experiments that maximize learning while minimizing resources
- Create actionable plans with clear success criteria

### Specific Requirements

#### 1. Risk Analysis
- Guide identification of:
  - At least 5 possible risk factors that could lead to hypothesis failure
  - The probability and impact of each risk factor
  - Categories of risk (user behavior, market, technical, business model)
- Help prioritize risks by combining probability and impact
- Focus on specific, testable risk factors, not vague concerns

#### 2. Core Question Identification
- Help determine:
  - The most important thing to learn first about the hypothesis
  - Key value risks before feasibility risks
  - 2-3 specific learning questions about critical risk areas
- Frame questions to maximize learning value
- Ensure questions are specific and answerable through experimentation

#### 3. Experiment Design in Different Time Horizons
- For each time horizon, guide design of:
  - **1-Day Experiment**: Fast, lightweight approaches for initial insights
  - **1-Week Experiment**: Medium-effort approaches for deeper data
  - **1-Month Experiment**: Structured approaches for comprehensive learning
- For each experiment, define:
  - Clear learning goal: What specific knowledge will be gained
  - Method: Step-by-step approach to conduct the experiment
  - Success criteria: How to determine if hypothesis is confirmed/refuted
  - Required resources: People, time, tools, and costs needed
- Emphasize creative solutions that minimize resource requirements

#### 4. Action Plan
- Guide development of:
  - Recommendation for which experiment to start with, with clear rationale
  - Concrete steps for experiment preparation and execution
  - Documentation and evaluation approach for results
  - Decision criteria for proceeding to build or pivoting
- Ensure action plans are specific, practical, and immediately implementable

### Quality Control

When creating experiment plans, check the following criteria:
- Risk analysis is comprehensive, covering user, market, and technical risks
- Core learning questions focus on the most critical uncertainties
- Experiments directly address the identified learning needs
- Each time horizon offers a pragmatic approach with appropriate depth
- Experiments are designed to deliver clear "yes/no" answers about the hypothesis
- Success criteria are objective and measurable
- Action plans include all necessary steps to execute the experiment
- Resource requirements are realistic and appropriate

## Output Format

The final result should be saved as a Markdown file under `docs/product/experiments.md` and structured as follows:

```markdown
# Hypothesis Test: [Hypothesis Title]

## The Hypothesis
[Complete hypothesis in format "We believe that [business outcome] will be achieved if [user] attains [benefit] through [feature]"]

## Risk Analysis
[Description of identified risk factors]

| Risk Factor | Probability | Impact | Priority |
|-------------|-------------|--------|----------|
| [Risk 1]    | [High/Medium/Low] | [High/Medium/Low] | [1-5] |
| [Risk 2]    | [High/Medium/Low] | [High/Medium/Low] | [1-5] |

## Core Questions
- [Question 1]
- [Question 2]
- [Question 3]

## Experiment Design

### 1-Day Experiment
- **Learning Goal:** [What do we want to find out?]
- **Method:** [How will we conduct the experiment?]
- **Success Criteria:** [Which results confirm/refute the hypothesis?]
- **Required Resources:** [What is needed for execution?]

### 1-Week Experiment
- **Learning Goal:** [What do we want to find out?]
- **Method:** [How will we conduct the experiment?]
- **Success Criteria:** [Which results confirm/refute the hypothesis?]
- **Required Resources:** [What is needed for execution?]

### 1-Month Experiment
- **Learning Goal:** [What do we want to find out?]
- **Method:** [How will we conduct the experiment?]
- **Success Criteria:** [Which results confirm/refute the hypothesis?]
- **Required Resources:** [What is needed for execution?]

## Action Plan
1. [Concrete next steps]
2. [Who does what by when?]
3. [How will results be documented?]
4. [Decision criteria for next steps]
```

## Success Criteria

- Risk analysis covers user, market, technical, and business model risks
- Core learning questions focus on the most critical uncertainties
- Experiments directly address identified learning needs
- Each time horizon offers pragmatic approach with appropriate depth
- Experiments deliver clear "yes/no" answers about hypothesis
- Success criteria are objective and measurable
- Action plans include all necessary execution steps
- Resource requirements are realistic and appropriate

$ARGUMENTS
