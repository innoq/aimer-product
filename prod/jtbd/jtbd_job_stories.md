# JTBD Job Stories

## Purpose

Development of comprehensive job stories for specific products or services that help product teams understand the situational context and motivations of users.

## Context

Job stories extend traditional user stories by emphasizing the situational context that triggers jobs. They follow the format "When [situation], I want [motivation], so that [outcome]" and help understand the circumstances that motivate users to complete certain jobs.

## Instructions

1. Analyze job, context, and users to identify different situational categories:
   - Various contexts, motivations, or job aspects
   - Situations that can trigger the job
   - Different circumstances of job completion

2. For each category create the specified number of job stories in the format:
   - **When [situational context]**
   - **I want [motivation/goal]**
   - **so that [expected outcome]**

3. Ensure that each job story:
   - Begins with a specific, realistic situational trigger
   - Clearly articulates the motivation or goal of users in this specific context
   - Ends with a concrete, valuable outcome that users expect to achieve
   - Is written from the first-person perspective of users
   - Avoids implementation details or solutions
   - Is specific enough to inform design decisions
   - Focuses on the job and its context, not on features or UI elements

4. Ensure that the complete collection of job stories:
   - Covers the full range of important situations in which the job could be performed
   - Represents different expertise levels or familiarity of users
   - Includes both common scenarios and critical edge cases
   - Follows the MECE principle (mutually exclusive and collectively exhaustive)
   - Is prioritized with the most important stories first in each category

5. After completing all job stories, add a brief section that highlights the key qualities of the job stories and explains how they should be used for product development

### Language Guidelines

- Use exclusively inclusive language and correct gendering
- Use gender-neutral formulations like "users", "applicants" or "people"
- Use the gender asterisk (*) when gender-neutral formulations are not possible
- Examples: "user*s", "developer*s", "applicant*s"

## Output Format

# Job Stories for [Product/Service]

## **1. [Category Name 1]**
- **When [situational context],**  
  **I want [motivation/goal],**  
  **so that [expected outcome].**

- **When [situational context],**  
  **I want [motivation/goal],**  
  **so that [expected outcome].**

## **2. [Category Name 2]**
- **When [situational context],**  
  **I want [motivation/goal],**  
  **so that [expected outcome].**

- **When [situational context],**  
  **I want [motivation/goal],**  
  **so that [expected outcome].**

[Continue for all categories]

---

### **Qualities of Job Stories**
- **[Quality 1]**: [Brief explanation]
- **[Quality 2]**: [Brief explanation]
- **[Quality 3]**: [Brief explanation]
- **[Quality 4]**: [Brief explanation]

## Success Criteria

- All job stories follow the format "When [situation], I want [motivation], so that [outcome]"
- Stories are organized by categories and prioritized within each category
- The collection is MECE-compliant and covers important situations
- Qualities of job stories are documented
- Inclusive language is used throughout
- Output is saved in the correct path: docs/domain/jtbd/[job-name]/04-job-stories.md

$ARGUMENTS