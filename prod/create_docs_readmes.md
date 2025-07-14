# Documentation READMEs

## Purpose
Create and maintain README files to improve navigation through project documentation while ensuring existing READMEs remain current.

## Context
Documentation directories require clear navigation structure with links to subdirectories and files. Existing README files may become outdated as the project evolves.

## Instructions

### 1. Analyze Current Documentation Structure
- Locate the main README file for the project
- Examine the structure of the documentation directory
- Identify existing README files and their content

### 2. Create or Update README Files
For each directory in the docs structure (including the root docs directory):
- Create a README.md file if none exists
- Update existing README.md files to ensure accuracy

### 3. README File Content
Each README.md file must contain:
- Brief description of the current directory's purpose
- Complete list of all subdirectories and files in the directory
- Relative links to each subdirectory and file
- Back-link to parent directory (except for root docs README)

### 4. Link Format Standards
Use relative paths for all links:
- Same directory file: `[File Name](file-name.md)`
- Subdirectory: `[Subdirectory Name](subdirectory-name/)`
- File in subdirectory: `[File Name](subdirectory-name/file-name.md)`

### 5. Update Project Root README
Add or update the link to the docs directory in the main README.md: `[Documentation](docs/)`

## Output Format

### For Each Directory README:
```markdown
# Directory Name

Brief description of the directory's purpose.

## Contents

- [File 1](file1.md)
- [File 2](file2.md)
- [Subdirectory 1](subdirectory1/)
- [Subdirectory 2](subdirectory2/)

[Back to parent directory](../)
```

## Success Criteria
- All documentation directories have current README files
- All links use relative paths and work correctly when rendered
- Existing README files are updated to reflect current directory contents
- Navigation between documentation sections is seamless
- No broken links or missing references

$ARGUMENTS
