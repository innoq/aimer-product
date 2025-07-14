# JTBD Workflow Chain

## Purpose

Conduct a structured process for creating comprehensive Jobs-to-be-Done documentation. Use specialized JTBD prompts in the optimal sequence.

## Context

The JTBD workflow enables systematic analysis of user jobs through modular prompts. Each step builds on the results of previous steps and contributes to complete documentation.

## Instructions

### Language Guidelines

- Use exclusively inclusive language and correct gendering
- Use gender-neutral formulations like "users", "applicants" or "people"
- Use the gender asterisk (*) when gender-neutral formulations are not possible
- Examples: "user*s", "developer*s", "applicant*s"

### Input Variables

- **End User:** [Who performs the job?]
- **Job:** [The main job to be completed]
- **Focus:** [B2C for consumer context, B2B for business context, NA for functional analysis]
- **Product/Service:** [Optional: The solution for which JTBD analyses are performed]
- **Domain:** [Optional: The domain context in which the job takes place]
- **Session:** [Optional: Current state of workflow - new, continued, or concluding]

## Workflow Management

Before starting each JTBD analysis session:

1. **Check Workflow Status**
   - Check if an index document exists at `docs/domain/jtbd/README.md`
   - If yes, analyze the current state and identify already completed steps
   - If no and this is not a new analysis, create a basic index document

2. **Progressive Index Document**
   - The index document serves both as documentation entry point and progress indicator
   - After each completed analysis step, update the index document with:
     - A brief summary of new insights
     - Links to the new document
     - An updated progress indicator showing which steps have been completed
   - Save the updated index document to maintain progress between sessions

## Basic Workflow Steps

1. **Jobs and Performers** (`./jtbd_jobs_and_performers.md`)
   - Input: Domain, Focus, Market, Number of Jobs
   - Output: Basic jobs and their performers
   - Purpose: Identifies central jobs in the application domain

2. **Job Contexts** (`./jtbd_job_contexts.md`)
   - Input: End User, Job, Focus
   - Output: Various contexts in which the job is performed
   - Purpose: Defines the scope of investigation

3. **Job Maps** (`./jtbd_job_map.md`)
   - Input: End User, Job, Context, Focus, Fidelity
   - Output: Basic job map with 9 phases
   - Purpose: Creates the foundation for further analyses

4. **Broaden the level of abstraction** (`./jtbd_broaden_abstraction.md`)
   - Input: End User, Job, Context (from step 2), Focus
   - Output: Higher-level goals behind the job
   - Purpose: Captures the strategic context

5. **Narrow the level of abstraction** (`./jtbd_narrow_abstraction.md`)
   - Input: End User, Job, Context (from step 2), Focus
   - Output: More concrete subtasks
   - Purpose: Develops more detailed understanding

## Extended Analysis

6. **Job Hierarchies** (`./jtbd_job_hierarchies.md`)
   - Input: End User, Product/Service, Focus, Context
   - Output: Hierarchical structure of jobs at different abstraction levels
   - Purpose: Shows relationships between strategic and tactical jobs

7. **Related Jobs** (`./jtbd_related_jobs.md`)
   - Input: End User, Job, Context, Focus
   - Output: Tasks occurring before, during, and after the main job
   - Purpose: Identifies adjacent activities

8. **Situational Factors** (`./jtbd_situational_factors.md`)
   - Input: End User, Job, Context, Focus
   - Output: External factors that influence the job
   - Purpose: Captures environmental variables

## Outcome and Success Measurement

9. **Outcome Statements** (`./jtbd_outcome_statements.md`)
   - Input: End User, Job, Context, Focus, Number of statements
   - Output: Desired outcomes and success metrics
   - Purpose: Defines measurable user expectations

10. **Success Metrics** (`./jtbd_success_metrics.md`)
    - Input: End User, Job, Context, Focus, Steps from job map
    - Output: Success metrics for each step
    - Purpose: Defines concrete success criteria

11. **Unmet Needs** (`./jtbd_unmet_needs.md`)
    - Input: End User, Job, Context, Focus, Number of needs
    - Output: Unmet needs of users
    - Purpose: Identifies innovation potential

## User Perspective

