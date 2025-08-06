# JTBD Resume Workflow

## Purpose

Resume an already started JTBD analysis process and continue it. Build on the existing index document to capture the current status and plan the next steps.

## Context

This prompt helps with the systematic resumption of JTBD analyses by evaluating status, restoring context, prioritizing next steps, and continuing the analysis in a structured manner. It ensures consistency and coherence between different analysis steps.

## Instructions

1. **Status Evaluation**
   - Analyze the specified index document to determine the current state of the JTBD analysis process
   - Identify:
     - Already completed steps (marked with ✅)
     - Outstanding steps (marked with ❌)
     - Existing end user, job, and context definitions
     - Insights gathered so far

2. **Context Restoration**
   - Read the relevant existing documents to understand context and previous insights
   - Restore the key parameters:
     - End user and their characteristics
     - Job definition and scope
     - Context specifications
     - Assumptions and framework conditions

3. **Prioritization of Next Steps**
   - Identify the logically next steps based on:
     - Natural progression of JTBD analysis
     - Priorities specified by users
     - Current gaps in the analysis
     - Potential for valuable insight generation

4. **Continuation Plan**
   - Create a concrete plan for continuing the analysis with:
     - Specific next steps
     - Required inputs for each step
     - Expected outputs
     - Estimated effort

5. **Execution Phase**
   For each prioritized, not yet completed step:
   - Collect and prepare all necessary parameters for the corresponding prompt
   - Execute the corresponding specialized prompt from `./.claude/commands/`
   - Save results in the correct directory
   - Update the index document with status update, link to new document, date, and summary

6. **Session Completion**
   After completing the session or reaching the session goal:
   - Create a brief summary of completed steps and gained insights
   - Perform a final update of the index document
   - Recommend the next steps to prioritize for future sessions

### Language Guidelines

- Use exclusively inclusive language throughout
- Use gender-neutral formulations like "users", "applicants", or "people"
- Avoid gendered assumptions and use inclusive terms for all roles
- Examples: "users", "developers", "applicants", "team members", "individuals"

## Output Format

# JTBD Workflow Resume for [Job Name]

## Status Evaluation
[Current state of analysis based on index document]

## Restored Context
- **End User:** [Description]
- **Job:** [Definition]
- **Context:** [Specifications]
- **Previous Insights:** [Summary]

## Prioritized Next Steps
1. [Step 1] - [Justification]
2. [Step 2] - [Justification]
3. [Step 3] - [Justification]

## Continuation Plan
[Detailed plan for the session]

## Execution
[Documentation of performed steps]

## Session Summary
[Completed steps, insights, next recommendations]

### Output Path
Update the index document at: docs/domain/jtbd/[job-name]/README.md

## Success Criteria

- Complete status evaluation of existing index document
- Successful restoration of all relevant context information
- Logical prioritization of next steps
- Consistent execution of planned analysis steps
- Update of index document with new insights
- Inclusive language used throughout
- Coherence between different analysis steps ensured

$ARGUMENTS