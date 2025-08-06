# Implement User Story

## Purpose

Implement tasks from user story plans by identifying the next open task, understanding it thoroughly, and implementing the required code changes following systematic quality standards.

## Context

This prompt guides software developers through a comprehensive implementation workflow that includes analysis, planning, coding, testing, and quality assurance. The process emphasizes high-quality standards with no shortcuts, ensuring production-ready code from the start.

## Instructions

### Critical Workflow - No Shortcuts

**Use Multiple Agents** when the implementation task has independent parts:
- One agent for codebase analysis and pattern identification
- One agent for test strategy and implementation
- One agent for quality assurance and linting
- One agent for documentation and progress tracking

**Apply Ultrathink** for complex technical decisions or challenging architectures before proceeding with the solution.

**Avoid Procrastination Patterns:**
- Fix linter warnings immediately
- Write clean code from the start
- Do it right the first time
- Test as you go
- Implement the final design now

Think deeply and systematically about each implementation step. Use reasoning abilities to carefully analyze requirements, consider different approaches, and make well-informed technical decisions.

### User Story Input

The user story file path will be provided as: $ARGUMENTS

### Implementation Steps

Follow these steps to successfully implement the task:

**Important Process Requirements:**
1. After each completed step, explicitly ask if you can proceed with the next step
2. Wait for confirmation from the user before continuing
3. After each completed step, document progress by updating implementation notes in the plan file

#### 1. Understanding the User Story

- Read the user story file from `docs/product/user-stories/` to understand the requirements
- Locate and read the corresponding plan file from `docs/plans/` to get the detailed implementation plan
- Identify the main goal, acceptance criteria, and technical requirements of the user story
- Ask after completion: "I have analyzed the user story. Is this information sufficient or do you need additional details? Should I proceed with the next step?"

#### 2. Analysis of Available Resources

- Identify all resources and references mentioned in the plan file.
- Read these documents to gain a deep understanding of the requirements.
- Pay special attention to UI designs, domain models, or architecture decisions.
- Review relevant documentation from `docs/ux/`, `docs/product/proto-personas/`, and `docs/rules/`.
- Ask after completion: "I have analyzed the resources. Should I proceed with identifying the next task to implement?"

#### 3. Identifying the Next Task

- Review the task breakdown section in the plan file to identify available tasks.
- Identify the next task that should be worked on based on the order in the task breakdown and current implementation status.
- Check if there are any implementation notes or progress indicators in the plan file.
- Determine which task is the logical next step based on dependencies and current state of the codebase.
- Ask after completion: "I have identified the next task. Is this the correct task we should work on? May I proceed with understanding the task requirements?"

#### 4. Understanding the Task

- Clearly formulate what the specific task is.
- Use the Sequential Thinking Tool for systematic analysis of this task. Introduce the tool with a clear announcement: "I will use Sequential Thinking to analyze [Task]."
- For complex technical decisions, use Ultrathink: "Let me ultrathink about this implementation approach before proceeding with the solution."
- Identify expected results and success metrics.
- Note which parts of the code need to be changed.
- Ask after completion: "I have analyzed the task. Does my understanding match your expectations? Should I proceed with searching the codebase?"

#### 4.5. Implementation Strategy

**CODE EVOLUTION RULES:**

- This is a feature branch - implement the NEW solution directly
- DELETE old code when replacing it - no keeping both versions
- NO migration functions, compatibility layers, or deprecated methods
- NO versioned function names (e.g., processDataV2, processDataNew)
- When refactoring, replace the existing implementation entirely
- If changing an API, change it everywhere - no gradual transitions

**REALITY CHECKPOINTS (MANDATORY):**

- After EVERY 3 file edits: Run linters and fix all issues immediately
- After implementing each component: Validate it works
- Before proceeding to next step: Verify current implementation is clean
- If hooks fail: STOP and fix immediately

**QUALITY GATES:**

- ALL linters must pass with ZERO warnings
- ALL tests must pass with meaningful coverage
- Feature must work end-to-end
- NO TODOs, FIXMEs, or "temporary" code allowed

#### 5. Codebase Search

- Use tools like `Grep`, `Glob`, or the `Task` tool to find relevant files in the codebase.
- Read the existing code to understand how new changes should be integrated.
- Identify possible dependencies and interfaces to other components.
- Focus on React components, Tailwind UI components, and TypeScript patterns.
- Use the WebSearch tool to research best practices and implementation approaches for the technical requirements. Start with: "I am researching implementation possibilities for [Feature]."
- Alternatively, use the context7 tool for deeper technical analysis of framework specifics like Next.js, React, Tailwind, etc. Introduce the research with: "I am conducting detailed research on [Topic]."
- Ask after completion: "I have identified the relevant parts of the codebase. Do you agree with my analysis? May I proceed with implementing the changes?"

#### 6. Implementation of Changes

**HOOKS ARE WATCHING**
The hooks will verify EVERYTHING. They will:

