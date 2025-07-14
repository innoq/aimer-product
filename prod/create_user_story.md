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

User stories should follow the standard format but with gender-inclusive and diverse language:
"Als [Benutzer*in/Rolle] möchte ich [eine Aktion] können, damit [ein Nutzen/ein Wert]."
(German language format with gender-inclusive terms: "As a [type of user], I want [an action] so that [a benefit/a value].")

IMPORTANT: Always use gender-inclusive language in your user stories. For example:

- Use "Benutzer\*in" instead of "Benutzer"
- Use "Nutzer\*in" instead of "Nutzer"
- Use "Manager\*in" instead of "Manager"
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
## Beschreibung
Als [Benutzertyp] möchte ich [eine Aktion] können, damit [ein Nutzen/ein Wert].

## Akzeptanzkriterien
1. [Kriterium 1]
2. [Kriterium 2]
3. [Kriterium 3]
...

## Bezug zu JTBD
- [Reference to relevant jobs-to-be-done from docs/domain/jtbd/]

## Betroffene Personas
- [List of personas affected by this story from docs/product/personas/]

## Bezug zu User Journeys
- [Reference to specific user journeys from docs/product/user-journeys/]

## UX-Dokumentation
- [Reference to relevant UX documentation with relative paths from docs/]

## Implementation Scope
[MVP/Future Release]

```

Present your output in markdown format.

Here's an example of a well-formed user story for this app:

<example_story>

## Beschreibung

Als Knowledge Manager möchte ich Prompts nach verschiedenen Kriterien kategorisieren können, damit ich eine strukturierte Promptbibliothek aufbauen und pflegen kann.

## Akzeptanzkriterien

1. Benutzer können benutzerdefinierte Tags für Prompts erstellen und zuweisen.
2. Benutzer können Prompts nach Tags filtern und sortieren.
3. Benutzer können die Kategoriestruktur jederzeit anpassen und erweitern.
4. Benutzer können Tags mit Farben oder Icons versehen, um die visuelle Unterscheidung zu erleichtern.
5. Benutzer können verschachtelte Kategorien erstellen, um eine Hierarchie zu bilden.

## Bezug zu JTBD

- "Wenn ich als Familie unsere Organisation verbessern möchte, will ich eine übersichtliche Kategorisierung, damit ich ähnliche Bereiche leicht finden kann."
- "Wenn ich nach Lösungen für unsere Familien-Herausforderungen suche, möchte ich nach relevanten Kategorien filtern können, damit ich die passenden Ansätze schneller finde."

## Betroffene Personas

- Sabine Strukturiererin (docs/product/personas/01-sabine-strukturiererin.md)
- Marco Spontanplaner (docs/product/personas/02-marco-spontanplaner.md)
- Lena Netzwerkerin (docs/product/personas/03-lena-netzwerkerin.md)

## Bezug zu User Journeys

- "Familie entdeckt klyngl über Instagram" (docs/product/user-journeys/00-klyngl-ueber-instagram-entdecken.md)
- "Family Assessment durchlaufen" (docs/product/user-journeys/01-family-assessment-durchlaufen.md)

## UX-Dokumentation

- Product Vision (docs/product/product-vision.md)
- Marketing Tone and Voice (docs/marketing/tone-and-voice.md)

## Implementation Scope

MVP
</example_story>

Remember to:

- Write user stories in German using gender-inclusive and diverse language (use \* for gender-inclusive terms).
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

**WICHTIG**: Nachdem Sie die User Story erstellt haben, fügen Sie diese in das lokale Backlog (`docs/product/backlog.md`) und erstellen Sie eine entsprechende User Story Datei im `docs/product/user-stories/` Verzeichnis mit einem fortlaufenden Index (z.B. `46-neue-user-story.md`).
