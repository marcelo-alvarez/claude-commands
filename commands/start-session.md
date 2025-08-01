# Start Session Command

This command initializes a Claude Code session by loading all necessary context and setting up for productive work.

## Usage

```
/start-session
```

## Implementation Steps

**IMPORTANT: This command ONLY reads files and reports status. DO NOT write code, create files, or implement features.**

1. Run /mcp__serena__initial_instructions i.e. "read Serena's initial instructions"
2. **Load Project Guidelines**: Read `CLAUDE.md` for project-specific protocols (if not present create a minimal one)
3. **Load Session Context**: Read `context.md` for previous session state (if not present create a minimal one)
4. **Decide Whether to Continue**: If both 1 and 2 were missing, return
5. **Check Project Status**: Review git status and current branch (DO NOT make commits or changes)
6. **Synthesize Context**: Provide structured summary of current state and next actions

**CONSTRAINTS:**
- DO NOT implement any features from tasks.md
- DO NOT write application code
- DO NOT create project files beyond CLAUDE.md/context.md
- ONLY read, analyze, and report
- Never modify tasks.md - it's the reference checklist for the current tasks

## Output

The command provides a comprehensive session summary including:
- Project understanding and current phase
- Test status and baseline protection requirements
- Next actions and priorities
- Key constraints and protocols