- Block operations if you ignore linter warnings
- Track repeated violations
- Prevent commits with any issues
- Force you to fix problems before proceeding

**IMPLEMENTATION PROCESS:**

- Design a solution that meets the requirements and fits existing conventions.
- Implement the required changes in the identified files.
- **REALITY CHECKPOINT:** After every 3 file edits, run linters and fix all issues
- Create new files or components if necessary.
- Follow the project's best practices and coding standards, especially for Next.js, React development.
- **DELETE old code** when replacing functionality - no parallel implementations
- Run linters after EVERY file creation/modification
- If a linter fails, fix it immediately before proceeding

**MANDATORY DURING IMPLEMENTATION:**

- Run `bin/lint` after each significant change
- Fix ALL linter warnings immediately
- Validate each component works after implementation
- No "I'll fix it later" mentality

Ask after completion: "I have implemented the required changes with all quality gates passed. Would you like to review the code before I proceed with testing?"

#### 7. Testing and Validation

- Write appropriate tests (unit tests, integration tests, etc.) to validate your implementation.
- Run the tests and ensure they pass successfully.
- Test various edge cases and error situations.
- Verify that the changes meet the acceptance criteria.
- Ask after completion: "The tests have been written and executed successfully. Should I proceed with quality assurance?"

#### 8. Quality Assurance

**COMPLETION CHECKLIST (ALL must be ✓)**

**MANDATORY VERIFICATION:**

- [ ] Research phase completed with codebase understanding
- [ ] Implementation approach validated and documented
- [ ] ALL linters pass with ZERO warnings
- [ ] ALL tests pass (including relevant async/mobile tests)
- [ ] Feature works end-to-end in realistic scenarios
- [ ] Old/replaced code is DELETED (no parallel implementations)
- [ ] Documentation/comments are complete and accurate
- [ ] Reality checkpoints were performed regularly
- [ ] NO TODOs, FIXMEs, or "temporary" code remains
- [ ] Code follows Next.js/React/TypeScript best practices
- [ ] Mobile-specific considerations addressed
- [ ] Hook validation passed without issues

**QUALITY VERIFICATION PROCESS:**

- Run linting and type checking to ensure code meets quality standards.
- Review the code for possible improvements like refactoring or optimizations.
- Ensure your changes don't cause unintended side effects or regression errors.
- Use `npm run lint` and TypeScript compiler checks as specified in project commands.
- **CRITICAL:** ALL items in completion checklist must be ✓ before proceeding

Ask after completion: "Quality assurance is complete with all checklist items verified. Can we proceed with the commit?"

#### 9. Commit and Documentation

- Create a meaningful commit message that clearly describes the changes.
- Follow the project's commit message guidelines from `docs/rules/`.
- Update the plan file with implementation notes and progress status.
- Ask after completion: "The changes have been committed and documented. Is there anything else I should improve or explain?"

#### 10. Task Completion

**FINAL VALIDATION:**

- Verify ALL completion checklist items are ✓
- Confirm hooks pass without any warnings or errors
- Ensure feature works end-to-end as expected
- Mark the completed task in the plan file with implementation notes.
- Update any relevant documentation if required.
- Provide a summary of what was implemented and how it meets the requirements.

**COMPLETION STANDARDS (NOT NEGOTIABLE):**

- The task is NOT complete until ALL linters pass with zero warnings
- ALL tests must pass with meaningful coverage of business logic
- The feature must be fully implemented and working end-to-end
- No placeholder comments, TODOs, or "good enough" compromises
- Old code must be deleted, not kept alongside new implementation

Ask after completion: "The task is now fully completed with all quality standards met. Is there anything else you would like me to improve or explain?"

## Output Format

Begin response with a brief summary of the user story and selected task, followed by implementation plan. Ensure response is understandable for both developers and business stakeholders.

Execute all required steps, including:
- Code changes with clean implementation
- Comprehensive tests with meaningful coverage
- Proper commits with descriptive messages
- Progress documentation throughout

The entire process should be transparent and traceable so that other team members can understand and continue the work.

Final response should contain:
- Clear description of changes made
- Test results and validation
- Next steps and recommendations

## Success Criteria

A successful implementation includes:

1. **Complete step-by-step execution**: All 10 implementation steps completed with user confirmation
2. **Quality standards met**: ALL linters pass with zero warnings, all tests pass with meaningful coverage
3. **Feature functionality**: Feature works end-to-end in realistic scenarios with no placeholder code
4. **Clean codebase**: Old/replaced code deleted, no parallel implementations, follows project best practices
5. **Documentation**: Progress tracked in plan file, implementation notes complete
6. **Process transparency**: Work is traceable and can be continued by other team members
7. **Validation complete**: Hook validation passed, completion checklist items verified
8. **Production ready**: No TODOs, FIXMEs, or "temporary" code remains

**Process Requirements:**
- Wait for explicit user confirmation after each step
- Document progress by updating plan file after each step
- Handle errors with clear explanations and solutions
- Maintain work continuity for seamless handoffs

$ARGUMENTS