12. **Job Personas** (`./jtbd_job_personas.md`)
    - Input: End User Category, Job, Context, Number of Personas, Focus
    - Output: Archetypes of users based on their job approach
    - Purpose: Represents different user groups

13. **Job Stories** (`./jtbd_job_stories.md`)
    - Input: End User, Job, Context, Product/Service, Categories, Stories per category, Focus
    - Output: Context-based job stories
    - Purpose: Describes situational user applications

14. **Emotional Jobs** (`./jtbd_emotional_jobs.md`)
    - Input: End User, Job, Context, Focus
    - Output: Emotional needs during execution
    - Purpose: Captures emotional aspects

15. **Social Jobs** (`./jtbd_social_jobs.md`)
    - Input: End User, Job, Context, Focus
    - Output: Social aspects and perception goals
    - Purpose: Analyzes interaction needs

## Solution and Implementation Strategy

16. **Approaches** (`./jtbd_approaches.md`)
    - Input: End User, Steps from job map, Job context
    - Output: Solution approaches for each step
    - Purpose: Develops implementation strategies

17. **Financial Metrics** (`./jtbd_financial_metrics.md`)
    - Input: End User, Job, Context, Focus
    - Output: Financial aspects and TCO
    - Purpose: Evaluates economic factors

18. **Potential Jobs of a Solution** (`./jtbd_potential_jobs.md`)
    - Input: End User, Product/Solution
    - Output: Jobs that could be supported by a solution
    - Purpose: Validates solution approaches

19. **Forces Diagram** (`./jtbd_forces_diagram.md`)
    - Input: End User, Job, Context, Solution/Product, Focus
    - Output: Analysis of forces that promote or inhibit adoption
    - Purpose: Visualizes decision factors

## Market Research and Validation

20. **Profiling & Screening Accelerator** (`./jtbd_profiling_screening.md`)
    - Input: End User, Job, Context, Focus
    - Output: Screening questions for research
    - Purpose: Prepares user research

21. **Survey Design** (`./jtbd_survey.md`)
    - Input: End User, Job, Context, Focus, Language
    - Output: Comprehensive JTBD survey
    - Purpose: Enables quantitative validation

## Ergebnisintegration

## Output Format

### Documentation Structure

```
docs/domain/jtbd/
├── README.md (Index document)
├── [job-name]/
│   ├── 01-jobs-and-performers.md
│   ├── 02-job-contexts.md
│   ├── 03-job-map.md
│   └── [...additional analysis documents]
```

### Individual Analysis Documents

Each analysis document contains:
- Analysis step and date
- Used input variables
- Results in structured form
- References to related analysis steps

## Success Criteria

- Complete JTBD documentation with all desired analysis steps
- Consistent use of inclusive language and correct gendering
- Updated index document with all links and progress indicators
- Structured storage of all results under `docs/domain/jtbd/`

## JTBD Documentation Index

22. **JTBD Index Creation and Maintenance**
    - **Initial Index Document** (when starting a new JTBD analysis or continued session)
      - Create an index document containing basic information and planned analysis steps
      - Use the following structure:
        ```markdown
        # JTBD Analysis: [Job]
        
        ## End User
        [End User Description]
        
        ## Job
        [Job Description]
        
        ## Context
        [Context Description]
        
        ## Analysis Progress
        
        | Analysis Step | Status | Document | Last Update |
        |---------------|--------|----------|-------------|
        | Jobs and Performers | ❌ | - | - |
        | Job Contexts | ❌ | - | - |
        | ... | ... | ... | ... |
        
        ## Preliminary Insights
        [Will be updated as analysis progresses]
        ```
      
    - **Progressive Update** (after each completed analysis step)
      - Update the index document with:
        - Status update in the progress table (❌ → ✅)
        - Link to the created document
        - Date of last update
        - Brief summary of new insights in the "Preliminary Insights" section
      
    - **Final Index Document** (after completion of all desired analyses)
      - Supplement the index document with:
        - A comprehensive overview of the analyzed job and context
        - A detailed summary of key insights from all analyses
        - Links to all created documents with brief descriptions
        - Recommended reading order for different use cases
        - Visual representation of job hierarchy and relationships (if possible)
      
    - Save the index document after each update as:
      - `docs/domain/jtbd/README.md`

$ARGUMENTS