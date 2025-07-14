# AIMER Product Workflow: From Idea to Prototype

## Suggested File Structure

The workflows essentially generate markdown documentation in these directories, which can then be used as context for AI agents (or human developers) during implementation:

```
├── docs/
│   ├── domain/          # JTBD documentation, user research
│   ├── marketing/       # Tone & Voice guidelines, competitive analysis
│   ├── product/         # PRD, product vision, canvases, personas
│   ├── reference/       # Input documents, glossaries, meeting summaries
│   ├── rules/           # Development guidelines, coding standards, team conventions
│   ├── technical/       # TRD, architecture decisions, API specs
│   ├── ux/              # User journeys, UX flows, wireframes
│   └── .../             # Additional project-specific directories
```

## Input References

Before starting the workflow, it's highly recommended to collect and organize existing documentation in the `/docs/reference/` directory. This provides essential context that workflow prompts can leverage as input, resulting in more accurate and relevant outputs.

**Recommended reference documents could be:**

- Dossiers
- Meeting Summaries
- Studies, Research & Statistics
- Other internal documents
- Glossaries
- Corporate Design / Style Guide
- Tone & Voice Guidelines
- Competitive Analysis

Having these documents readily available allows the following workflow prompts to incorporate existing knowledge, maintain consistency with established guidelines, and build upon previous work rather than starting from scratch.

## Workflow Overview

This workflow follows proven product development methodologies and is aligned with the Software Development Life Cycle (SDLC) phases **Product Vision** → **Research & Requirements** → **Experiments & Prototyping** → **Implementation & Rampup**.

## ⚠️ Important: Human Review and Team Collaboration Required

**These prompts are designed to accelerate documentation, not replace human judgment.** Each step requires:

- **Human review and validation** of AI-generated outputs
- **Team collaboration** during creation - many steps work best when developed in groups
- **Iterative refinement** based on stakeholder feedback
- **Domain expertise** to ensure accuracy and relevance

The AI assists with structure and initial content, but **human insight and team alignment are essential** for creating successful products.

**Note on "Recommended Input":** The input suggestions for each step are recommendations to improve output quality, not mandatory requirements. Work with whatever documentation and context you have available - the prompts are designed to be flexible and adapt to your specific situation.

## Detailed Process

### 1. Create Product Requirements Document (PRD)

**Prompt:** [`/create_prd`](prod/create_prd.md)
**SDLC Phase:** Product Vision  
**Method:** Product Requirements Document  
**Origin:** Developed in software development, popularized by Google and other tech companies  
**Purpose:** Defines product requirements, target audience, success metrics and scope. Serves as a central reference for all stakeholders and ensures everyone works with the same understanding of the product.  
**Recommended Input:** Initial project brief, stakeholder interviews, market research, competitive analysis, business goals documentation

### 2. Create Technical Requirements Document (TRD)

**Prompt:** [`/create_trd`](experiments/create_trd.md)  
**SDLC Phase:** Architecture  
**Method:** Technical Requirements Document  
**Origin:** Complement to PRD, developed based on the Tech Stack Canvas by INNOQ  
**Purpose:** Defines technical requirements, system architecture and implementation details. Translates product requirements into technical specifications.  
**Recommended Input:** PRD, existing system documentation, technical constraints, infrastructure requirements, team capabilities

### 3. Create Tone & Voice Guidelines

**Prompt:** [`/create_tone_and_voice_guide`](experiments/create_tone_and_voice_guide.md)  
**SDLC Phase:** Product Vision  
**Method:** Brand Voice & Tone Guidelines  
**Origin:** Developed in marketing and content design, popularized by MailChimp and other content-focused companies  
**Purpose:** Defines communication strategy and brand personality. Ensures all content is communicated consistently and appropriately to the target audience.  
**Recommended Input:** Brand guidelines, target audience research, existing content samples, competitor analysis, marketing strategy

### 4. Create Product Vision (optional)

