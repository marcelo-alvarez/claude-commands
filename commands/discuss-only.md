# Discuss Only Command

This command tells Claude Code to only note the provided information or discuss it without taking any actions or modifying files.

## Usage

```
/discuss-only [content]
```

## Examples

```
/discuss-only architecture patterns for the authentication system
```

```
/discuss-only please note that commit 48ttt9e has a critical bug that affects user authentication
```

## Implementation

When this command is used, Claude Code will:
- Note the topic mentioned in the argument in its context window
- Answer any questions about the topic
- Provide analysis, explanations, or discussions as requested
- **NEVER** modify, create, or edit any files
- **NEVER** execute any commands that change the system state
- **NEVER** take any actions beyond discussion and analysis

The purpose is to enable pure discussion and knowledge sharing without any risk of unintended modifications to the codebase or system.

IMPORTANT: This is a read-only mode. No file modifications, command executions, or system changes are permitted when this command is active for the current turn.