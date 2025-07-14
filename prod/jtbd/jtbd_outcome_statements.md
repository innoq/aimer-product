# JTBD Outcome Statements

## Purpose

Create comprehensive outcome statements for a specific job that help product teams understand the metrics by which users evaluate the success of job execution.

## Context

Outcome statements are measurable criteria that define what users evaluate as successful. They help identify solution-independent improvement opportunities and prioritize product decisions.

## Instructions

Analyze the provided parameters and create outcome statements based on the following guidelines:

1. **Complete Analysis**: Analyze job, context, and focus from the perspective of the specified users. Consider both functional and emotional aspects of job execution.

2. **Identify Relevant Topics**: Identify relevant topics for outcome statements (approximately 1 topic per 4-5 statements). Topics should reflect central concerns of users, such as efficiency, reliability, etc.

3. **Outcome Statement Format**: Generate outcome statements for each topic with the following format:
   - **Direction of Change** (minimize, maximize, increase, decrease, etc.)
   - **Metric** (time, probability, frequency, number, etc.)
   - **Control Object** (the thing that is improved/reduced, etc.)
   - **Contextual Qualifier** (when, where, or under what conditions)

4. **Quality Criteria**: Ensure outcome statements are:
   - Measurable (can be evaluated on a scale)
   - Solution-independent (not tied to specific features)
   - Outcome-oriented (not activity-oriented)
   - Free from vague adjectives and adverbs
   - Comprehensive (cover the entire job execution process)
   - MECE (mutually exclusive, collectively exhaustive)

5. **Thematic Organization**: Organize statements by topics with topic names as headings.

6. **Distribution**: About 80% of statements should focus on desired improvements, while 20% should focus on avoiding negative outcomes.

### Language Guidelines

- Use exclusively inclusive language and correct gendering
- Use gender-neutral formulations like "users", "applicants" or "people"
- Use the gender asterisk (*) when gender-neutral formulations are not possible
- Examples: "user*s", "developer*s", "applicant*s"

## Output Format

# Outcome Statements: [Job]

## [Topic 1]
1. [Direction] [Metric] of [Control Object] [contextual qualifier].
2. [Direction] [Metric] of [Control Object] [contextual qualifier].
3. [Direction] [Metric] of [Control Object] [contextual qualifier].
...

## [Topic 2]
1. [Direction] [Metric] of [Control Object] [contextual qualifier].
2. [Direction] [Metric] of [Control Object] [contextual qualifier].
...

[Continue for all topics]

Save the analysis as a Markdown file at: docs/domain/jtbd/[job-name]/07-outcome-statements.md

## Success Criteria

- All {{n}} outcome statements are generated
- Statements follow the specified format
- Topics cover all relevant aspects
- 80/20 distribution between improvements and avoidance is maintained
- Inclusive language is used throughout

$ARGUMENTS