**Prompt:** [`/create_product_vision`](prod/create_product_vision.md)
**SDLC Phase:** Product Vision  
**Method:** Product Vision Statement  
**Origin:** Developed in strategic product management, popularized by Geoffrey Moore ("Crossing the Chasm")  
**Purpose:** Creates a clear, inspiring vision for the product. Particularly important for customer-facing products to align team and stakeholders.  
**Recommended Input:** PRD, company vision/mission, market analysis, stakeholder goals, long-term strategy documents

### 5. Lean Product Canvas Suite

**Prompts:** [`/create_product_canvas_chain`](prod/lean-product-canvas/create_product_canvas_chain.md)
**SDLC Phase:** Product Vision  
**Method:** Lean Product Methodology
**Origin:** Jeff Gothelf and Josh Seiden, based on the Lean UX Canvas  
**Purpose:** Provides a systematic approach to validate business hypotheses and reduce uncertainty in product development. Helps teams focus on the most critical assumptions and test them quickly and cost-effectively.  
**Recommended Input:** PRD, product vision, market research, user interviews, business model assumptions, competitive analysis  
**Available Prompts:**

- [`/create_lean_product_canvas`](prod/lean-product-canvas/create_lean_product_canvas.md) - Lean Product Canvas
- [`/create_lean_strategy_canvas`](prod/lean-product-canvas/create_lean_strategy_canvas.md) - Lean Strategy Canvas
- [`/create_hypothesis_prioritization_canvas`](prod/lean-product-canvas/create_hypothesis_prioritization_canvas.md) - Hypothesis Prioritization
- [`/create_hypothesis_tests`](prod/lean-product-canvas/create_hypothesis_tests.md) - Hypothesis Testing
- [`/create_okr_roadmap`](prod/lean-product-canvas/create_okr_roadmap.md) - OKR & Roadmap Planning

### 6. Jobs-to-be-Done (JTBD) Documentation

**Prompt:** [`/jtbd_workflow_chain`](prod/jtbd/jtbd_workflow_chain.md) - Complete JTBD Analysis  
**SDLC Phase:** Research & Requirements  
**Method:** Jobs-to-be-Done Framework  
**Origin:** Clayton Christensen (Harvard Business School), further developed by Tony Ulwick (Outcome-Driven Innovation)  
**Purpose:** Understands the fundamental "jobs" users want to accomplish. Focuses on user motivation rather than just features and helps identify innovation opportunities.  
**Recommended Input:** User interviews, survey data, customer support tickets, usage analytics, market research, existing product feedback

**Available JTBD Individual Prompts:**

- [`/jtbd_approaches`](prod/jtbd/jtbd_approaches.md) - Various JTBD approaches
- [`/jtbd_workflow_chain`](prod/jtbd/jtbd_workflow_chain.md) - Complete JTBD workflow
- [`/jtbd_job_map`](prod/jtbd/jtbd_job_map.md) - Job mapping
- [`/jtbd_outcome_statements`](prod/jtbd/jtbd_outcome_statements.md) - Define outcome statements
- [`/jtbd_forces_diagram`](prod/jtbd/jtbd_forces_diagram.md) - Create forces diagram
- [`/jtbd_job_stories`](prod/jtbd/jtbd_job_stories.md) - Write job stories
- 15+ additional specialized JTBD prompts available

### 7. Create Proto-Personas

**Prompt:** [`/create_proto_persona`](prod/create_proto_persona.md)
**SDLC Phase:** Research & Requirements  
**Method:** Proto-Personas (Assumption-based Personas)  
**Origin:** Jeff Gothelf and Josh Seiden (Lean UX), based on Alan Cooper's Persona concept  
**Purpose:** Creates hypothetical user profiles based on assumptions and existing data. Faster than complete personas, but still helpful for product decisions.  
**Recommended Input:** JTBD documentation, user research data, analytics, customer interviews, demographic data, behavioral patterns

### 8. Create User Journeys

