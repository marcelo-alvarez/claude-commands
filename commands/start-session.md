# Start Session Command

This command initializes a Claude Code session by loading all necessary context and setting up for productive work.

## Usage

```
/start-session [prompt]
```

## Implementation Steps

**IMPORTANT: This command ONLY reads files and reports status. DO NOT write code, create files, or implement features.**

1. Run /mcp__serena__initial_instructions i.e. "read Serena's initial instructions"
2. Read workflow-wisdom.md if present, otherwise create an empty template indicating these are memories for proper workflow, based on previous mistakes. It should be concise and not weigh down the context too much.
3. **Load Project Guidelines**: Read `CLAUDE.md` for project-specific protocols (if not present create a minimal one)
4. **Load Current Project Tasks**: Read `tasks.md` for project-specific tasks currently being worked on (if not present create a minimal one)
5. **Load Session Context**: Read `context.md` for previous session state (if not present create a minimal one)
6. **Check Project Status**: Review git status and current branch (DO NOT make commits or changes)
7. **Synthesize Context**: Report a structured summary of current state and next actions
8. **Process prompt**: If provided, respond to the text in the prompt but do not write to disk or execute commands other than file reading

**CONSTRAINTS:**
- DO NOT implement any features from tasks.md
- DO NOT write application code
- DO NOT create project files beyond CLAUDE.md/context.md
- ONLY read, analyze, and report
- Never modify tasks.md - it's the reference checklist for the current tasks
- Never modify context.md - that's for other operations

## Output

The command provides a comprehensive session summary including:
- Project understanding and current phase
- Test status and baseline protection requirements
- Next actions and priorities
- Key constraints and protocols
If a prompt is provided, it also responds to the prompt, in read-only mode as specified above.