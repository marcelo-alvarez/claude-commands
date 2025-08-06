
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

2. **Audit Context**
   Follow all instructions in `~/.claude/commands/audit-context.md`

3. **Continue Work**
   Then follow all instructions in `~/.claude/commands/continue-work.md`

4. **Save Context**
   Follow all instructions in `~/.claude/commands/save-context.md`

5. **Final Audit**
   `/clear`
   Then Follow all instructions in `~/.claude/commands/start-session.md`
   Then follow all instructions in `~/.claude/commands/audit-context.md`
