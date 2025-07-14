# Prioritize User Story Maps

## Purpose

Create prioritized CSV files from all existing user story maps by consolidating, deduplicating, and organizing stories by priority and user journey flow.

## Context

This process extracts user stories from multiple story maps, removes duplicates, and organizes them into MVP and future release categories while maintaining the natural user journey flow.

## Instructions

1. **Extract stories** from all user story maps in `docs/product/user-story-maps/`
2. **Consolidate duplicates** by identifying stories with identical content
3. **Separate by priority** into MVP and Future release groups
4. **Sort by user journey** to reflect natural navigation flow through the product
5. **Generate CSV files** for each priority group

### CSV Structure

Generate files with the following format:
```csv
ID,User Activity,User Task,Story,Source
PM001,"Discover & Browse Prompts","Search for prompts","As a technical consultant, I want to search for prompts with keywords so that I can quickly find relevant prompts during customer meetings","Prompt Management"
```

Where:
- **ID**: Unique identifier with source prefix (NM=New Member, O=Organization, PM=Prompt Management, PE=Prompt Evolution)
- **User Activity**: Higher-level user activity/epic
- **User Task**: Specific task/feature
- **Story**: User story in format "As a [persona], I want to [action] so that [benefit]"
- **Source**: Origin story map name

## Output Format

Generate consolidated CSV file in `docs/product/user-story-maps/`:

**Consolidated Stories**: `user-stories.csv` - Contains all stories from all maps, deduplicated and sorted by user journey flow, with both MVP and Future stories in one file

## Success Criteria

- All user stories are extracted from existing story maps
- Duplicate stories are identified and consolidated
- Stories are sorted to reflect natural user journey flow with MVP stories first
- Single CSV file is generated with correct structure and naming
- All metadata and attributes are preserved from original stories
- File is saved as `docs/product/user-story-maps/user-stories.csv` for workflow compatibility

$ARGUMENTS