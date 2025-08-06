# JTBD Broaden Abstraction Level

## Purpose

Identify higher-level jobs or goals that explain why specific users execute a specific job in a given context.

## Context

Broadening the abstraction level helps understand the strategic motivations and higher-level goals behind individual jobs. This enables the development of innovative solution approaches and captures the broader context of user needs.

## Instructions

Analyze the provided parameters and identify higher-level jobs based on the following guidelines:

1. **Input Analysis**: Thoroughly examine users, job, and context.

2. **Higher-level Job Identification**: Determine {{number}} higher-order jobs with a superset of supporting goals.

3. **Current Job Embedding**: Ensure the provided job is contained within the superset.

4. **Consider New Users**: Higher-level jobs may have completely different users (e.g., orchestrators vs. executors).

5. **Formatting**: Formulate each higher-level job as a Job-to-be-Done with gerund form (ending in "-ing").

6. **Structured Presentation**: Create a numbered list with the following elements:
   - **Bold Job Title**: Brief explanation with context and reasoning
   - **Current Job Role**: Explanation of how the current job is a mini-goal within the higher-level job
   - **New Users**: If different, justify the new users based on their functional role

### Language Guidelines

- Use exclusively inclusive language throughout
- Use gender-neutral formulations like "users", "applicants", or "people"
- Avoid gendered assumptions and use inclusive terms for all roles
- Examples: "users", "developers", "applicants", "team members", "individuals"

## Output Format

1. **[Job Title]**: [Brief explanation with context and reasoning]
   - **Current Job Role**: [Explanation of embedding]
   - **New Users**: [If applicable, justification of new users]

2. **[Job Title]**: [Brief explanation with context and reasoning]
   - **Current Job Role**: [Explanation of embedding]
   - **New Users**: [If applicable, justification of new users]

Save the analysis as a Markdown file at: docs/domain/jtbd/[job-name]/02-broaden-abstraction.md

## Success Criteria

- All {{number}} higher-level jobs are identified
- Each higher-level job is clearly justified
- The role of the current job is explained in each higher-level job
- New users are functionally justified
- Inclusive language is used throughout

$ARGUMENTS