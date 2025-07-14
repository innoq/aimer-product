# AIMER Prompt Guidelines

These guidelines define best practices for creating and maintaining prompts in this repository.

## Prompt Structure

Every prompt must follow this structure:

```markdown
# [Prompt Name]

## Purpose

[Clear, concise description of the prompt's goal in 1-2 sentences]

## Context

[Background information that helps the AI model understand the task]

## Instructions

[Detailed step-by-step instructions]

## Output Format

[Exact description of the expected output]

## Success Criteria

[Measurable criteria for successful execution]

$ARGUMENTS
```

## Writing Style Guidelines

### 1. Use Imperative, Direct Language

✅ **Good:**

```markdown
Analyze the codebase structure and identify architectural patterns.
```

❌ **Avoid:**

```markdown
You should analyze the codebase structure and try to identify what architectural patterns might be present.
```

### 2. Avoid Role-Based Prompting

✅ **Good:**

```markdown
Analyze the system architecture and identify potential bottlenecks.
```

❌ **Avoid:**

```markdown
You are a senior software architect. As an expert in system design, analyze...
```

### 3. Be Specific Without Being Overly Prescriptive

✅ **Good:**

```markdown
Examine the dependency graph and identify:

- Circular dependencies
- Overly coupled components
- Missing abstractions
```

❌ **Avoid:**

```markdown
First, you must carefully examine each and every dependency. Then, you should create a detailed mental model. After that, think step by step about...
```

### 4. Structure Instructions Clearly and Logically

Use:

- Numbered lists for sequential steps
- Bullet points for enumerations
- Clear headings for different sections
- Code blocks for examples

### 5. Use $ARGUMENTS for Dynamic Parameters

The `$ARGUMENTS` placeholder allows slash commands to accept dynamic values from the user:

```markdown
## Instructions

1. Analyze the code for issue #$ARGUMENTS
2. Generate documentation following the team's style guide

$ARGUMENTS
```

**Usage Examples:**

- `/fix-issue 123` → `$ARGUMENTS` becomes `123`
- `/analyze-component Button` → `$ARGUMENTS` becomes `Button`
- `/security-review authentication` → `$ARGUMENTS` becomes `authentication`

## Output Format Specification

### 1. Define the Desired Structure Explicitly

✅ **Good:**

```markdown
## Output Format

### 1. Executive Summary

- Key findings (3-5 bullet points)
- Overall assessment score (1-10)

### 2. Detailed Analysis

For each component:

- Name and purpose
- Dependencies
- Potential issues
```

### 2. Use Examples Where Helpful

For complex outputs, show a brief example:

```markdown
## Output Format

Generate a risk assessment in the following format:

| Risk          | Severity | Likelihood | Impact   | Mitigation       |
| ------------- | -------- | ---------- | -------- | ---------------- |
| SQL Injection | High     | Medium     | Critical | Input validation |
```

## Best Practices

### 1. Focus on Essentials

- Keep prompts as short as possible, but as long as necessary
- Remove redundant instructions
- Avoid excessive details that might confuse the model

### 2. Use Clear Action Verbs

Preferred verbs:

- Analyze, Identify, Generate, Create
- Evaluate, Compare, Summarize
- Extract, List, Categorize
- Document, Explain, Describe

### 3. Structure for Reusability

- Keep prompts generic enough for different codebases
- Use $ARGUMENTS for dynamic user input and specific customizations
- Avoid hardcoded technology assumptions

### 4. Test and Iterate

- Test prompts with various examples
- Document known limitations
- Update based on user feedback

## Advanced Prompt Techniques

### 1. Subagents for Parallel Task Processing

When prompts involve multiple independent analysis areas, use subagents to process tasks in parallel:

**When to use Multiple Agents:**

- Complex analysis requiring different expertise areas
- Independent research tasks that can be processed simultaneously
- Large-scale analysis with multiple components
- Tasks requiring different perspectives or approaches

**Example Pattern:**

```markdown
**USE MULTIPLE AGENTS** when the task has independent analysis areas:
"I'll spawn agents to analyze different aspects of this problem:"

- One agent for technical analysis and dependencies
- One agent for UI/UX considerations and mobile patterns
- One agent for domain modeling and persona analysis
- One agent for test planning and quality assurance
```

### 2. Ultrathink and Sequential Thinking

