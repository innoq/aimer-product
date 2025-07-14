# Generate Product Backlog Workflow

## Purpose

Create a comprehensive product backlog from user story maps by processing CSV files and generating detailed feature descriptions and user stories.

## Context

This workflow processes user stories from CSV files, matches them with personas, generates feature descriptions, and creates detailed user stories. It maintains progress tracking and ensures systematic backlog generation.

## Instructions

1. **Initialize workflow** by checking existing progress and creating directory structure
2. **Process CSV file** `docs/product/user-story-maps/user-stories.csv` systematically
3. **Generate feature descriptions** for each story using structured template
4. **Create user stories** by using the `.claude/commands/prod/create_user_story.md` prompt
5. **Track progress** through comprehensive index document
6. **Organize backlog** by priority and backbone activities

### CSV Structure

Expected input format:

```csv
ID,User Activity,User Task,Story,Priority,Source
1,Onboarding,User registration,"As a new user, I want to create an account so that I can access the app",MVP,User Story Map
2,Search,Find rides,"As a user, I want to search for rides so that I can find transportation",MVP,User Story Map
```

### Workflow Sessions

- **New session**: `session=new` - Initialize directories and index
- **Continue session**: `session=continue` - Resume from last position
- **Final session**: `session=final` - Complete processing and summary

### Processing Steps

1. **Initialization**

   - Create directories: `docs/product/backlog/features/` and `docs/product/backlog/user-stories/`
   - Create or update index document at `docs/product/backlog/README.md`
   - Validate CSV file exists and has correct structure

2. **Story Processing**

   - Process each row from CSV file
   - Extract ID, User Activity, User Task, Story, Priority, and Source
   - Match stories with appropriate personas from `docs/product/proto-personas/`
   - Generate feature descriptions using structured template
   - Call `create_user_story.md` command with persona and feature description
   - Save files with kebab-case naming convention

3. **Progress Tracking**
   - Update index document after each processing batch
   - Maintain accurate counts and status
   - Generate continuation commands for workflow management

## Output Format

### Index Document Structure

```markdown
# Product Backlog

## Overview

This document tracks backlog creation progress from user stories CSV file.

## Processing Progress

| Processed | Total | Status         | Last Updated |
| --------- | ----- | -------------- | ------------ |
| 0/241     | 241   | ⏳ In Progress | 2023-05-06   |

## MVP Stories

### Backbone: [Backbone Name]

#### Story/Task: [Story/Task Name]

##### Story: [Story title]

[Detailed User Story]

## Next Steps

Use the following command to continue processing:
/generate_backlog_workflow start_index=5 max_stories=10 session=continue
```

### Feature Description Template

```markdown
# Feature: [User Task] within [User Activity]

This feature enables [Persona] to [perform action] in the context of [User Activity].

## Context

The feature is part of the overarching activity "[User Activity]" and focuses on the task "[User Task]".

## User Story

[Story]

## Priority

[Priority]

## Source

[Source]

## Product Context

This feature should be integrated into the application and work with existing functions for [relevant functions].
```

### File Naming Convention

- Feature descriptions: `docs/product/backlog/features/{id}.md`
- User stories: `docs/product/backlog/user-stories/{id}-{story-name}.md` (kebab-case)

## Success Criteria

- All CSV entries are processed systematically
- Feature descriptions follow exact template structure
- User stories are generated using create_user_story.md command
- Progress tracking is updated after each batch
- File naming conventions are followed consistently
- Index document maintains accurate status and links
- All generated files meet quality standards

$ARGUMENTS
