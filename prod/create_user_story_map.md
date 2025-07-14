# Create User Story Map

## Purpose

Generate a comprehensive user story map based on Jeff Patton's methodology that provides both the "big picture" of the product and detailed stories for implementation.

## Context

User story maps visualize the user journey through the product while organizing features by priority. They help teams understand the narrative flow and identify the minimum viable product (MVP) through a structured approach.

## Instructions

1. **Analyze source documents** from the provided paths
2. **Review existing maps** in `docs/product/user-story-maps/` to avoid duplicates
3. **Create narrative flow** from left to right showing user journey
4. **Structure hierarchically** with backbone activities and detailed stories
5. **Organize by priority** with MVP stories separated from future releases
6. **Generate outputs** in both markdown and CSV formats

### Story Map Structure

Create a hierarchical structure with:
- **Backbone (top row)**: Major user activities representing the workflow
- **Walking Skeleton (subsequent rows)**: Detailed tasks and stories by priority

### Story Creation Process

Use Sequential Thinking for breaking down journeys:
- Identify major user activities forming the backbone
- Break activities into specific tasks
- Create user stories delivering specific value
- Apply simple format: "As a [user], I want to [action] so that [outcome]"
- Draw release line separating MVP from future stories

### Gap Analysis

Identify missing functionality that would prevent coherent user experience and document potential issues.

## Output Format

Generate two files in `docs/product/user-story-maps/`:

### Markdown Format
```markdown
# User Story Map: [Journey Name]

## Backbone (User Activities)
Activity 1 → Activity 2 → Activity 3 → Activity 4

## Walking Skeleton (Tasks & Stories)
### Activity 1
- Task 1.1
  - As a [user], I want to [action] so that [outcome] [MVP]
  - As a [user], I want to [action] so that [outcome] [Future]
```

### CSV Format
```csv
ID,User Activity,User Task,Story,Priority,Source
1,Activity 1,Task 1.1,"As a [user], I want to [action] so that [outcome]",MVP,User Story Map
2,Activity 1,Task 1.2,"As a [user], I want to [action] so that [outcome]",Future,User Story Map
```

File naming: `user_story_map_[shortname].md` and `user_story_map_[shortname].csv`

## Success Criteria

- User story map contains clear narrative flow from left to right
- Stories are properly prioritized with MVP/Future categorization
- Both markdown and CSV formats are generated
- All stories follow "As a [user], I want to [action] so that [outcome]" format
- No duplicate stories across existing maps
- Files are saved with correct naming convention

$ARGUMENTS
