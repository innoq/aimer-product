# Plan User Story

## Purpose

Create a comprehensive plan for a user story that considers all important aspects including technical requirements, UI/UX considerations, domain modeling, and testing approaches.

## Context

User stories require detailed planning to ensure successful implementation. This prompt helps analyze user stories against INVEST criteria, identify technical challenges, and break down implementation tasks.

## Instructions

**USE MULTIPLE AGENTS** when the planning task has independent analysis areas:
"I'll spawn agents to analyze different aspects of this user story:"

- One agent for technical analysis and dependencies
- One agent for UI/UX considerations and mobile patterns
- One agent for domain modeling and persona analysis
- One agent for test planning and quality assurance

**ULTRATHINK FOR COMPLEX ANALYSIS:**
For complex user stories or challenging INVEST evaluations, say:
"Let me ultrathink about this user story breakdown and technical architecture before finalizing the plan."

**PROCRASTINATION PATTERNS (FORBIDDEN):**

- "I'll detail this in the implementation phase" → NO, plan thoroughly now
- "The technical details can be figured out later" → NO, identify challenges now
- "We'll see what's needed during development" → NO, anticipate requirements now
- "This is good enough for planning" → NO, create comprehensive plans

Analyze the user story in $ARGUMENTS and create a detailed plan covering the following aspects:

1. **INVEST-Quick-Check:**
   - Evaluate the user story against the INVEST criteria:
     - Independent – can be deployed standalone?
     - Negotiable – still room for design flexibility?
     - Valuable – noticeable benefit?
     - Estimable – do you understand enough to estimate?
     - Small – < ½ Sprint?
     - Testable – test criteria recognizable?
   - If a criterion is not met, suggest breaking down the story or gathering additional information.

2. **Implementation Details and Technical Requirements:**
   - Gather all technical details relevant for implementing the story.
   - Identify potential technical challenges and possible solution approaches without producing code examples yet.
   - List dependencies (e.g., API X, Library Y).
   - Consider security/compliance requirements.
   - Reference relevant development rules stored as Markdown files under docs/rules/ if they are relevant for implementing the story.
   - Consider using feature flags or migration paths.

3. **User Interface Information:**
   - Reference existing prototypes, screenshots, or UI designs relevant to this story.
   - Reference relevant UX documentation stored under docs/ux.
   - Mention required translations or tone-and-voice guide for text creation.
   - Consider Tailwind UI components and mobile-first design principles.

4. **Domain Information:**
   - Consider relevant personas and user journeys that are in the context of this story.
   - Reference persona files from docs/product/personas/.

5. **Existing Resources:**
   - Reference existing documentation or resources relevant to this story.
   - Briefly explain how these resources will be integrated into the planning.

6. **Acceptance Criteria:**
   - Explain how each criterion should be fulfilled.

7. **Test Plan Outline:**
   - Determine the types of tests needed (Unit, Integration, E2E).
   - Clarify if test data is needed and whether mocks or real data should be used.
   - Consider mobile testing specifics (different devices, orientations).

8. **Task Breakdown:**
   - Break down the story into maximum 1-day tasks (Code, Test, Review, Docs).
   - Do not add estimates per task, its not necessary
   - Note the order and parallelizability of tasks.

## Output Format

### Planning Document Structure

Begin your response with the heading "# Planning for User Story: [Short Story Title]" and structure the rest of the plan according to the points mentioned above.

Create a new Markdown file with the plan and save it under the directory `docs/plans/{STORY_ID}-{STORY_NAME}.md` where:
- STORY_ID is the ID of the story
- STORY_FILE_NAME is the base name of the user story file (without .md extension)
- The plan should be complete and comprehensive for future reference
- Example: If the user story file is `20100-setup-basic-application-infrastructure.md`, the plan file should be `20100-setup-basic-application-infrastructure-plan.md`

## Success Criteria

- Complete INVEST evaluation with clear recommendations
- Technical requirements identified with dependencies
- Clear task breakdown with defined order
- Comprehensive test plan outline
- Integration with existing project resources

## Tool Integration

### Multiple Agents Strategy

Leverage subagents for parallel analysis when planning has independent aspects:

**When to use:**

- Complex user stories with multiple domains (UI, API, data, testing)
- Stories requiring both technical and business analysis
- When different expertise areas need simultaneous evaluation

**How to apply:**

1. Announce: "I'll spawn agents to analyze different aspects of this user story"
2. Delegate specific analysis areas to different agents
3. Synthesize results into comprehensive plan

### Ultrathink for Complex Planning

Engage maximum reasoning for challenging planning scenarios:

**When to use:**

- Stories failing INVEST criteria requiring breakdown
- Complex technical architectures or integration challenges
- Stories with unclear requirements or multiple solution paths

**How to apply:**

1. Announce: "Let me ultrathink about this user story breakdown and technical architecture"
2. Apply deep reasoning to all aspects of the story
3. Consider multiple implementation approaches before deciding

### Sequential Thinking Tool

Use this tool to analyze complex problems step by step.

**When to use:**

- When analyzing the INVEST quick check
- When breaking down a complex user story into tasks
- When evaluating technical dependencies
- When systematically creating the test plan

**How to apply:**

1. Start with: "Let me think through this systematically using Sequential Thinking."
2. Call the tool explicitly before analyzing complex requirements or creating the task breakdown
3. Example: "I will use Sequential Thinking to create the task breakdown for implementing the user onboarding flow."

### context7 Tool

Use context7 for deeper technical information or analysis of Next.js, React, Tailwind components.

**When to use:**

- For complex integration questions between Next.js, React and other APIs and services
- For security/compliance aspects
- For technical challenges at the framework level

**How to apply:**

1. Share: "This requires deeper technical analysis. Let me research the details about [Aspect]."
2. Use precise search queries for relevant project technologies
3. Example: "I will use context7 to research secure methods for storing user data according to GDPR in React applications with mobile considerations."

$ARGUMENTS
