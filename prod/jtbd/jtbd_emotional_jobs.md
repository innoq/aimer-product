# JTBD Emotional Jobs

## Purpose

Identification and analysis of emotional jobs that users want to fulfill or avoid during the completion of functional jobs.

## Context

Emotional jobs represent the feelings that users want to experience or avoid while completing their functional jobs. These emotional dimensions are crucial for designing products and services that are not only functional but also emotionally appealing.

## Instructions

1. Analyze the role, job, and context to identify relevant emotional states:
   - Consider the emotional needs of the focused users
   - Account for the specific context of job completion
   - Understand the connection between functional and emotional aspects

2. Generate desired emotions:
   - Create a complete list of emotions that are desired during job completion
   - Begin each desired emotion with "Feel". Example: "Feel excitement"
   - Provide a brief explanation for each emotion that connects it to the role, job, and context

3. Generate undesired emotions:
   - Create a complete list of emotions that should be avoided during job completion
   - Begin each undesired emotion with "Avoid feeling". Example: "Avoid feeling: sadness"
   - Provide a brief explanation for each emotion that connects it to the role, job, and context

4. Formatting rules:
   - Group titles should be bold formatted
   - Disregard context if none is provided
   - Output should be a numbered list
   - Use correct Markdown

### Language Guidelines

- Use exclusively inclusive language and correct gendering
- Use gender-neutral formulations like "users", "applicants" or "people"
- Use the gender asterisk (*) when gender-neutral formulations are not possible
- Examples: "user*s", "developer*s", "applicant*s"

## Output Format

**Desired Emotions:**

1. Feel [emotion] - [Brief explanation connecting the emotion to role, job, and context]
2. Feel [emotion] - [Brief explanation connecting the emotion to role, job, and context]
[Continue for all desired emotions]

**Undesired Emotions:**

1. Avoid feeling: [emotion] - [Brief explanation connecting the emotion to role, job, and context]
2. Avoid feeling: [emotion] - [Brief explanation connecting the emotion to role, job, and context]
[Continue for all undesired emotions]

## Success Criteria

- All desired emotions begin with "Feel"
- All undesired emotions begin with "Avoid feeling"
- Each emotion has a brief explanation connecting it to role, job, and context
- Lists are complete and relevant to the specific job context
- Inclusive language is used throughout
- Output is saved in the correct path: docs/domain/jtbd/[job-name]/05-emotional-jobs.md

$ARGUMENTS