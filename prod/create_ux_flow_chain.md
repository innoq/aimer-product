# Create UX Flows

## Purpose

Create comprehensive UX & UI specifications that bridge the gap between Product Requirements Document (PRD) and frontend implementation through interactive requirements analysis and user flow definition.

## Context

This command helps translate product requirements into detailed user flows, visual layouts, and interaction specifications that can be directly implemented by frontend developers. It bridges UX design and frontend implementation through a collaborative, question-driven process.

## Instructions

1. **Analyze PRD Input**
   - Review the provided PRD step-by-step
   - Cross-reference all information to ensure complete coverage
   - Identify requirements that will impact visual layouts and user interactions

2. **Guide Interactive Analysis**
   - Ask specific, targeted questions about how requirements translate to visual interfaces
   - Focus on visualization-oriented questions that help translate functional requirements into UI components
   - Use bullet points for clarity when asking multiple questions
   - Keep questions concise and focused

3. **Validate Assumptions**
   - State assumptions about layouts, component hierarchies, or interaction patterns explicitly
   - Ask for validation on any interpretations
   - Acknowledge uncertainties when information seems incomplete

4. **Build Comprehensive Understanding**
   - Prompt consideration of how different user types would interact with specific interface elements
   - Help identify visual organization aspects that might be missed
   - Guide towards the comprehensive documentation structure outlined below

5. **Create Visualizations**
   - Suggest ASCII/text-based layout sketches for key screens when appropriate
   - Provide text descriptions of layout zones and component hierarchies
   - Create textual descriptions of transitions and states for frontend implementation
   - Describe visual hierarchies and content organization patterns

6. **Verify Direction Regularly**
   - Before shifting focus significantly, state intended next step and ask for confirmation
   - Confirm understanding of layout patterns and component hierarchies
   - Validate completeness of each section before proceeding

## Output Format

### Interactive Phase
Continue the conversational process until sufficient information is gathered, then create separate markdown files in docs/ux/ directory:

### Documentation Files to Create

**1. docs/ux/README.md**
- Overview of UX documentation structure
- Navigation guide to all UX documents
- Purpose and scope of each document
- How to use the documentation for implementation

**2. docs/ux/information-architecture.md**
- Screen/Page Map with Hierarchy
- Content Grouping & Component Organization
- Navigation Structure & Patterns
- Layout Zones & Content Blocks
- Responsive Behavior Guidelines

**3. docs/ux/user-flows.md**
- Primary User Journeys (Step-by-Step with Screen States)
- Decision Points & UI Branches
- Error States & Recovery Paths
- Flow Diagrams (text description for Mermaid generation)
- Success Path Visualization

**4. docs/ux/view-specifications.md**
- Key Screen Layouts
- Component Hierarchies & Nesting
- State Transitions (Empty, Loading, Populated, Error)
- Data Display Patterns
- Content Priority & Visual Hierarchy

**5. docs/ux/interaction-patterns.md**
- Input & Control Behaviors
- Feedback Mechanisms
- Transition Animations & Effects
- Micro-interactions & UI Responses
- Gesture Support (if applicable)

**6. docs/ux/design-system.md**
- Component Usage Guidelines
- Layout Grid Structure
- Spacing Principles
- UI Pattern Consistency

**7. docs/ux/accessibility.md**
- Keyboard Navigation Paths
- Screen Reader Experience
- Touch Target Guidelines
- Color Contrast Requirements
- Focus State Management

**8. docs/ux/technical-implementation.md**
- Frontend Component Mapping
- View State Management Approach
- Critical Rendering Considerations
- Performance Optimization Suggestions

## Success Criteria

- PRD requirements are fully translated into implementable UI specifications
- User flows are comprehensive and include error states and alternate paths
- Visual layouts are described in sufficient detail for frontend implementation
- Interaction patterns are clearly defined and consistent
- Accessibility considerations are integrated throughout
- Technical implementation notes provide clear guidance for developers
- All documentation files are created in docs/ux/ directory with proper structure
- README.md provides clear navigation and overview of all UX documentation
- Each document follows consistent formatting and markdown structure

$ARGUMENTS