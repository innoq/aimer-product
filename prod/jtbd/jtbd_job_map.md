# JTBD Job Map

## Purpose

Create a comprehensive job map that covers all nine sequential phases of the JTBD framework while identifying the capabilities and steps that users need to successfully complete a specific job.

## Context

The job map is a central instrument in the Jobs-to-be-Done framework that presents the entire spectrum of user needs in structured form. It helps identify improvement opportunities and optimize products or services in a targeted manner.

## Instructions

Analyze the given parameters and create a structured job map based on the following guidelines:

1. **JTBD Framework**: Consider all 9 sequential phases:
   - Define: What must be defined, planned, or evaluated by users?
   - Locate: Which resources must be located, collected, or retrieved?
   - Prepare: How must inputs or environments be prepared?
   - Confirm: What must be verified, prioritized, or decided?
   - Execute: What is the primary execution action?
   - Monitor: What must be monitored for successful execution?
   - Resolve: Which problems might need to be solved?
   - Modify: What might need to be adjusted or modified?
   - Conclude: What must be done to complete the job?

2. **Step Generation**: Create at least one step per phase, begin each step with a verb, and focus on what users want to achieve faster or better.

3. **Fidelity Requirements**: Adhere to the specified level of detail (Low: 10-12 steps, Medium: 13-14 steps, High: 15-18 steps).

4. **MECE Principle**: Ensure that steps are mutually exclusive and collectively exhaustive.

5. **Scoping**: Start at {{start_point}} and end at {{end_point}}, if specified.

### Language Guidelines

- Use exclusively inclusive language and correct gendering
- Use gender-neutral formulations like "users", "applicants" or "people"
- Use the gender asterisk (*) when gender-neutral formulations are not possible
- Examples: "user*s", "developer*s", "applicant*s"

## Output Format

Format each step as follows:
1. **Step Name** - The ability to [explanation].
2. **Next Step Name** - The ability to [explanation].

Save the analysis as a Markdown file at: docs/domain/jtbd/[job-name]/01-job-map.md

## Success Criteria

- All 9 JTBD phases are covered
- Steps follow the MECE principle
- Fidelity requirements are met
- Inclusive language is used throughout
- Job map is logically structured and comprehensible

$ARGUMENTS