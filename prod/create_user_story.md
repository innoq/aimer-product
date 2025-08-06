You are an AI agent tasked with creating user stories based on a given proto persona and feature description. Your goal is to generate high-quality user stories that follow the best practices outlined by Jeff Patton, Mike Cohn, and Gojko Adzic. These user stories will be used to guide the development of this app, a Next.js / React web application in Typescript.

**ADVANCED USER STORY TECHNIQUES**

**USE MULTIPLE AGENTS** when the story creation task has independent analysis areas:
"I'll spawn agents to analyze different aspects of this user story creation:"

- One agent for persona analysis and user psychology
- One agent for feature breakdown and INVEST criteria validation
- One agent for technical feasibility and implementation hints
- One agent for QA test case design and edge case identification

**ULTRATHINK FOR COMPLEX FEATURES:**
For complex features or challenging persona-feature combinations, say:
"Let me ultrathink about this user story architecture and user journey integration before creating the stories."

**PROCRASTINATION PATTERNS (FORBIDDEN):**

- "I'll refine the acceptance criteria later" → NO, create comprehensive criteria now
- "The technical details can be vague" → NO, provide actionable implementation hints
- "Basic test cases are sufficient" → NO, cover all edge cases and error scenarios
- "This story is good enough" → NO, ensure it meets all INVEST criteria perfectly

You will be provided with these inputs:

1. <persona>
   {{$ARGUMENTS}}
   </persona>

This contains information about the target user, including their background, goals, and pain points.

2. <feature_description>
   {{$ARGUMENTS}}
   </feature_description>

This provides a high-level overview of the feature or functionality to be developed.

You should also consider:

- Current implementation status of this app
- User journeys documentation in `docs/product/user-journeys/`
- Jobs-to-be-done (JTBD) documentation in `docs/domain/jtbd/`
- Product requirements document (PRD) in `docs/product/PRD.md`
- Product backlog in `docs/product/backlog.md`
- UX documentation in `docs/` (if available)

User stories should follow the standard format with gender-inclusive and diverse language:
"As [type of user], I want [an action] so that [a benefit/a value]."

IMPORTANT: Always use gender-inclusive language in your user stories. For example:

- Use gender-neutral job titles and roles when possible
- Use diverse and inclusive examples in your descriptions
- Avoid gender stereotypes in personas and scenarios
- Ensure language is respectful and inclusive of all identities

Incorporate the following best practices when creating user stories:

1. Focus on the user's perspective and needs (Jeff Patton)
2. Keep stories simple and concise (Mike Cohn)
3. Ensure stories are valuable, estimable, small, and testable (Bill Wake's INVEST criteria)
4. Include acceptance criteria for each story (Gojko Adzic)
5. Consider the impact on the user and the business (Jeff Patton)
6. Use inclusive, gender-neutral language throughout

Follow these steps to create user stories:

1. Analyze the persona to understand the user's context, goals, and pain points.
2. Review the feature description to identify the main functionality and purpose.
3. Break down the feature into smaller, valuable chunks that align with user needs.
4. For each chunk, create a user story using the standard format.
5. Ensure each story is independent and can be developed and tested separately.
6. Add 2-5 acceptance criteria for each user story to clarify the definition of done.
7. Include technical implementation hints for developers.
8. Identify if the story is for MVP or Future Release based on available information.
9. Reference related JTBD, user journeys, UX documentation and affected personas with relative paths from `docs/`

Each story should have this structure:

```
## Description
As [user type], I want [an action] so that [a benefit/a value].

## Acceptance Criteria
1. [Criterion 1]
2. [Criterion 2]
3. [Criterion 3]
...

## JTBD Reference
- [Reference to relevant jobs-to-be-done from docs/domain/jtbd/]

## Affected Personas
- [List of personas affected by this story from docs/product/personas/]

## User Journey Reference
- [Reference to specific user journeys from docs/product/user-journeys/]

## UX Documentation
- [Reference to relevant UX documentation with relative paths from docs/]

## Implementation Scope
[MVP/Future Release]

```

Present your output in markdown format.

Here's an example of a well-formed user story for this app:

<example_story>

## Description

As a Knowledge Manager, I want to categorize prompts according to various criteria so that I can build and maintain a structured prompt library.

## Acceptance Criteria

1. Users can create and assign custom tags to prompts.
2. Users can filter and sort prompts by tags.
3. Users can adjust and extend the category structure at any time.
4. Users can provide tags with colors or icons to facilitate visual distinction.
5. Users can create nested categories to form a hierarchy.

## JTBD Reference

- "When I want to improve our family organization, I want a clear categorization so I can easily find similar areas."
- "When I search for solutions to our family challenges, I want to be able to filter by relevant categories so I can find the right approaches faster."

## Affected Personas

- Sabine Strukturiererin (docs/product/personas/01-sabine-strukturiererin.md)
- Marco Spontanplaner (docs/product/personas/02-marco-spontanplaner.md)
- Lena Netzwerkerin (docs/product/personas/03-lena-netzwerkerin.md)

## User Journey Reference

- "Familie entdeckt klyngl über Instagram" (docs/product/user-journeys/00-klyngl-ueber-instagram-entdecken.md)
- "Family Assessment durchlaufen" (docs/product/user-journeys/01-family-assessment-durchlaufen.md)

## UX Documentation

- Product Vision (docs/product/product-vision.md)
- Marketing Tone and Voice (docs/marketing/tone-and-voice.md)

## Implementation Scope

MVP
</example_story>

Remember to:

- Write user stories using gender-inclusive and diverse language.
- Always include the Implementation Scope (MVP or Future Release) in the user story.
- Create user stories that align with the provided documents and current implementation status.
- Ensure each story is independent, valuable, and testable.
- Use clear, concise language that focuses on user benefits.
- Include relevant acceptance criteria, technical notes, and references to JTBD and user journeys.
- Always include relative paths to referenced documentation (personas, user journeys, UX docs, etc.).
- Do not invent IDs for stories; they will be assigned automatically when created as GitHub issues.
- Reference specific personas from the docs/product/personas/ directory.
- Refer to user journeys documented in docs/product/user-journeys/ directory.
- Use JTBD documentation from docs/domain/jtbd/ directory.
- Reference product vision and strategy from docs/product/ directory.

Begin creating your user stories now, using the provided context as guidance.

**IMPORTANT**: After you have created the user story, add it to the local backlog (`docs/product/backlog.md`) and create a corresponding user story file in the `docs/product/user-stories/` directory with a sequential index (e.g. `46-new-user-story.md`).
