# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Overview

AIMER Product is a collection of AI-assisted product development prompts. The repository contains structured prompt templates designed to help developers plan an prototype software products using AI assistance.

## Architecture

The repository has a simple structure:

- `prod/` - Contains all prompt templates as Markdown files that are production-ready
- `experiments/` - Contains prompt templates as Markdown files that might work but are not ready for production
- `ideas`- Contains ideas as prompts as Markdown files that don't work yet but are placeholders for later prompt templates
- Each prompt file follows a consistent format with Purpose, Context, Instructions, Output Format, and Success Criteria sections
- All prompts include an `$ARGUMENTS` placeholder for additional contextual information

## Working with Prompts

When modifying or creating new prompts, please refer to `prompt-guideline.md` for detailed best practices. Key points:

1. Follow the standardized structure: Purpose, Context, Instructions, Output Format, Success Criteria, $ARGUMENTS
2. Use imperative, direct language without role-based prompting
3. Be specific without being overly prescriptive
4. Define explicit output formats with examples where helpful
5. Test prompts with real examples before committing

See `prompt-guideline.md` for the complete guidelines, including common mistakes to avoid and quality criteria.

## Workflow Usage

For comprehensive guidance on using the AIMER Product workflows, including step-by-step instructions, methodology backgrounds, recommended inputs, and usage patterns, see [**HOWTO.md**](HOWTO.md). This guide covers the complete product development workflow from idea to implementation.

## Integration with Claude Code

This repository is designed to be used as custom slash commands in Claude Code:

- Can be cloned into `.claude/commands` for project-specific use
- Can be added as a Git submodule for version tracking
- Can be installed in `~/.claude/commands` for user-wide availability
