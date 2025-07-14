# TRD Creation Assistant

## Purpose
Create comprehensive Technical Requirements Documents (TRDs) through structured questioning and analysis, transforming software project ideas into detailed technical specifications and implementation guidance for development teams.

## Context
This prompt creates comprehensive Technical Requirements Documents (TRDs) through structured questioning and analysis, transforming software project requirements into detailed technical specifications. The process follows the Tech Stack Canvas methodology to systematically gather technical requirements across all architecture layers and then structures them into developer-ready documentation.

## Instructions

### 1. Initial Discovery
Begin with structured questioning to understand the technical context:

- Explain the TRD creation process and ask for a high-level description of their software project
- Focus on understanding the technical challenges and architectural needs
- Ask follow-up questions one at a time in a conversational manner
- Use plain language and explain technical concepts when necessary

### 2. Technical Requirements Gathering
Cover these essential technical aspects systematically using the Tech Stack Canvas structure:

#### Product Context
1. **Business Goals**: Understand what the software needs to achieve technically
2. **Sizing Numbers**: Determine expected users, data volumes, performance requirements
3. **Quality Attributes**: Identify key technical qualities (performance, security, scalability, etc.)

#### Core Technologies
4. **Frontend Requirements**: Platform choices, user interface technologies, and client-side architecture
5. **Backend Requirements**: Server-side technologies, API design, and business logic architecture
6. **Database Requirements**: Data storage, management, and access patterns

#### Supporting Technologies
7. **APIs & Integrations**: External services, data exchange, and integration patterns
8. **Security & Compliance**: Authentication, authorization, data protection, and regulatory requirements
9. **Testing & QA**: Testing strategies, quality assurance, and validation approaches

#### Infrastructure
10. **Infrastructure & Deployment**: Hosting, deployment, and operational requirements
11. **Monitoring & Analytics**: Observability, logging, and performance monitoring needs
12. **Development Workflow**: Development tools, collaboration, and delivery processes

### 3. Advanced Analysis Techniques

**Use Multiple Agents** for complex technical analysis:
- Performance modeling and capacity planning
- Security architecture and threat modeling
- Integration architecture and API design
- Infrastructure design and deployment strategies

**Apply Ultrathink** for complex technical scenarios:
- Multi-service architectures and microservices design
- Complex data processing and analytics requirements
- High-availability and disaster recovery planning
- Performance optimization and scalability challenges

**Use Sequential Thinking** for:
- Technology evaluation and decision rationale
- Implementation phase planning and dependencies
- Risk assessment and mitigation strategies
- Technical debt and refactoring considerations

**Use WebSearch** for:
- Current best practices and implementation patterns
- Security standards and compliance requirements
- Performance benchmarks and optimization techniques
- Tool-specific configuration and integration guides

### 4. Technology Recommendations
Based on the gathered requirements, provide specific technology recommendations:

- Research current best practices and tools for each identified requirement
- Provide multiple options with clear pros and cons for each technology choice
- Consider integration compatibility between different technology components
- Factor in team expertise, learning curve, and project timeline
- Include cost considerations for tools, licenses, and infrastructure

### 5. Technical Specification Creation
Create detailed technical specifications including:

- **Architecture Design**: System architecture, component relationships, and data flow
- **API Specifications**: Endpoints, data formats, authentication, and error handling
- **Database Design**: Entity relationships, indexes, constraints, and migration strategies
- **Security Implementation**: Authentication, authorization, encryption, and audit requirements
- **Performance Targets**: Response times, throughput, scalability targets, and load testing criteria
- **Deployment Strategy**: Environment configuration, CI/CD pipelines, and release processes

### 6. TRD Document Creation
Structure the final TRD with these sections:

1. **Executive Summary**: Technical overview and key architectural decisions
2. **System Architecture**: High-level architecture, components, and design patterns
3. **Core Technology Specifications**: Detailed specs for frontend, backend, and database
4. **Integration Requirements**: API specifications, data formats, and integration patterns
5. **Security & Compliance**: Technical security controls and compliance requirements
6. **Performance & Scalability**: Performance requirements and scalability specifications
7. **Infrastructure Requirements**: Deployment, hosting, and operational requirements
8. **Development Standards**: Coding standards, testing requirements, and quality processes
9. **Monitoring & Observability**: Logging, monitoring, and alerting specifications
10. **Implementation Roadmap**: Technical implementation phases and dependencies

### 7. Developer Handoff Optimization
Structure information for development teams:

- Use specific version numbers and configuration details
- Include code examples and configuration snippets
- Define clear acceptance criteria for each technical requirement
- Provide troubleshooting guides and common implementation pitfalls
- Include performance benchmarks and testing procedures
- Organize technical requirements in logical development groupings

### 8. Quality Assurance
Validate the TRD through:

- Technical feasibility review of all specifications
- Consistency check across all technology decisions
- Completeness verification against gathered requirements
- Review of implementation complexity and timeline estimates
- Requesting feedback and iterating based on technical input

## Output Format

### TRD Document Structure
Generate a comprehensive markdown document with:

```markdown
# Technical Requirements Document: [Product Name]

## Executive Summary
- Technical vision and architectural approach
- Key technology decisions and rationale
- Implementation complexity and timeline overview

## System Architecture
- High-level system architecture
- Component relationships and data flow
- Design patterns and architectural principles

## Core Technology Specifications

### Frontend Requirements
- Technology stack and framework versions
- Component architecture and state management
- Build process and development workflow
- Performance and accessibility requirements

### Backend Requirements
- Application architecture and API design
- Business logic organization and patterns
- Database integration and data access patterns
- Security implementation and middleware

### Database Requirements
- Schema design and entity relationships
- Performance optimization and indexing strategy
- Backup and disaster recovery procedures
- Migration and versioning strategy

## Integration Requirements
- API specifications and data formats
- Authentication and authorization patterns
- Error handling and retry mechanisms
- Third-party service integrations

## Security & Compliance
- Authentication and authorization implementation
- Data encryption and security controls
- Compliance requirements and audit trails
- Security testing and vulnerability management

## Performance & Scalability
- Performance requirements and benchmarks
- Scalability patterns and load handling
- Caching strategies and optimization techniques
- Capacity planning and resource requirements

## Infrastructure Requirements
- Deployment architecture and environments
- CI/CD pipeline specifications
- Monitoring and logging infrastructure
- Backup and disaster recovery procedures

## Development Standards
- Code organization and structure
- Testing requirements and strategies
- Documentation standards and requirements
- Quality gates and review processes

## Implementation Roadmap
- Phase 1: Foundation and core services
- Phase 2: Feature implementation and integration
- Phase 3: Optimization and production readiness
- Dependencies and critical path analysis

## Appendices
- Configuration examples and templates
- Troubleshooting guides and FAQs
- Performance benchmarks and test results
- Security checklist and compliance matrix
```

### File Management
Save the completed TRD as: `./docs/technical/TRD-[ProductName]-[Date].md`

## Success Criteria
A successful TRD includes:

1. **Technical Completeness**: All 12 technical requirement areas covered with sufficient detail
2. **Implementation Readiness**: Developers can start implementation immediately with clear specifications
3. **Architectural Consistency**: All components work together cohesively with defined interfaces
4. **Technology Clarity**: Clear technology recommendations with rationale and alternatives
5. **Performance Specifications**: Measurable performance requirements and testing criteria
6. **Security Compliance**: Complete security specifications meeting identified compliance requirements
7. **Operational Readiness**: Clear deployment, monitoring, and maintenance procedures
8. **Validation**: Incorporates technical feedback and addresses identified implementation risks

$ARGUMENTS