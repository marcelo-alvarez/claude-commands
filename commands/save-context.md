# Save Context Command

This command saves the current session context to `context.md` for continuity between Claude Code sessions.

## Usage

```
/save-context [optional note]
```

## Examples

```
/save-context
```

```
/save-context just completed utility extraction phase
```

## Implementation

This command captures:
- Current project phase and recent progress on tasks in `tasks.md` and bugs in `bugs.md`
- Recent discoveries and decisions
- Next steps and blockers

The context is saved to `context.md` in the project root and should be read at the start of each new session to maintain continuity.

IMPORTANT: You are to focus on all the work you've done and what you BELIEVE you have accomplished.DO NOT claim ANYTHING HAS ACTUALLY BEEN ACCOMPLISHED. This will be left to a future instance to check, with fresh context.

Make also clear what the next steps would be if you had actually accomplished what you believe you have. make no other changes this turn. Remember, you are done and only documenting what you believe. YOU ARE NOT TO VALIDATE OR CLAIM ANYTHING WAS ACTUALLY ACCOMPLISHED. A FUTURE INSTANCE WILL CHECK LATER.

Never modify tasks.md - it's the reference checklist for the current tasks
