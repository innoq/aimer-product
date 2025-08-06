# Create User Story

## Purpose

Generate high-quality user stories based on proto personas and feature descriptions, following best practices from Jeff Patton, Mike Cohn, and Gojko Adzic for Next.js / React web applications in TypeScript.

## Context

This prompt creates comprehensive user stories that guide development by transforming persona insights and feature requirements into structured, testable development tasks. The process emphasizes inclusive language, INVEST criteria compliance, and integration with existing project documentation.

## Instructions

### Advanced User Story Techniques

**Use Multiple Agents** when the story creation task has independent analysis areas:
- One agent for persona analysis and user psychology
- One agent for feature breakdown and INVEST criteria validation
- One agent for technical feasibility and implementation hints
- One agent for QA test case design and edge case identification

**Apply Ultrathink** for complex features or challenging persona-feature combinations to analyze user story architecture and user journey integration before creating the stories.

**Avoid Procrastination Patterns:**
- Create comprehensive acceptance criteria immediately
- Provide actionable implementation hints
- Cover all edge cases and error scenarios
- Ensure all stories meet INVEST criteria perfectly

### Input Analysis

Analyze the provided inputs:

1. <persona>
   {{$ARGUMENTS}}
   </persona>

This contains information about the target user, including their background, goals, and pain points.

2. <feature_description>
   {{$ARGUMENTS}}
   </feature_description>

This provides a high-level overview of the feature or functionality to be developed.

### Context Analysis

Also consider:
- Current implementation status of this app
- User journeys documentation in `docs/product/user-journeys/`
- Jobs-to-be-done (JTBD) documentation in `docs/domain/jtbd/`
- Product requirements document (PRD) in `docs/product/PRD.md`
- Product backlog in `docs/product/backlog.md`
- UX documentation in `docs/` (if available)

### User Story Format and Best Practices

Follow the standard format with gender-inclusive and diverse language:
"As [type of user], I want [an action] so that [a benefit/a value]."

**Inclusive Language Requirements:**
- Use gender-neutral job titles and roles when possible
- Use diverse and inclusive examples in descriptions
- Avoid gender stereotypes in personas and scenarios
- Ensure language is respectful and inclusive of all identities

**Core Best Practices:**
1. Focus on the user's perspective and needs (Jeff Patton)
2. Keep stories simple and concise (Mike Cohn)  
3. Ensure stories are valuable, estimable, small, and testable (Bill Wake's INVEST criteria)
4. Include acceptance criteria for each story (Gojko Adzic)
5. Consider the impact on the user and the business (Jeff Patton)
6. Use inclusive, gender-neutral language throughout

### User Story Creation Process

1. Analyze the persona to understand the user's context, goals, and pain points
2. Review the feature description to identify the main functionality and purpose
3. Break down the feature into smaller, valuable chunks that align with user needs
4. For each chunk, create a user story using the standard format
5. Ensure each story is independent and can be developed and tested separately
6. Add 2-5 acceptance criteria for each user story to clarify the definition of done
7. Include technical implementation hints for developers
8. Identify if the story is for MVP or Future Release based on available information
9. Reference related JTBD, user journeys, UX documentation and affected personas with relative paths from `docs/`

## Output Format

Each story should have this structure:

```markdown
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

### Example User Story

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

- Sabine Structure-Focused (docs/product/personas/01-sabine-structure-focused.md)
- Marco Spontaneous-Planner (docs/product/personas/02-marco-spontaneous-planner.md)
- Lena Network-Builder (docs/product/personas/03-lena-network-builder.md)

## User Journey Reference

- "Family discovers platform through Instagram" (docs/product/user-journeys/00-discover-platform-via-instagram.md)
- "Complete Family Assessment" (docs/product/user-journeys/01-complete-family-assessment.md)

## UX Documentation

- Product Vision (docs/product/product-vision.md)
- Marketing Tone and Voice (docs/marketing/tone-and-voice.md)

## Implementation Scope

MVP
</example_story>

## Success Criteria

A successful user story includes:

1. **Gender-inclusive language**: Uses diverse and inclusive examples throughout
2. **Implementation scope clarity**: Clearly identified as MVP or Future Release
3. **Document alignment**: Aligns with provided documents and current implementation status
4. **Independence**: Each story can be developed and tested separately
5. **Value focus**: Uses clear, concise language that focuses on user benefits
6. **Comprehensive references**: Includes relevant acceptance criteria, technical notes, and references to JTBD and user journeys
7. **Proper documentation paths**: Always includes relative paths to referenced documentation
8. **Backlog integration**: Added to local backlog and created as a file in docs/product/user-stories/ directory

**File Management:**
- Add completed user story to `docs/product/backlog.md`
- Create corresponding user story file in `docs/product/user-stories/` directory with sequential index (e.g. `46-new-user-story.md`)
- Do not invent IDs for stories; they will be assigned automatically when created as GitHub issues

$ARGUMENTS
