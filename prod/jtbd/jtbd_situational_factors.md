# JTBD Situational Factors

## Purpose

Generate a list of situational factors that could influence the job performance of specific users. These factors are used in a survey where respondents rate each factor on a scale from 1 (low) to 5 (high).

## Context

Situational factors help understand the variable conditions that influence job execution. This analysis enables the development of context-specific solutions and optimizes the user experience under different circumstances.

## Instructions

Analyze the provided parameters and create situational factors based on the following guidelines:

1. **Establish Topics**: Create 3-5 comprehensive topics that cover all job aspects. Add one topic for every 5 additional factors when {{n}} > 15.

2. **Generate Situational Factors**: Create {{n}} mutually exclusive and collectively exhaustive (MECE) situational factors relevant to job, context, and focus. Formulate factors as questions beginning with "How is/was the level of..." or similar, and focus on external, variable conditions, not on user capabilities.

3. **Group Factors by Topics**: Assign each factor to one or more topics and maintain balance. Combine multiple topics per factor for lower {{n}} values to ensure comprehensive coverage.

4. **Format Output**: Present results as survey tables, grouped by topics.

### Language Guidelines

- Use exclusively inclusive language throughout
- Use gender-neutral formulations like "users", "applicants", or "people"
- Avoid gendered assumptions and use inclusive terms for all roles
- Examples: "users", "developers", "applicants", "team members", "individuals"

## Output Format

The situation is rated by survey participants on a scale from 1 to 5, where 1 is the worst case and 5 is the best case.

### Topic 1: [Topic Name]

|Situations/Complexities|1 (Worst Case)|2|3|4|5 (Best Case)|
|---|---|---|---|---|---|
|[Factor 1]|[Worst Case]||||[Best Case]|
|[Factor 2]|[Worst Case]||||[Best Case]|
|[Factor 3]|[Worst Case]||||[Best Case]|
|[Factor 4]|[Worst Case]||||[Best Case]|
|[Factor 5]|[Worst Case]||||[Best Case]|

### Topic 2: [Topic Name]

|Situations/Complexities|1 (Worst Case)|2|3|4|5 (Best Case)|
|---|---|---|---|---|---|
|[Factor 6]|[Worst Case]||||[Best Case]|
|[Factor 7]|[Worst Case]||||[Best Case]|
|[Factor 8]|[Worst Case]||||[Best Case]|
|[Factor 9]|[Worst Case]||||[Best Case]|
|[Factor 10]|[Worst Case]||||[Best Case]|

[Continue for all topics]

Save the analysis as a Markdown file at: docs/domain/jtbd/[job-name]/06-situational-factors.md

## Success Criteria

- All {{n}} situational factors are identified
- Factors follow the MECE principle
- Topics cover all job aspects
- Tables are clearly structured and comprehensible
- Inclusive language is used throughout

$ARGUMENTS