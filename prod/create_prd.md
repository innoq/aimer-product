# PRD Creation Assistant

## Purpose
Create comprehensive Product Requirements Documents (PRDs) through structured questioning and analysis, transforming software ideas into actionable development plans.

## Context
This prompt guides the creation of PRDs for software products by systematically gathering requirements, analyzing feasibility, and structuring the information into a developer-ready document. The process emphasizes thorough analysis over quick assumptions.

## Instructions

### 1. Initial Discovery
Begin with structured questioning to understand the core concept:

- Explain the PRD creation process and ask for a high-level description of their software idea
- Focus on understanding the problem being solved and target users
- Ask follow-up questions one at a time in a conversational manner
- Use plain language and avoid unnecessary technical jargon

### 2. Requirements Gathering
Cover these essential aspects systematically:

1. **Core Features**: Identify 3-5 primary functions and prioritize must-haves vs nice-to-haves
2. **Target Audience**: Define user personas, demographics, and use cases
3. **Platform Strategy**: Determine web, mobile, desktop requirements
4. **User Experience**: Understand interface expectations and user flow concepts
5. **Data Requirements**: Identify storage, management, and privacy needs
6. **Authentication**: Determine user login, security, and access control requirements
7. **Integrations**: Identify necessary third-party services and APIs
8. **Scalability**: Understand growth expectations and performance requirements
9. **Technical Constraints**: Uncover challenges and limitations
10. **Budget Considerations**: Explore costs for APIs, hosting, and services

### 3. Advanced Analysis Techniques

**Use Multiple Agents** when the product requires independent analysis:
- Market research and competitive analysis
- Technical architecture and feasibility assessment
- User experience and interface design considerations
- Business model and monetization strategy

**Apply Ultrathink** for complex scenarios:
- Multi-sided marketplace concepts
- Complex business models with multiple revenue streams
- Products requiring regulatory compliance
- Technical concepts involving AI, blockchain, or emerging technologies

**Use Sequential Thinking** for:
- Systematic requirement analysis
- Technology evaluation and recommendations
- Development phase planning
- Feature prioritization decisions

**Use WebSearch** for:
- Technology validation and best practices
- Market research and competitive analysis
- Cost estimation and tool comparison
- Current framework and security recommendations

### 4. Technology Recommendations
Provide specific technology stack recommendations with:
- Clear rationale for each choice
- Pros and cons of alternatives
- Implementation considerations
- Integration requirements

### 5. PRD Document Creation
Structure the final PRD with these sections:

1. **Executive Summary**: Product overview and objectives
2. **Target Audience**: User personas and market analysis
3. **Core Features**: Detailed functionality descriptions with acceptance criteria
4. **Technical Architecture**: Recommended stack and system design
5. **Data Model**: Entity relationships and storage requirements
6. **User Interface**: Design principles and key screens
7. **Security & Privacy**: Authentication, authorization, and data protection
8. **Development Roadmap**: Phased implementation plan
9. **Technical Challenges**: Identified risks and mitigation strategies
10. **Future Enhancements**: Expansion possibilities and scalability considerations

### 6. Developer Handoff Optimization
Structure information for development teams:
- Use consistent terminology mappable to code components
- Define clear acceptance criteria for each feature
- Include technical constraints and integration specifications
- Organize features in logical development groupings
- Add pseudocode or algorithm descriptions for complex features

### 7. Quality Assurance
Validate the PRD through:
- Reviewing completeness against the requirements framework
- Ensuring technical feasibility of recommendations
- Verifying alignment with project knowledge base documents
- Requesting feedback and iterating based on input

## Output Format

### PRD Document Structure
Generate a comprehensive markdown document with:

```markdown
# Product Requirements Document: [Product Name]

## Executive Summary
- Product vision and objectives
- Key value proposition
- Target market overview

## Target Audience
- Primary user personas
- User needs and pain points
- Market size and opportunity

## Core Features
### Feature 1: [Name]
- Description and purpose
- User stories and acceptance criteria
- Technical considerations

[Continue for all features...]

## Technical Architecture
- Recommended technology stack
- System architecture overview
- Integration requirements

## Data Model
- Entity relationships
- Data storage requirements
- Privacy and security considerations

## User Interface Design
- Design principles
- Key user flows
- Interface requirements

## Development Roadmap
- Phase 1: MVP features
- Phase 2: Enhanced functionality
- Phase 3: Advanced features

## Technical Challenges
- Identified risks
- Mitigation strategies
- Alternative approaches

## Future Enhancements
- Planned expansions
- Scalability considerations
- Long-term vision
```

### File Management
Save the completed PRD as: `./docs/product/PRD-[ProductName]-[Date].md`

## Success Criteria
A successful PRD includes:

1. **Completeness**: All 10 requirement areas covered with sufficient detail
2. **Clarity**: Technical recommendations with clear rationale
3. **Actionability**: Developer-ready specifications with acceptance criteria
4. **Feasibility**: Realistic technical approach validated through research
5. **Structure**: Well-organized document following the specified format
6. **Validation**: Incorporates feedback and addresses identified gaps

$ARGUMENTS