**Prompt:** [`/create_user_journey`](prod/create_user_journey.md)
**SDLC Phase:** Research & Requirements  
**Method:** User Journey Mapping  
**Origin:** Service Design, popularized by Adaptive Path and IDEO  
**Purpose:** Visualizes the user experience across all touchpoints. Identifies pain points and optimization opportunities in user interaction.  
**Recommended Input:** Proto-personas, JTBD documentation, user research, current state analysis, touchpoint inventory, customer feedback

### 9. UX Flow Documentation

**Prompt:** [`/create_ux_flow_chain`](prod/create_ux_flow_chain.md)
**SDLC Phase:** Experiments & Prototyping  
**Method:** User Experience Flow Design  
**Origin:** Interaction Design, developed in the UX community  
**Purpose:** Defines user guidance and interaction flows. Serves as a foundation for wireframes and prototypes.  
**Recommended Input:** User journeys, proto-personas, JTBD documentation, existing UI patterns, technical constraints, business rules

### 10. Create User Story Maps

**Prompt:** [`/create_user_story_map`](prod/create_user_story_map.md)
**SDLC Phase:** Implementation & Rampup  
**Method:** User Story Mapping  
**Origin:** Jeff Patton ("User Story Mapping")  
**Purpose:** Organizes user stories in a two-dimensional representation. Uses a user journey as a basis. Helps with prioritization and understanding the user journey from a development perspective.  
**Recommended Input:** User journeys, UX flows, proto-personas, JTBD documentation, technical constraints, business priorities

### 11. Generate User Stories (Backlog)

**Prompt:** [`/generate_backlog_workflow`](prod/generate_backlog_workflow.md)
**SDLC Phase:** Implementation & Rampup  
**Method:** User Story Writing + Backlog Management  
**Origin:** Agile Software Development, popularized by Extreme Programming (Kent Beck)  
**Purpose:** Creates implementable user stories with acceptance criteria. Forms the foundation for sprint planning.  
**Recommended Input:** User story maps, UX flows, proto-personas, technical requirements, business rules, acceptance criteria guidelines

**Additional Prompts:**

- [`/create_user_story`](prod/create_user_story.md) - Create individual user stories
- [`/priorize_user_story_maps`](prod/priorize_user_story_maps.md) - Prioritize user story maps

### 12. Implementation Planning

**Prompt:** [`/plan_user_story`](prod/plan_user_story.md)
**SDLC Phase:** Implementation & Rampup  
**Method:** Story Planning & Task Breakdown  
**Origin:** Agile Software Development, Scrum Framework  
**Purpose:** Breaks down user stories into implementable tasks. Defines efforts and dependencies for development.  
**Recommended Input:** User stories with acceptance criteria, technical requirements, team capabilities, development standards, existing codebase

### 13. Implementation

**Prompt:** [`/implement_user_story`](prod/implement_user_story.md)
**SDLC Phase:** Implementation & Rampup  
**Method:** Agile Development with AI Support  
**Origin:** Agile Software Development  
**Purpose:** Supports actual implementation of user stories with code generation and best practices.  
**Recommended Input:** Implementation plans, user stories, technical specifications, coding standards, existing codebase, test requirements

## Additional Workflows

### Documentation

**Prompt:** [`/create_docs_readmes`](prod/create_docs_readmes.md)
**Purpose:** Creates (and updates) project-specific README files for existing documentation in the repository (`docs/`) for reading convenience.

**Prompt:** [`/create_readme`](experiments/create_readme.md)  
**Purpose:** Creates comprehensive README files for projects, repositories, or specific components.

## Workflow Recommendations

1. **For new products:** Go through complete workflow from PRD to implementation
2. **For feature development:** Start with JTBD or User Journey
3. **For technical products:** Create TRD after PRD
4. **For B2B products:** Focus on JTBD and User Journey Mapping
5. **For B2C products:** Prioritize Product Vision and Tone & Voice Guidelines

## Usage Tips

- Use `think` or `ultrathink` as argument for deeper analysis
- Use previous outputs as input for subsequent steps
- Adapt the sequence according to project requirements
- Iterate between steps based on new insights
