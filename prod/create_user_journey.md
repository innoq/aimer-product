# Create User Journey

## Purpose

Generate a comprehensive user journey map based on product documentation that documents the end-to-end experience of a user accomplishing a specific goal with the product.

## Context

User journey maps visualize how users navigate through a product to accomplish goals, connecting product requirements to realistic user behavior patterns. They help identify pain points, optimization opportunities, and alignment with Jobs to Be Done analysis.

## Instructions

1. **Analyze Input Sources**
   - Review Product Requirements Document (PRD): docs/product/PRD.md
   - Examine Jobs to Be Done analysis: docs/domain/jtbd/
   - Check existing personas: docs/product/personas/
   - Review existing user journeys: docs/product/user-journeys/

2. **Select Persona and Define Goal**
   - Choose appropriate persona from existing documentation
   - Clearly state what the user is trying to accomplish
   - Connect goal to specific jobs from JTBD analysis
   - Explain motivation and context for this goal

3. **Map the Journey**
   - Divide journey into logical phases (5-8 phases recommended)
   - Document specific touchpoints for each phase
   - Include user actions, thoughts, and system responses
   - Note emotional responses at each touchpoint
   - Identify pain points, moments of delight, or confusion
   - Connect to specific PRD features

4. **Create Comprehensive Documentation**
   - Include alternative paths and error scenarios
   - Document both digital and non-digital touchpoints
   - Reflect persona's specific characteristics and preferences
   - Show realistic emotional responses throughout

## Output Format

### Persona Selection
- **Persona Name**: [Brief description focusing on characteristics relevant to this journey]
- **Why This Persona**: [Explanation of why this persona is well-suited for this journey]

### Goal Definition
- **Primary Goal**: [Clear statement of what user wants to accomplish]
- **JTBD Connection**: [How this connects to specific jobs from analysis]
- **Motivation**: [Context and driving factors for this goal]

### Starting Situation
- **Current State**: [User's situation before beginning the journey]
- **Existing Tools/Workarounds**: [What they currently use]
- **Journey Trigger**: [What initiates this journey]

### Journey Phases

#### Phase [N]: [Phase Name]
**Touchpoint [N]: [Interface Element/Screen Name]**
- **User Action**: [What the user does]
- **System Response**: [How the system responds]
- **User Thought**: [What the user is thinking]
- **Emotional State**: [User's emotional state]
- **Pain Points**: [Any friction or confusion]

### Outcome
- **End Result**: [Whether goal was achieved]
- **User Satisfaction**: [How user feels about the outcome]
- **Follow-up Actions**: [What happens next]

### Optimization Potential
- [Specific improvement suggestion with rationale]
- [Additional improvement with impact assessment]
- [Long-term enhancement opportunity]

### JTBD Alignment
- **Functional Jobs**: [How journey addresses functional needs]
- **Emotional Jobs**: [How journey addresses emotional needs]
- **Social Jobs**: [How journey addresses social needs]

## Success Criteria

- Journey reflects realistic user behavior patterns
- All touchpoints include emotional states and system responses
- Pain points and optimization opportunities are clearly identified
- Strong connection to JTBD analysis and PRD features
- Alternative paths and error scenarios are documented
- Cohesive narrative that guides development priorities
- Actionable insights for improving user experience

$ARGUMENTS