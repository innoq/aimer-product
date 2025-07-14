# JTBD Narrow Abstraction Level

## Purpose

Identify potential obstacles that might prevent users from successfully completing a specific job in a given context, and formulate these as action-oriented Jobs-to-be-Done.

## Context

Narrowing the abstraction level helps understand concrete challenges and barriers that can occur during job execution. This analysis enables the development of targeted solutions and improves the user experience.

## Instructions

Analyze the provided parameters and identify obstacles based on the following guidelines:

1. **Understand the Inputs**:
   - Analyze the users: What key characteristics, needs, and potential limitations are relevant?
   - Break down the job into core components: What actions, decisions, or outcomes are involved?
   - Examine the context: What environmental, social, or technological factors can influence users' ability?

2. **Brainstorm Potential Obstacles**:
   - Generate a list of potential obstacles (physical, cognitive, emotional, and external factors)
   - Ensure obstacles are mutually exclusive and collectively exhaustive (MECE principle)

3. **Transform Obstacles into Jobs-to-be-Done**:
   - Formulate each obstacle as a Job-to-be-Done with gerund form (e.g., "Finding", "Understanding", "Managing")
   - Express the challenge as an action that users must accomplish

4. **Evaluate and Refine**:
   - Evaluate each Job-to-be-Done for clarity, relevance, and action-orientation
   - Verify that the final list meets the MECE principle

### Language Guidelines

- Use exclusively inclusive language and correct gendering
- Use gender-neutral formulations like "users", "applicants" or "people"
- Use the gender asterisk (*) when gender-neutral formulations are not possible
- Examples: "user*s", "developer*s", "applicant*s"

## Output Format

1. **{Job-to-be-Done 1 in Gerund Form}**: {Brief explanation of why this could be an obstacle and how it relates to users, job, and context}
2. **{Job-to-be-Done 2 in Gerund Form}**: {Explanation...}
3. **{Job-to-be-Done 3 in Gerund Form}**: {Explanation...}
...(Continue the list as needed)...

Save the analysis as a Markdown file at: docs/domain/jtbd/[job-name]/03-narrow-abstraction.md

## Success Criteria

- All relevant obstacles are identified
- Each obstacle is formulated as an action-oriented Job-to-be-Done
- The list follows the MECE principle
- All Jobs-to-be-Done are clear, relevant, and action-oriented
- Inclusive language is used throughout

$ARGUMENTS