For complex analysis requiring deep reasoning:

**Ultrathink Pattern:**
Use for scenarios requiring comprehensive analysis before action:

```markdown
**ULTRATHINK FOR COMPLEX ANALYSIS:**
For complex problems or challenging evaluations, say:
"Let me ultrathink about this [problem/analysis] before finalizing the approach."
```

**Sequential Thinking Pattern:**
Use for systematic, step-by-step analysis:

```markdown
**SEQUENTIAL THINKING:**

- Break complex problems into logical sequences
- Process one step thoroughly before moving to the next
- Build upon previous findings systematically
- Validate conclusions at each step
```

### 3. WebSearch for Research and Validation

Incorporate web research for current information and validation:

**When to use WebSearch:**

- Technology validation and best practices
- Market research and competitive analysis
- Cost estimation and tool comparison
- Current framework and security recommendations
- Regulatory compliance information

**Example Pattern:**

```markdown
**Use WebSearch** for:

- Technology validation and best practices
- Market research and competitive analysis
- Cost estimation and tool comparison
- Current framework and security recommendations
```

### 4. Anti-Patterns to Avoid

**PROCRASTINATION PATTERNS (FORBIDDEN):**

- "I'll detail this in the implementation phase" → NO, analyze thoroughly now
- "The technical details can be figured out later" → NO, identify challenges now
- "We'll see what's needed during development" → NO, anticipate requirements now
- "This is good enough for planning" → NO, create comprehensive analysis

## Quality Criteria for Prompts

A good AIMER prompt:

1. **Is self-explanatory**: Can be understood without additional context
2. **Produces consistent results**: Delivers comparable outputs for similar inputs
3. **Is action-oriented**: Leads to concrete, actionable results
4. **Follows a clear format**: Uses the standardized structure
5. **Is tested**: Has been validated with real examples

## Common Mistakes to Avoid

### 1. Instructions That Are Too Vague

❌ **Avoid:**

```markdown
Look at the code and find problems.
```

✅ **Better:**

```markdown
Analyze the codebase for:

- Security vulnerabilities (OWASP Top 10)
- Performance bottlenecks
- Code quality issues (complexity, duplication)
```

### 2. Excessive Chain-of-Thought Prompting

❌ **Avoid:**

```markdown
First, think about what makes good architecture. Then, consider how this applies here. Next, reason through each component and write down your thoughts into a scratchpad...
```

✅ **Better:**

```markdown
Evaluate the architecture against these criteria:

- Separation of concerns
- Scalability
- Maintainability
```

### 3. Missing Output Structure

❌ **Avoid:**

```markdown
Provide your analysis of the system.
```

✅ **Better:**

```markdown
Structure your analysis as:

1. System Overview (1 paragraph)
2. Key Strengths (3-5 points)
3. Critical Issues (prioritized list)
4. Recommendations (actionable items)
```

## Integration with Claude Code

Prompts are optimized for use as custom slash commands in Claude Code:

1. **Clarity**: Each prompt works standalone without additional context
2. **Flexibility**: $ARGUMENTS allows for dynamic user input and project-specific adjustments
3. **Consistency**: Uniform structure across all prompts
4. **Efficiency**: Optimized for token usage and response quality

### Additional Claude Code Features

**Bash Command Execution:**
Execute bash commands using `!` prefix:

```markdown
Current git status: !`git status`
Current branch: !`git branch --show-current`
```

**YAML Frontmatter:**
Add metadata to command files:

```markdown
---
allowed-tools: Bash(git add:*), Bash(git status:*)
description: Create a git commit
---
```

## Maintenance and Updates

1. **Versioning**: Use Git for change tracking
2. **Testing**: Test prompts with real examples before committing
3. **Documentation**: Update README for new prompts
4. **Review**: Peer review for significant changes

## Automated Quality Assurance

For CI/CD integration, the following checks can be implemented:

1. **Structure validation**: All required sections present
2. **Style checks**: No forbidden patterns (e.g., role-based prompting)
3. **Format consistency**: Markdown formatting correct
4. **$ARGUMENTS presence**: Placeholder present at the end

These guidelines are intended to be living documents - updates based on new insights and user feedback are welcome.

## Markdown stylistics

- Ensure correct heading structure
- A prompt MUST start with a h1 heading
