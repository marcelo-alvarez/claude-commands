
# Run Development Cycle Command

This command executes a complete development cycle.

## Usage
```
/run-dev-cycle
```

## Implementation

Execute the following sequence of commands in order. 

1. **Start Session**
   `/clear`
   Then follow all instructions in `~/.claude/commands/start-session.md`

2. **Continue Work**
   Then follow all instructions in `~/.claude/commands/continue-work.md`

3. **Save Context**
   Follow all instructions in `~/.claude/commands/save-context.md`

4. **Audit**
   `/clear`
   Then Follow all instructions in `~/.claude/commands/start-session.md`
   Then follow all instructions in `~/.claude/commands/audit-context.md`
