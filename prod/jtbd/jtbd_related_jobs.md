# JTBD Related Jobs

## Purpose

Create a comprehensive list of tasks or goals that must be completed by users before, during, and after a specific job.

## Context

Related jobs help understand the entire ecosystem of tasks connected to a central job. This analysis shows the complete user journey and identifies improvement opportunities beyond the core job.

## Instructions

Analyze the provided parameters and create a structured list of related jobs based on the following guidelines:

1. **Complete Analysis**: Consider the users' perspective, the nature of the job, the given context, and the focus.

2. **Three-Category Structure**: Generate tasks for three categories: "Before", "During", and "After" the specified job. Each category should contain at least 5 tasks.

3. **Job-to-be-Done Format**: Formulate each task as a Job-to-be-Done, using the same verb structure as the provided job. For example, if the job is "organizing", use verbs ending in "-ing".

4. **Provide Explanations**: Give a brief explanation for each task of its importance or how it contributes to the overall job.

5. **Structured Formatting**: Use bold category headings and numbered tasks with bold task titles.

### Language Guidelines

- Use exclusively inclusive language and correct gendering
- Use gender-neutral formulations like "users", "applicants" or "people"
- Use the gender asterisk (*) when gender-neutral formulations are not possible
- Examples: "user*s", "developer*s", "applicant*s"

## Output Format

**Before {{Job}}**

1. **[Task 1]** - [Brief explanation]
2. **[Task 2]** - [Brief explanation]
...

**During {{Job}}**

1. **[Task 1]** - [Brief explanation]
2. **[Task 2]** - [Brief explanation]
...

**After {{Job}}**

1. **[Task 1]** - [Brief explanation]
2. **[Task 2]** - [Brief explanation]
...

Save the analysis as a Markdown file at: docs/domain/jtbd/[job-name]/05-related-jobs.md

## Success Criteria

- All three categories (Before, During, After) are completely filled out
- Each category contains at least 5 relevant tasks
- All tasks are formulated as Jobs-to-be-Done
- Each task has a clear explanation of its relevance
- Inclusive language is used throughout

$ARGUMENTS